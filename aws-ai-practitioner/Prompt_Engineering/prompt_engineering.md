# Prompt Engineering

### Enhanced Prompting
- Instructions
- Context
- Input Data
- Output Indicator

### Negative Prompting
Explicitly instruct the model what not to include the response

### Prompt Performance Optimization
**System Prompts** : How the model should behave and reply

**Temperature (0-1)** : Creativity of the model's output. 
- Low (0.2) outputs are more conservative, repetitive, focused on most likely response.
- High (1.0) outputs are more diverse, creative, and unpredictable, maybe less coherent

**Top P (0-1)** : 
- Low P (0.25) : Only consider 25% most likely words, will make a more coherent response
- High P (0.99) : Consider a broad range of possible words, possibly a more creative and diverse output

**Top K** : Limits the number of probable words
- Low K (10) : More coherent response, less probable words. Get the top 10 most probable words.
- High K (500) : Consider top 500 words. More diverse and creative.

**Length** : Maximum length of the answer

**Stop Sequences** : Tokens that signal the model to stop generating output.

### Prompt Latency
How fast the model responds.

Impacted by:
- Model size
- Model type
- Number of tokens in the input
- Number of tokens in the output

Not Impacted by:
- Top P, Top K, Temperature

### Zero-Shot Prompting
Present a task to the model without providing examples ore explicit training for that specific task.
- Rely fully on the model's general knowledge.
- The larger and more capable FM, the more likely you'll get good results.

### Few-Shots Prompting
Provide examples of a task to the model to guide its output
- One example is one-shot or single-shot

### Chain of Thought Prompting
Divide the task into a sequence of reasoning steps, leading to more structure and coherence
- Using a sentence like "Think step by step" helps
- Helpful when solving a problem as a human usually requires several steps
- Can be combined with Zero-Shot or Few-Shots prompting

### Retrieval-Augmented Generation (RAG)
(RAG is not a Prompt Engineering technique but it is often compared to Prompt Engineering Technique in the exam)  
Combine the model's capability with external data sources to generate a more informed and contextually rich response.
