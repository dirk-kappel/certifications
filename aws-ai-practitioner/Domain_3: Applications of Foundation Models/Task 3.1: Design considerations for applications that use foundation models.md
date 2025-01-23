## Identify selection criteria to choose pre-trained models (for example, cost, modality, latency, multi-lingual, model size, model complexity, customization, input/output length).
**Cost**: Evaluate pricing models, including pay-per-use or subscription-based costs, and consider whether the model aligns with your budget for both training and inference.

**Modality**: Choose a model that supports the required data type, such as text, image, audio, or multi-modal capabilities.

**Latency**: Consider the time taken for inference. Low-latency models are ideal for real-time applications like chatbots, while higher latency may be acceptable for batch processing tasks.

**Multi-Lingual Support**: Opt for models with built-in multi-language capabilities if your application targets a global audience.

**Model Size**: Smaller models are typically faster and cheaper to deploy but may sacrifice accuracy, while larger models provide better performance but require more computational resources.

**Model Complexity**: Complex models may handle nuanced tasks better but could introduce higher operational and tuning costs.

**Customization**: Check whether the model supports fine-tuning or additional training to adapt to specific use cases.

**Input/Output Length**: Ensure the model can handle your application’s requirements for input and output length, particularly for tasks like long-form content generation or summarization.

## Understand the effect of inference parameters on model responses (for example, temperature, input/output length).
**Temperature**: Controls the randomness of model outputs. Lower values (e.g., 0.2) make responses more deterministic, while higher values (e.g., 0.8) increase creativity and diversity.

**Input Length**: Determines how much of the input is considered by the model. Longer inputs can provide more context but may require additional computational resources.

**Output Length**: Sets the maximum length of the generated response. Shorter outputs are suitable for concise answers, while longer ones enable detailed responses.

**Top-k Sampling**: Restricts the model to consider only the top k most likely next tokens, reducing randomness.

**Top-p Sampling (Nucleus Sampling)**: Limits the token selection to a cumulative probability p (e.g., 0.9), balancing randomness and determinism.

**Beam Search**: A decoding strategy that explores multiple paths during generation to improve response quality but may increase latency.

## Define Retrieval Augmented Generation (RAG) and describe its business applications (for example, Amazon Bedrock, knowledge base).
Retrieval-augmented generation (RAG) is a technique that supplies domain-relevant data as context to produce responses based on that data. This technique is similar to fine-tuning. However, rather than having to fine-tune an FM with a small set of labeled examples, RAG retrieves a small set of relevant documents and uses that to provide context to answer the user prompt. RAG will not change the weights of the foundation model, whereas fine-tuning will change model weights.

## Identify AWS services that help store embeddings within vector databases (for example, Amazon OpenSearch Service, Amazon Aurora, Amazon Neptune, Amazon DocumentDB [with MongoDB compatibility], Amazon RDS for PostgreSQL).
**Amazon OpenSearch Service**: Offers vector search capabilities to store and query embeddings for similarity matching, ideal for applications like recommendation systems or semantic search.

**Amazon Aurora**: Supports custom implementations of vector storage and querying, particularly when combined with extensions for handling similarity searches.

**Amazon Neptune**: A graph database that can be used for storing embeddings, especially in use cases involving relationships and connections between data points.

**Amazon DocumentDB (with MongoDB Compatibility)**: Provides flexibility in storing embeddings as JSON-like documents and supports advanced queries with integration.

**Amazon RDS for PostgreSQL**: Supports PostGIS or other extensions to store and query vector data, providing advanced spatial and similarity search capabilities.

## Explain the cost tradeoffs of various approaches to foundation model customization (for example, pre-training, fine-tuning, in-context learning, RAG).
**Pre-Training**:
- Cost: High computational and resource costs due to training from scratch on large datasets.
- Use Case: Needed for highly specific domains or tasks without existing pre-trained models.
- Tradeoff: Significant upfront investment but offers complete customization.

**Fine-Tuning**:
- Cost: Moderate, as it builds on pre-trained models with domain-specific data.
- Use Case: Ideal for enhancing performance in a specific use case or industry.
- Tradeoff: Balances cost and customization, with potential to optimize accuracy.

**In-Context Learning**:
- Cost: Low, as it doesn’t modify the model but uses context in prompts to achieve the desired output.
- Use Case: Suitable for tasks requiring temporary or lightweight customization.
- Tradeoff: Minimal cost but limited to tasks achievable through context manipulation.

**Retrieval-Augmented Generation (RAG)**:
- Cost: Medium, combining storage costs (e.g., vector databases) with retrieval and generation.
- Use Case: For applications needing real-time information retrieval (e.g., knowledge bases).
- Tradeoff: Effective for dynamic data but requires infrastructure for retrieval and model integration.

## Understand the role of agents in multi-step tasks (for example, Agents for Amazon Bedrock).
**Definition**: Agents automate and coordinate multi-step tasks by combining AI models with decision-making logic to complete complex workflows.

**Agents for Amazon Bedrock**: Enable the orchestration of multiple foundation models and APIs for tasks like data retrieval, processing, and synthesis.

**Functionality**: Agents can dynamically select the appropriate foundation model or tool for each step, reducing manual intervention and improving task efficiency.

**Use Case Examples**:
- Multi-modal tasks, such as analyzing customer sentiment (NLP) and generating visual content (image models).
- Complex decision-making workflows, such as personalized marketing campaigns or advanced troubleshooting scenarios.