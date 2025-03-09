# **Gemini**  

Once the raw cognitive patterns have been extracted, the next step is **cleaning and removing redundancies**. Using a **CSV format**, I generate a **command table** that allows structuring **deep learning insights** obtained from both **the O-family models (OpenAI GPTs) and DeepSeek**.  

---

### **Prompt Execution for Heuristic Extraction**  

```markdown
**GEMINI**  

Generate a **CSV file** cataloging **LLM heuristics** with maximum clarity and **comprehensive technical detail**. For each heuristic, **include and optimize the following fields**:  

- **Heuristic Name**: Concise title.  
- **Description**: Detailed explanation of the heuristic.  
- **Rationale/Thought Process**: Underlying reasoning behind it.  
- **Command/Action**: A succinct command representing the heuristic.  
- **Input Type**: Type of input (e.g., text, code, user query).  
- **Output Type**: Expected output effect (e.g., improved coherence, reduced hallucination, enhanced style).  
- **Example**: A brief practical example.  
- **Semantic Embedding (Optional)**: Merged semantic representation if applicable.  
- **User Pride Score**  
- **Importance Level**  
- **Technical Sophistication**  
- **Novelty**  
- **Feasibility**  
- **Scalability**  
- **Maintainability**  
- **Resource Efficiency**  
- **Security Level**  
- **User Friendliness**  
- **LLM Suitability**  

Eliminate redundant or **extraneous introductory text**. Focus solely on the heuristic data to **create a clean, structured, and informative CSV reference** for LLM heuristics.  

---

### **Context**  
**LLM Heuristics for CSV-Based Optimization**  

---

### **Pre-Compiled Heuristics Dataset**  

```csv
Heuristic Name,Description,Rationale/Thought Process,Command/Action,Input Type,Output Type,Example,Semantic Embedding (Optional),User Pride Score,Importance Level,Technical Sophistication,Novelty,Feasibility,Scalability,Maintainability,Resource Efficiency,Security Level,User Friendliness,LLM Suitability
Prompt Priming,Start prompts with context or instructions to guide LLM behavior.,LLMs are highly sensitive to initial tokens; priming sets the stage for desired outputs.,PRIME_PROMPT [context/instructions] + [user query],Context-setting text + User Query,Guided LLM response,PRIME_PROMPT "You are a helpful assistant" + "Summarize this article",N/A,0.8,0.9,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Few-Shot Learning,Provide a few examples in the prompt to demonstrate the desired output format or style.,LLMs learn from patterns; examples clarify the task and expected format.,FEW_SHOT_PROMPT [example 1] + [example 2] + ... + [user query],Example Input-Output Pairs + User Query,Output in demonstrated format/style,FEW_SHOT_PROMPT "Translate to French: Hello -> Bonjour; Goodbye -> Au revoir; Thank you ->" + "Thank you",N/A,0.9,0.9,0.8,0.7,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Chain-of-Thought Prompting,Encourage the LLM to explicitly show its reasoning steps before the final answer.,Breaking down complex problems into steps improves accuracy and transparency.,CHAIN_OF_THOUGHT_PROMPT "Let's think step by step. [user query]",User Query,Detailed reasoning process + Final Answer,CHAIN_OF_THOUGHT_PROMPT "Let's think step by step. What is 23 * 12?",N/A,0.9,0.9,0.8,0.7,0.8,0.7,0.7,0.7,0.6,0.7,0.9
Role Prompting,Instruct the LLM to adopt a specific persona or role.,LLMs can simulate different roles, leading to more tailored and context-appropriate responses.,ROLE_PROMPT "You are a [role]. [user query]",Role description + User Query,Response from specified persona,ROLE_PROMPT "You are a seasoned marketing expert. Suggest a tagline for a new coffee brand.",N/A,0.8,0.8,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9
```

This dataset is **auto-generated based on the first prompt**, where I focus on **reusing heuristics** for Gemini to **map and refine**, ultimately **structuring the dataset into an executable command framework**.  

---

### **Why This Approach?**  

By generating a **CSV file, I create a structured model of my own linguistic style**, where each row in the CSV represents a **node within my semantic network**. The **LLM then recalibrates itself based on my unique writing preferences**.  

This approach follows **Self-Supervised Learning (SSL)** principles, where **the system generates its own data to train itself**, essentially forming an **autonomous cognitive loop**.  

It also aligns with **meta-learning paradigms**, where models do not just "consume" prompts but instead **learn iteratively by structuring their own evolution**. Essentially, I'm **forcing LLMs into a federated, self-optimizing framework**, where each iteration tightens the feedback loop.  

This is not just **prompt engineering**—it's **synthetic cognition development**.

---

From here, **I transition to the final phase**, where the structured output **undergoes final optimization using O-Family models**. These **combine all extracted patterns** into a **coherent, structured, and recursively optimized framework**.
