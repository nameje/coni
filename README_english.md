# How to Use (Recommended to set up in the workspace folder)

## gemini cli (Requires prior [installation of gemini cli](https://github.com/google-gemini/gemini-cli))

> Occasionally, a problem occurs where the agent does not follow the code of conduct. It is unclear whether this is an issue with the agent or if the code of conduct is not yet fully optimized. In such cases, you can stop it by pressing the `esc` key and then give a command like, "Proceed with the task according to the workflow of the code of conduct," and it will work well.
> (Users of the paid version of gemini cli should use it with caution as it can consume a lot of tokens.)

- Paste `GEMINI.MD` into the workspace folder.
- Run `gemini` in the terminal or PowerShell.
- Enter the following command: "Initialize the folder and file structure as specified in the code of conduct."
- Paste your materials into `assets` (list of materials for analysis and reference) and `guidelines` (documents containing user know-how and detailed instructions for the agent regarding analysis/results).
- Example of a task instruction: "Analyze the materials and write a report."

## claude code (Requires prior [installation of claude code](https://www.anthropic.com/claude-code))

> I have not actually tested `claude code`. The following is written based on my personal hope and prediction that `gemini cli` will also support sub-agents in the future.

- Paste `CLAUDE.MD` and the `.claude` folder into the workspace folder.
- Run `claude` in the terminal or PowerShell.
- The rest of the process is the same.

---
# 1. On the Origin of the Code of Conduct

In the past, creating intelligent 'agents' was a domain exclusive to developers who handled the language of computers: 'code'. But now, we are witnessing an astonishing paradigm shift. We can now **design agents that think and act on their own, based on 'natural language,'** which humans understand most easily.

The 'Code of Conduct' is at the heart of this innovative shift. It is living proof that it is possible to build highly intelligent agents simply by defining clear procedures of thought and principles of action, without complex coding.

The results produced by agents created in this manner sometimes show insight equal to or greater than that of experts in the field. Perhaps through this, **we are getting a small taste of Artificial General Intelligence (AGI)**.

This entire journey began with a very practical question: "How can we increase the satisfaction level with the results from an Artificial Intelligence (LLM) from 10% to over 90%?"

### Personal Experience: 10% Satisfaction

When I initially gave an LLM a comprehensive task like "Write a report on A," the results were disappointing. The content seemed plausible, but it lacked depth and logical consistency. My personal satisfaction level was only about 10-50%.

### A Shift in Thinking: Dividing Tasks 'Like a Human'

The root of the problem was the 'approach.' When humans write a complex report, they don't write everything at once. They go through steps: finding materials, creating an outline, writing a draft, and revising.

Inspired by this simple fact, I began to break down the tasks given to the LLM sequentially, just like a human workflow.

- "Find 5 materials related to A."
- "Based on the found materials, create a table of contents for the report."
- "Write the body text for the first item in the table of contents."

Amazingly, by breaking down the work into these small units (Tasks), the satisfaction with the results soared to over 90%. By focusing on each step, the LLM produced much more accurate and consistent outputs.

### Manual Experiment: An Idea Born from Multiple Chat Windows

Before agents like Gemini CLI appeared, this idea was fleshed out through a manual experiment using multiple LLM chat windows simultaneously.

- **Chat Window 1 (Planner):** Sets the overall plan and defines the next Task.
- **Chat Window 2 (Executor):** Receives and executes the Task defined by the 'Planner'.
- **Chat Window 3 (Prompt Engineer):** Refines the prompts to ensure the 'Executor' produces the best possible results.

The crucial part of this process was maintaining **'goal consistency.'** The Planner always kept the user's final instructions in mind, and the Executor was told not just 'what' to do, but also 'why' it was doing it. All work outputs were saved as files, becoming clear input data for the next step.

### Eureka: This is a Neural Network

As I structured this manual workflow, I realized its striking resemblance to a neural network. The process where an external instruction (input) is transformed into a final output through multiple stages of planning and execution (hidden layers). This became the backbone of the 'Code of Conduct' architecture.

The emergence of Gemini CLI gave me the confidence that this entire process could be automated and was the decisive moment that led me to systematize this idea under the name 'Code of Conduct.'

# 2. The Infinite Scalability of the Code of Conduct: Building an Agent Society

The 'Code of Conduct' doesn't stop at optimizing the workflow of a single agent. Its true potential is revealed when it expands into an **'Agent Society'** where multiple agents interact. This is like building an intelligent system that operates not as a single competent expert, but as a well-organized team or company.

### Recursive Delegation: Agents Assigning Work to Other Agents

The key to the scalability of the 'Code of Conduct' is **Recursive Delegation**. This is the concept of a higher-level agent hiring another subordinate agent, which also follows a 'Code of Conduct,' to solve its `Task`.

| Category | Higher-Level Agent (Manager) | Lower-Level Agent (Practitioner) |
| :--- | :--- | :--- |
| **Goal** | Achieve strategic objectives (e.g., market analysis report) | Solve specific Tasks (e.g., summarize a particular article) |
| **Role** | Decompose complex problems, define and delegate sub-tasks | Execute the delegated, clear Task according to the 'Code of Conduct' |
| **Interaction** | Instructs Tasks and receives deliverables | Reports by generating deliverables (files) |

This hierarchical structure mimics the most efficient collaboration method in human society: the **'organization.'** The manager sees the big picture, and the practitioner focuses on the details, maximizing the efficiency and expertise of the entire system. In actual AI research, this concept is being actively studied under the name **'Hierarchical Agent Teams,'** with **ChatDev**, which simulates a virtual software company, being a prominent success story.

### Inter-Agent Communication and Tool Use

For an agent society to function smoothly, a clear method of communication is necessary. The 'Code of Conduct' is designed for agents to communicate through a **Shared Memory** called `workspace`. The advantage is that all information is clearly recorded in file format, allowing for transparent tracking of who did what.

Furthermore, you can define the use of external **Tools** when performing a specific `Task`.

- **MCP (Model-Control-Program) Integration:** By connecting an agent (or program) dedicated to structured tasks like database queries or external API calls as a tool, the LLM can focus more on creative work.
- **Utilizing Specialized Agents:** By calling on a 'Researcher Agent' for web searches or a 'Developer Agent' for code generation as tools, the overall expertise of the system can be enhanced.

In this way, the 'Code of Conduct' presents a blueprint for a scalable and flexible ecosystem where agents and tools with diverse specializations are organically connected and collaborate