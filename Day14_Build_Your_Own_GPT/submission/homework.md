trainer = SFTTrainer(
    model=model,
    train_dataset=data,
    peft_config=peft_config,
    dataset_text_field="text",
    args=training_arguments,
    tokenizer=tokenizer,
    packing=False, # HOMEWORK
    max_seq_length=512
)


Here, packing=False means the trainer processes each text example one by one instead of combining several shorter ones into a single long sequence (up to 512 tokens).
If it were packing=True, it would group multiple short texts together to make better use of space and speed up training — but with False, each text stays separate for clarity and simplicity.