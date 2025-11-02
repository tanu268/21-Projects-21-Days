The notebook explores how CrewAI can be used to create AI agents and automate workflows. It walks through a few experiments, showing how agents can work together to complete tasks.

1. Content Creation Workflow:

Multiple agents were set up for content planning, writing, and editing.

Each agent had a specific task: planning content on a given topic, writing a blog post from that plan, and editing the final post.

These agents were combined into a Crew that executed tasks sequentially.

When the workflow was started with the topic “Artificial Intelligence”, the output showed the process in action—for example, the Market Researcher agent searched for AI trends to gather relevant information.

2. Customer Support Workflow:

Agents were defined for senior support and quality assurance.

A web scraping tool was added to help access documentation.

Tasks were created for resolving customer inquiries using the tool and for reviewing the responses.

A Crew was set up with memory enabled to handle sequential tasks.

The workflow was initiated with a customer question about setting up a Crew with memory, and the output showed how the agents used tools and delegated tasks to solve the inquiry.

3. Market Analyst Crew:

The notebook also tried to build a market analysis workflow:

Libraries like crewai, crewai-tools, and langchain-google-genai were installed.

A Gemini model and a Serper search tool were initialized using API keys.

A Market Researcher agent was set up with the search tool and Gemini model.

A Content Writer agent was defined with the ability to delegate tasks.

Research and writing tasks were created, and a marketing crew was assembled to execute them sequentially.

When the crew was kicked off, there were some errors related to the delegation tool and argument validation.

Despite the errors, the initial research task ran successfully, and the output—summarizing the latest AI trends—was saved in a file called blog_post.md.

In short: the notebook demonstrates how CrewAI workflows can be set up and executed, shows how agents and tools interact, and highlights both successes and challenges—like errors in delegation—but still produces useful outputs such as the research report.