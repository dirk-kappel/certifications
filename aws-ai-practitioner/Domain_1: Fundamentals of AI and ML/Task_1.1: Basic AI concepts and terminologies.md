## Define basic AI terms (for example, AI, ML, deep learning, neural networks, computer vision, natural language processing [NLP], model, algorithm, training and inferencing, bias, fairness, fit, large language model [LLM]).
**Artificial Intelligence**: AI is a broad field that encompasses the development of intelligent systems capable of performing tasks that typically require human intelligence, such as perception, reasoning, learning, problem-solving, and decision-making. AI serves as an umbrella term for various techniques and approaches, including machine learning, deep learning, and generative AI, among others.

**Machine Learning**: ML is a type of AI for understanding and building methods that make it possible for machines to learn. These methods use data to improve computer performance on a set of tasks.

**Deep Learning**: Deep learning uses the concept of neurons and synapses similar to how our brain is wired. An example of a deep learning application is Amazon Rekognition, which can analyze millions of images and streaming and stored videos within seconds.

**Generative AI**: Generative AI is a subset of deep learning because it can adapt models built using deep learning, but without retraining or fine tuning. Generative AI systems are capable of generating new data based on the patterns and structures learned from training data.

**Neural Networks**: Neural networks have lots of tiny units called nodes that are connected together. These nodes are organized into layers. The layers include an input layer, one or more hidden layers, and an output layer.

**Computer Vision**: A field of artificial intelligence that makes it possible for computers to interpret and understand digital images and videos. Deep learning has revolutionized computer vision by providing powerful techniques for tasks such as image classification, object detection, and image segmentation.

**Natural Language Processing [NLP]**: A branch of artificial intelligence that deals with the interaction between computers and human languages. Deep learning has made significant strides in NLP, making possible tasks such as text classification, sentiment analysis, machine translation, and language generation.

**Model**: A mathematical representation trained to perform a specific task, such as predicting outcomes or classifying data.

**Algorithm**: A set of rules or procedures followed by a computer to solve a problem or perform a task.

**Training**: The process of teaching a model by feeding it labeled data to learn patterns.

**Inferencing**: Using a trained model to make predictions or decisions based on new, unseen data.

**Bias**: Systematic error introduced in a model due to skewed training data or flawed algorithms.

**Fairness**: Ensuring AI systems provide equitable outcomes for all user groups, avoiding discrimination.

**Fit**: A measure of how well a model represents the data it's trained on. Overfitting occurs when it fits training data too closely, missing general patterns.

**Large Language Model [LLM]**: Models that can understand and generate human-like text. They are trained on vast amounts of text data from the internet, books, and other sources, and learn patterns and relationships between words and phrases. Examples include GPT and BERT.

## Describe the similarities and differences between AI, ML, and deep learning.
AI, ML, and deep learning are interconnected fields with shared goals of mimicking or enhancing human intelligence through data-driven systems. AI is the broadest concept, encompassing rule-based systems, expert systems, and data-driven approaches like ML and deep learning. ML is a subset of AI focused on systems learning from data, while deep learning, a further subset of ML, uses neural networks with multiple layers to analyze complex patterns. AI systems can range from simple to highly complex, while ML typically requires structured data, and deep learning demands vast amounts of often unstructured data and high-performance hardware like GPUs. Use cases vary, with AI being applied in chatbots and decision-making tools, ML excelling in tasks like recommendation engines and anomaly detection, and deep learning powering advanced applications like image recognition, natural language processing, and autonomous vehicles.

## Describe various types of inferencing (for example, batch, real-time).
- After the model has been trained, it is time to begin the process of using the information that a model has learned to make predictions or decisions. This is called inferencing.

**Batch**: Batch inferencing is when the computer takes a large amount of data, such as images or text, and analyzes it all at once to provide a set of results. This type of inferencing is often used for tasks like data analysis, where the speed of the decision-making process is not as crucial as the accuracy of the results.

**Real-time**: Real-time inferencing is when the computer has to make decisions quickly, in response to new information as it comes in. This is important for applications where immediate decision-making is critical, such as in chatbots or self-driving cars. The computer has to process the incoming data and make a decision almost instantaneously, without taking the time to analyze a large dataset.  

## Describe the different types of data in AI models (for example, labeled and unlabeled, tabular, time-series, image, text, structured and unstructured).
**Labeled Data**: Labeled data is a dataset where each instance or example is accompanied by a label or target variable that represents the desired output or classification. These labels are typically provided by human experts or obtained through a reliable process.
- Example: In an image classification task, labeled data would consist of images along with their corresponding class labels (for example, cat, dog, car).  

**Unlabeled Data**: Unlabeled data is a dataset where the instances or examples do not have any associated labels or target variables. The data consists only of input features, without any corresponding output or classification.
- Example: A collection of images without any labels or annotations

**Structured Data**: Structured data refers to data that is organized and formatted in a predefined manner, typically in the form of tables or databases with rows and columns. This type of data is suitable for traditional machine learning algorithms that require well-defined features and labels. The following are types of structured data.
- **Tabular Data**: This includes data stored in spreadsheets, databases, or CSV files, with rows representing instances and columns representing features or attributes.  
- **Time-series Data**: This type of data consists of sequences of values measured at successive points in time, such as stock prices, sensor readings, or weather data.  

**Unstructured Data**: Unstructured data is data that lacks a predefined structure or format, such as text, images, audio, and video. This type of data requires more advanced machine learning techniques to extract meaningful patterns and insights.
- **Text Data**: This includes documents, articles, social media posts, and other textual data.  
- **Image Data**: This includes digital images, photographs, and video frames.  

## Describe supervised learning, unsupervised learning, and reinforcement learning.
**Supervised Learning**: Algorithms are trained on labeled data. The goal is to learn a mapping function that can predict the output for new, unseen input data.

**Unsupervised Learning**: Algorithms that learn from unlabeled data. The goal is to discover inherent patterns, structures, or relationships within the input data.

**Reinforcement Learning**: The machine is given only a performance score as guidance and semi-supervised learning, where only a portion of training data is labeled. Feedback is provided in the form of rewards or penalties for its actions, and the machine learns from this feedback to improve its decision-making over time.