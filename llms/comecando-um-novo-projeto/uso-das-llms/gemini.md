# Gemini

Bom, com os pensamentos gerados, o objetivo é limpar e remover redundancias, onde através de uma tabela csv, gero uma tabela de comando, assim, utilizando tando o deep learnig da familia O e do deepseek

```markdown
**GEMINI**

Generate a CSV file cataloging LLM heuristics with maximum clarity and comprehensive detail. For each heuristic, include and optimize the following columns:

- **Heuristic Name**: A concise title.
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

Eliminate redundant or extraneous introductory text. Focus solely on the heuristic data itself to create a clean, informative CSV reference for LLM heuristics.

**Context**: LLM Heuristics for CSV Organization

**Pre-Compiled Heuristics Data**:

Heuristic Name,Description,Rationale/Thought Process,Command/Action,Input Type,Output Type,Example,Semantic Embedding (Optional),User Pride Score,Importance Level,Technical Sophistication,Novelty,Feasibility,Scalability,Maintainability,Resource Efficiency,Security Level,User Friendliness,LLM Suitability
Prompt Priming,Start prompts with context or instructions to guide LLM behavior.,LLMs are highly sensitive to initial tokens; priming sets the stage for desired outputs.,PRIME_PROMPT [context/instructions] + [user query],Context-setting text + User Query,Guided LLM response,PRIME_PROMPT "You are a helpful assistant" + "Summarize this article",N/A,0.8,0.9,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Few-Shot Learning,Provide a few examples in the prompt to demonstrate the desired output format or style.,LLMs learn from patterns; examples clarify the task and expected format.,FEW_SHOT_PROMPT [example 1] + [example 2] + ... + [user query],Example Input-Output Pairs + User Query,Output in demonstrated format/style,FEW_SHOT_PROMPT "Translate to French: Hello -> Bonjour; Goodbye -> Au revoir; Thank you ->" + "Thank you",N/A,0.9,0.9,0.8,0.7,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Chain-of-Thought Prompting,Encourage the LLM to explicitly show its reasoning steps before the final answer.,Breaking down complex problems into steps improves accuracy and transparency.,CHAIN_OF_THOUGHT_PROMPT "Let's think step by step. [user query]",User Query,Detailed reasoning process + Final Answer,CHAIN_OF_THOUGHT_PROMPT "Let's think step by step. What is 23 * 12?",N/A,0.9,0.9,0.8,0.7,0.8,0.7,0.7,0.7,0.6,0.7,0.9
Role Prompting,Instruct the LLM to adopt a specific persona or role.,LLMs can simulate different roles, leading to more tailored and context-appropriate responses.,ROLE_PROMPT "You are a [role]. [user query]",Role description + User Query,Response from specified persona,ROLE_PROMPT "You are a seasoned marketing expert. Suggest a tagline for a new coffee brand.",N/A,0.8,0.8,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Temperature Scaling,Adjust the temperature parameter during decoding to control randomness.,Temperature affects the probability distribution; higher values increase randomness, lower values increase determinism.,TEMP_SCALE_DECODE [temperature value],Decoding parameters,Varied text generation style (creative vs. factual),TEMP_SCALE_DECODE temperature=0.2 (for factual), TEMP_SCALE_DECODE temperature=1.0 (for creative),N/A,0.7,0.8,0.6,0.5,0.8,0.7,0.7,0.9,0.7,0.7,0.8
Top-P Sampling,Dynamically select from the most probable tokens whose cumulative probability exceeds a threshold (p).,Focuses on the most likely tokens while allowing for some diversity.,TOP_P_DECODE [p value],Decoding parameters,Balanced text generation (between coherence and diversity),TOP_P_DECODE p=0.9 (select from top 90% probability mass),N/A,0.7,0.8,0.6,0.5,0.8,0.7,0.7,0.9,0.7,0.7,0.8
Frequency Penalty,Penalize tokens that have already appeared frequently in the generated text.,Reduces repetition and encourages the model to explore less frequent tokens.,FREQ_PENALTY_DECODE [penalty strength],Decoding parameters,Less repetitive and more diverse text,FREQ_PENALTY_DECODE penalty_strength=0.5,N/A,0.6,0.7,0.6,0.5,0.7,0.6,0.6,0.8,0.7,0.6,0.7
Presence Penalty,Penalize tokens based on whether they have appeared at all in the generated text.,Discourages the model from repeating topics or concepts.,PRESENCE_PENALTY_DECODE [penalty strength],Decoding parameters,Text with broader topic coverage,PRESENCE_PENALTY_DECODE penalty_strength=1.0,N/A,0.6,0.7,0.6,0.5,0.7,0.6,0.6,0.8,0.7,0.6,0.7
Reinforcement Learning from Human Feedback (RLHF),Fine-tune LLMs using human preferences to align model behavior with human values.,Directly optimizes models for desired qualities like helpfulness and harmlessness.,RLHF_FINE_TUNE [preference data],Preference data (human ratings),Models aligned with human preferences,RLHF_FINE_TUNE using datasets of preferred responses,N/A,0.9,0.9,0.9,0.8,0.7,0.8,0.7,0.7,0.9,0.8,0.9
Constitutional AI,Guide LLM behavior with a constitution of principles during training and inference.,Provides explicit ethical and behavioral guidelines for the model to follow.,CONSTITUTIONAL_AI_GUIDE [constitution document],Constitution document,Ethically guided and principle-adherent responses,CONSTITUTIONAL_AI_GUIDE using "Do no harm" principle,N/A,0.8,0.9,0.8,0.7,0.7,0.7,0.7,0.7,0.9,0.8,0.9
Retrieval-Augmented Generation (RAG),Augment LLM knowledge by retrieving relevant information from external knowledge sources.,Overcomes LLM knowledge limitations by grounding responses in up-to-date or domain-specific data.,RAG_GENERATE [user query] + RETRIEVE [relevant docs],User Query + External Knowledge Source,Knowledge-enhanced and contextually relevant responses,RAG_GENERATE "What is the capital of Brazil?" + RETRIEVE from Wikipedia,N/A,0.9,0.9,0.8,0.7,0.9,0.8,0.8,0.7,0.7,0.8,0.9
Self-Correction/Refinement,Prompt LLM to review and refine its own initial drafts.,Iterative refinement improves quality and reduces errors.,SELF_CORRECT_PROMPT "Draft: [initial draft]. Refine this draft.",Initial LLM Draft,Improved and refined LLM output,SELF_CORRECT_PROMPT "Draft: The sky is blue becaus... Refine this draft.",N/A,0.8,0.8,0.7,0.6,0.8,0.7,0.7,0.7,0.6,0.7,0.8
Output Formatting Heuristics,Instruct LLMs to output in specific formats (JSON, CSV, lists).,Facilitates structured data extraction and parsing for downstream applications.,FORMAT_PROMPT "Output in [format]: [user query]",Format specification + User Query,Structured output in specified format,FORMAT_PROMPT "Output in JSON: List the capitals of Europe.",N/A,0.7,0.8,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9
Style Transfer Heuristics,Guide LLMs to adopt a specific writing style (formal, informal, poetic).,Allows tailoring the output tone and style to match the desired context or audience.,STYLE_PROMPT "Write in [style] style: [user query]",Style specification + User Query,Output text with specified style,STYLE_PROMPT "Write in a formal style: Explain quantum physics.",N/A,0.7,0.8,0.7,0.6,0.8,0.7,0.7,0.7,0.6,0.8,0.9
Hallucination Mitigation Heuristics,Strategies to reduce factual inaccuracies in LLM outputs.,Improves reliability and trustworthiness of LLM-generated content.,MITIGATE_HALLUCINATION [strategy] + [user query],User Query,Factually more accurate output,MITIGATE_HALLUCINATION "Verify facts" + "Explain the theory of relativity.",N/A,0.9,0.9,0.8,0.7,0.8,0.7,0.7,0.9,0.8,0.8,0.9
Context Window Management,Strategies for effectively using the limited context window of LLMs.,Maximizes information utilization within the constraint of the context window.,CONTEXT_WINDOW_MANAGE [strategy] + [input text],Long Input Text,Efficient processing of long texts,CONTEXT_WINDOW_MANAGE "Summarize sections" + [long document],N/A,0.7,0.8,0.7,0.6,0.8,0.7,0.7,0.8,0.7,0.7,0.8
Iterative Refinement Prompting,Refine prompts iteratively based on LLM outputs to achieve desired results.,Trial and error approach to prompt engineering,ITERATIVE_PROMPT [initial prompt] -> [LLM output] -> [refined prompt]...,User Query,Optimized LLM response over iterations,ITERATIVE_PROMPT "Initial prompt: Summarize article" -> [bad summary] -> "Refined prompt: Summarize concisely...",N/A,0.8,0.8,0.7,0.7,0.8,0.7,0.7,0.7,0.6,0.7,0.8
Data Augmentation for Fine-tuning,Increase the diversity and size of fine-tuning datasets using heuristic-based augmentations.,Improves model generalization and robustness with limited data.,DATA_AUGMENT [augmentation technique] + [dataset],Limited Dataset,Enhanced fine-tuning dataset,DATA_AUGMENT "Back-translation" + [English dataset],N/A,0.7,0.7,0.7,0.6,0.8,0.7,0.8,0.7,0.6,0.7,0.8
Ensemble Decoding,Combine outputs from multiple decoding strategies or models.,Reduces variance and improves the overall quality and robustness of generated text.,ENSEMBLE_DECODE [decoding strategies/models],Decoding parameters/Multiple models,More robust and higher quality text,ENSEMBLE_DECODE [Temperature Sampling, Top-P Sampling],N/A,0.8,0.8,0.7,0.6,0.8,0.7,0.7,0.9,0.7,0.7,0.8
Constraint Satisfaction Prompting,Incorporate constraints or limitations into prompts to guide LLM generation.,Ensures outputs adhere to specific requirements or formats.,CONSTRAINT_PROMPT "Answer in under 50 words: [user query]",User Query + Constraints,Output adhering to constraints,CONSTRAINT_PROMPT "Answer in under 50 words: Explain blockchain.",N/A,0.7,0.8,0.7,0.6,0.9,0.8,0.8,0.7,0.6,0.8,0.9

```

No caso, essa tabela foi gerada no primeiro prompt, onde foquei em reutilizar as heuristicas para o Gemini mapear, e assim gero as instruções para o modelo que quero incorporar.

### Por que faço isso

Ao gera **um CSV, crio** um **modelo estruturado da minha linguagem**, onde cada linha do CSV representa um nó dentro da tua rede semântica. A IA usa isso para **se recalibrar em função das tuas próprias preferências de escrita**.

Essa abordagem lembra **Aprendizado Auto-Supervisionado** (Self-Supervised Learning), onde **o próprio sistema gera os dados necessários para treinar a si mesmo**.
