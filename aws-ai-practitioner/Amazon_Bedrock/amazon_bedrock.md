# Amazon Bedrock
Fully managed service
Access is provided to Foundation Models
Unified API

## AWS Console - Bedrock
- Providers : List of Foundation Model providers that are available.
  - API usage examples are provided.
- Model Access : Shows all models that you have access to. You must first enable the model before using it.
  - Enable all models : This will request access to all.
    - Enabling does not cost money. Using the models will cost money.
- Playgrounds : Provide examples for using the models.
  - Text : Select provider and model
  - Chat : 
  - Image : Provide a text prompt to create an image.
- Custom Models : Enrich a base model with your own data.
    - Fine Tuning a Model:
        - Data is added via S3 buckets.
        - Hyperparameters : Configurations for how the algorithm should behave.
        - Need to purchase provision throughput to run this.
        - Provide unlabeled data to continue the training of the foundation model.
        - Also called domain-adaptation fine-tuning, to make a model expert in a specific domain.
        - Feed input using JSON
    - Transfer Learning : The broader concept of re-using a pre-trained model to adapt it to a new related task.
        - Widely used for image classification.

### Base Foundation Model
- How to choose?
    - Model types, performance requirements, capabilities, constraints, compliance
    - Level of customization, model size, inference options, licensing agreements, context windows, latency
    - Multimodal models (varied types of input and outputs)
- What is Amazon Titan?
    - High-performing Foundation Models from AWS
    - Image, text, multimodal model choices via fully-managed APIs
    - Can be customized with your own data
- Smaller models are more cost effective

### Automatic Evaluation
- Evaluate a model for quality control
- Built-in task types:
  - Text summarization
  - Question and answer
  - Text classification
  - Open-ended text generation
- Bring your own prompt dataset or use built-in curated prompt datasets
- Scores are calculated automatically

**ROUGE** : Recall-Oriented Understudy of Gisting Evaluation
- Evaluating automatic summarization and machine translation systems
- ROUGE-N : Measure the number of matching n-grams between reference and generated text
- ROUGE-L : Longest common subsequence between reference and generated text

**BLEU** : Bilingual Evaluation Understudy
- Evaluated the quality of generated text, especially for translations
- Considers both precision and penalizes too much brevity

**BERTScore** :
- Semantic similarity between generated text
- Uses pre-trained BERT models (Bidirectional Encoder Representations from Transformers) to compare the contextualized embeddings of both texts and computes the cosine similarity between them.

**Perplexity** : How well the model predicts the next token (lower is better)

Business Metrics to Evaluate a Model On
- User Satisfaction
- Average Revenue Per User (ARPU)
- Cross-Domain Performance
- Conversion Rate
- Effeciency