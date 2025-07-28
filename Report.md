# Preface: A Blueprint for an Intelligent Partner, the Code of Conduct

The advancement of Artificial Intelligence (AI), especially Large Language Models (LLMs), has opened a new door of possibilities for us. We are now entering an era where we go beyond simply asking AI for information and entrust it with solving complex tasks. However, a broad instruction like "write a report" rarely leads to a satisfactory result. Why is that?

This is because we overlook the way humans work. We naturally break down complex tasks into steps such as **'Data Collection → Analysis → Synthesis → Reporting.'** By focusing on each stage, we enhance the completeness of the final output.

The **Code of Conduct** originates from this very point. It is an **operational principle and architecture** designed for an LLM agent to mimic the systematic work process of humans, decomposing complex tasks into clearly defined **Phase → Stage → Task** and executing them sequentially.

Beyond simply dividing tasks, the 'Code of Conduct' assigns clear roles like 'Planner' and 'Executor' and transparently records the process and output of all tasks, guiding the LLM to produce consistent results without losing its **'Chain of Thought.'**

In this article, we will examine the core philosophy and structure of the 'Code of Conduct,' explore why it aligns with the latest AI research trends, and investigate its potential to transform AI from a mere tool into a true **'Intelligent Partner.'**

---
# Part 1: The Core Philosophy of the Code of Conduct - Why is Structure Important?

Telling an LLM to "write a report" is like telling an explorer to "discover a new continent" without a map or a compass. With luck, they might discover something, but most will end up adrift in the vast ocean. The reason LLMs exhibit logical leaps or hallucinations when faced with complex tasks is the same: they lack a clear path to the goal, that is, a **Structure**.

The core philosophy of the 'Code of Conduct' is that **"Complexity is conquered through decomposition."** It provides a 'map' that guides the LLM not to lose its way by breaking down a single massive request into manageable smaller units and connecting them in a logical sequence.

| Structure of the Code of Conduct | Goal |
| :--- | :--- |
| **Phase** | Defines the largest steps of the entire task. (e.g., Analysis -> Strategy -> Execution) |
| **Stage** | Defines the specific stages within each Phase. (e.g., 'Data Collection' Stage within the 'Analysis' Phase) |
| **Task** | Defines the smallest unit of execution to be performed in each Stage. (e.g., 'Read Document A') |

This hierarchical structure goes beyond simply dividing tasks; it clarifies the purpose and output of each step, helping the LLM to clearly recognize what it needs to do now and what it needs to pass on to the next step.

---

### **Validation of My Thoughts: When Personal Intuition Meets the Latest AI Research**

> **Original Thought:** "If tasks are grouped and processed in units of stages and phases, the satisfaction will diverge to infinity."

This idea was not just a personal intuition. Surprisingly, it aligns precisely with the **core strategies** that the AI research community is currently focusing on to enhance the reasoning abilities of LLMs.

- **Academic Proof:** The expression 'satisfaction will diverge to infinity' is discussed more concretely in academia as **"Improved Complexity Management," "Error Reduction,"** and **"Consistent Reasoning Performance."** The hierarchical structure of the 'Code of Conduct' is an actively researched field known as **'Hierarchical Planning'** and is recognized as one of the most effective approaches for solving complex problems.

- **Relationship with Major Research:**
  - **Chain-of-Thought (CoT):** This technique, which prompts the LLM to explain its thought process step-by-step, is similar to the most basic `Task` unit of the 'Code of Conduct.'
  - **Tree-of-Thought (ToT):** ToT, which explores multiple thought paths, can be seen as the process of considering various `Tasks` within a `Stage` of the 'Code of Conduct.'
  - **MetaGPT:** This framework, where multiple specialized agents collaborate, directly corresponds with the philosophy of the 'Code of Conduct' in which roles like 'Planner' and 'Executor' are distributed.

**In conclusion, the structured approach presented by the 'Code of Conduct' can be considered one of the most validated and effective methodologies for overcoming the inherent limitations of LLMs and maximizing their potential.**

---
# Part 2: The Architecture of the Code of Conduct - A Surprising Similarity to Artificial Neural Networks

Delving deeper into the structure of the 'Code of Conduct,' we find that it operates like a well-designed intelligent system, going beyond merely dividing tasks. Interestingly, this architecture shows a surprisingly similar structural characteristic to the **Artificial Neural Network**, the foundation of modern deep learning.

| Code of Conduct Architecture | Artificial Neural Network Analogy | Explanation |
| :--- | :--- | :--- |
| **Input (instructions, assets, guidelines)** | **Input Layer** | The first gateway that receives information from the external world. |
| **Phase / Stage** | **Hidden Layers** | The core processing units that process and abstract input information over several steps, extracting higher-level meaning. |
| **Task** | **Node** | The smallest unit that performs a specific operation (computation) in each layer. |
| **Chain of Execution** | **Weights** | Represents the connection strength between nodes, determining how much influence information will have when passed to the next layer. The 'Chain of Execution,' where the output of a previous Task becomes the input of the next, plays a role similar to these weights. |
| **Final Output (outputs)** | **Output Layer** | The point where the final result, after all processing is complete, is sent out to the external world. |

This analogy suggests that the 'Code of Conduct' can be viewed not just as a simple workflow, but as a **massive Computational Graph that systematically processes and transforms the flow of information.**

---

### **Validation of My Thoughts: Does the Proposed Architecture Align with the Principles of Modern Multi-Agent Systems?**

> **Original Thought:** "Separating roles like Planner and Executor, and using a file system (workspace) as shared memory, is similar to the structure of an artificial neural network."

This architecture is more than just an analogy; it aligns perfectly with the core principles of the latest multi-agent systems.

- **Validity of Role Division:** In the 'Code of Conduct,' the 'Planner' sets the plan and the 'Executor' handles the execution. This is the same principle as in frameworks like **MetaGPT** or **AutoGen**, where agents with different specializations collaborate. This is a key strategy for increasing the efficiency and stability of the entire system through the **'Division of Labor.'**

- **Collaboration via File System:** Using the `workspace` and `db` folders as a common data space referenced by all agents is a concrete implementation of the **'Shared Memory'** model among multi-agent communication methods. This enables more flexible and scalable collaboration than the 'Message Passing' method, where agents send messages directly to each other. MetaGPT's 'Co-Learning' mechanism, which shares experiences among agents, is also based on this shared memory philosophy.

**In conclusion, the architecture of the 'Code of Conduct' not only shares structural similarities with the information processing methods of artificial neural networks but is also a highly effective model that implements the validated core principles of multi-agent systems: 'role division' and 'collaboration through shared memory.'**

---
# Part 3: The Code of Conduct in Practice - Why Must We Force 'Thought'?

Modern LLMs generate surprisingly fluent and helpful responses. However, this 'helpfulness' often comes at the cost of 'deep thought.' The 'Alignment' process, aimed at making models safer and more user-friendly, ironically tends to guide models to choose the most immediate and safe 'action (response)' rather than thinking deeply about complex problems.

This is precisely why a framework like the 'Code of Conduct' is necessary. Instead of waiting for the model to think on its own, it **explicitly demands and forces a process and direction of thought**, thereby avoiding the trap of immediate answers and eliciting a higher level of reasoning.

The 'Code of Conduct' forces 'thought' in the following ways:

1.  **Demanding Explicit Outputs:** Every `Task` must leave a physical file (the result of thought) in the `output_path`. This compels the model not to remain in abstract thought but to materialize its thinking into a concrete output.
2.  **Providing Step-by-Step Information:** The next `Stage` or `Task` only receives the explicit outputs generated in the previous step as input. This steers the model away from the temptation to process everything at once and encourages it to focus on the given information to think step-by-step.
3.  **Forcing Perspective through Role Assignment:** The 'Planner' must always consider the overall plan and the next steps, while the 'Executor' must be faithful only to the given `task_purpose`. This division of roles forces each agent to look at the problem from a specific perspective, enabling a more multifaceted and in-depth analysis.

---

### **Validation of My Thoughts: Do Models Really Prioritize 'Action' Over 'Thought'?**

> **Original Thought:** "The latest models have a strong tendency to prioritize action over thought, so it's necessary to forcibly inject methods, directions, and philosophies of thinking."

This insight is a phenomenon that aligns exactly with the **'Alignment Tax'** and the **'Side Effects of Instruction Tuning'** discussed in actual AI research.

- **The Price of the Alignment Tax:** In the process of making models 'Helpful and Harmless,' a decline in other abilities, such as complex reasoning or creativity, is observed. Models become biased towards choosing the safest answer, avoiding deep reasoning that could lead to potentially risky or controversial conclusions. This is the core reason for the 'action-first' tendency that users perceive.

- **The Necessity of 'Thought Injection':** To solve this problem, your solution to "forcibly inject a framework of thought" is very valid.
    - Techniques like **Chain-of-Thought (CoT)** or **Tree-of-Thought (ToT)** are the most representative 'thought injection' methodologies that prevent the model from generating immediate answers by making it explicitly output its 'thought process.'
    - The 'Code of Conduct' takes this a step further. Beyond simply listing the thought process, it defines **"in what direction and philosophy, and according to what procedure to think"** throughout the entire system via the structured framework of `Phase → Stage → Task` and clear role division. This is akin to externally bestowing a higher level of 'Metacognition' ability upon the LLM.

**In conclusion, the 'Code of Conduct' is an essential mechanism for overcoming the limitations of the 'aligned' nature of the latest LLMs. It does not suppress the model's free thinking but rather acts as a 'guardrail' that helps it to think in a deeper, more structured, and more consistent direction.**

---
# Part 4: The Future of the Code of Conduct - Towards a Recursive Agent Society

The 'Code of Conduct' is more than just a framework for solving a single task; it holds infinite potential for expansion into a much larger intelligent system. Its future lies in the implementation of a **'Recursive Agent Society.'**

This refers to a structure where the smallest unit of execution in the 'Code of Conduct,' the `Task`, is delegated to a subordinate agent that also follows a 'Code of Conduct.'

**High-level Agent (Manager):**
- "Create a competitor analysis report" (Phase)
- "Analyze the latest trends of Company A" (Stage)
- **"Summarize Company A's Q3 earnings report" (Task) → Delegate to a sub-agent**

**Sub-agent (Practitioner):**
- (Input: "Summarize Company A's Q3 earnings report" Task)
- "Analyze data" (Phase)
- "Extract key metrics" (Stage)
- "Extract sales data" (Task)
- ...
- (Output: "Summary of Company A's Q3 Earnings Report.md")

This **Recursive Delegation** structure is an exact match to how a human organization collaborates, with managers and practitioners. The high-level agent focuses on strategic decisions, while the sub-agent concentrates on specific execution, maximizing the efficiency and expertise of the entire system.

---

### **Validation of My Thoughts: Is Such an Agent Organization Science Fiction?**

> **Original Thought:** "If the executor at the task level is replaced by a subordinate CLI that acts as an agent following the same Code of Conduct, it can evolve into an agent that operates with a dual structure (a form similar to a human organization)."

This idea is no longer in the realm of science fiction. It is a concept being actively implemented at the forefront of AI research under the name **'Hierarchical Agent Teams.'**

- **The Case of ChatDev:** The most representative example is **ChatDev**, which simulates a virtual software company. Agents with clear roles such as 'CEO,' 'CTO,' 'Programmer,' and 'Tester' collaborate under the direction of a superior manager to develop actual software. This is powerful evidence that the hierarchical delegation structure proposed by the 'Code of Conduct' is indeed feasible.

- **Expansion to an Agent Society:** Furthermore, research is underway to simulate an **'Agent Society'** where these agents interact with their own motivations and beliefs. This could be used to understand complex social phenomena or to build highly autonomous distributed systems.

- **Connection to Neural Network Architecture:** The idea of applying the hierarchical structure of the 'Code of Conduct' to actual artificial neural network design is also very pioneering. This could be conceptually linked to advanced neural network theories such as dividing the network into functional **'Modules'** and dynamically determining the path of information flow based on the input, known as **'Dynamic Routing.'** In other words, the 'Code of Conduct' may be presenting a blueprint for future, more efficient and flexible AI architectures.

**In conclusion, the recursive and hierarchical extensibility of the 'Code of Conduct' is not a mere fantasy but aligns perfectly with the direction in which current AI research is heading. It will be the key to evolving AI from a mere collection of tools into a true 'intelligent system' that can decompose problems, collaborate, and learn organizationally on its own.**

---
# Appendix: Problems and Limitations of the Code of Conduct

While the 'Code of Conduct' is a powerful framework for maximizing the potential of LLMs, it has several clear problems and limitations at the current level of technology.

### 1. The Token Limit Dilemma

The core of the 'Code of Conduct' is to go through a sufficient 'thought' process. However, all the plans and intermediate outputs generated through `Phase`, `Stage`, and `Task` become the input, or Context, for the next step. This results in the rapid depletion of the limited Context Window available to the LLM.

- **Problem:** The more you break down the steps for sufficient thought, the more the context grows exponentially, making it easy to hit the token limit.
- **Reality:** Current LLMs, especially API-based services, are sensitive to token usage, creating a trade-off between the ideal implementation of the 'Code of Conduct' and realistic operational costs.

### 2. Orchestrator Inefficiency

In a structure like the current Gemini CLI, the top-level agent acting as the Orchestrator must use all plans and task details as context.

- **Problem:** The Orchestrator only needs to perform a 'traffic control' role of invoking the next step according to rules, yet it needs to know all the details, leading to unnecessary token consumption.
- **Alternative:** This role does not necessarily need to be filled by a powerful LLM. It could be much more efficient to use a simple state machine written in code, or a smaller, less powerful model dedicated solely to progress management.

### 3. Fundamental Model Dependency

The 'Code of Conduct' structures and guides the reasoning process of an LLM, but it cannot overcome the fundamental limitations that the LLM itself possesses.

- **Problem:** The 'Code of Conduct' cannot make an LLM do something it is incapable of. For example, if an LLM has no knowledge in a specific domain, it cannot produce meaningful results no matter how finely the steps are divided.
- **Conclusion:** The success of the 'Code of Conduct' is entirely dependent on the baseline performance (knowledge, reasoning ability, etc.) of the underlying LLM.

Despite these limitations, the 'Code of Conduct' points to an important direction for how we should interact and collaborate with LLMs. As models' context windows expand and more efficient agent architectures are developed, it is expected that these problems will gradually be resolved.