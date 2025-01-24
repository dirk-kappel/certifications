**self-supervised learning** 
- It works when models are provided vast amounts of raw, almost entirely, or completely unlabeled data and then generate the labels themselves.
- Foundation models use self-supervised learning to create labels from input data. In self-supervised learning, models are provided vast amounts of raw completely unlabeled data and then the models generate the labels themselves. This means no one has instructed or trained the model with labeled training data sets.

**underfit**  
- Underfitting occurs when a model is too simplistic to capture the underlying patterns in the data, resulting in poor performance on both the training data and new data.
- Your model is underfitting the training data when the model performs poorly on the training data. This is because the model is unable to capture the relationship between the input examples (often called X) and the target values (often called Y).   
- Underfit models experience high bias — they give inaccurate results for both the training data and test set. More model training results in less bias but variance can increase. Data scientists aim to find the sweet spot between underfitting and overfitting when fitting a model. A well-fitted model can quickly establish the dominant trend for seen and unseen data sets.

**overfit**
- Overfitting happens when a model learns the training data too well, including noise and outliers, leading to excellent performance on the training data but poor generalization to new, unseen data.
- Your model is overfitting your training data when you see that the model performs well on the training data but does not perform well on the evaluation data. This is because the model is memorizing the data it has seen and is unable to generalize to unseen examples.
- Overfit models experience high variance - they give accurate results for the training set but not for the test set.

**Amazon SageMaker Ground Truth**
- Offers the most comprehensive set of human-in-the-loop capabilities, allowing you to harness the power of human feedback across the ML lifecycle to improve the accuracy and relevancy of models. You can complete a variety of human-in-the-loop tasks with SageMaker Ground Truth, from data generation and annotation to model review, customization, and evaluation, either through a self-service or an AWS-managed offering.

**SageMaker Data Wrangler**
- Supports tabular, time-series, and image data, offering 300+ pre-configured data transformations to prepare these different data modalities. For customers wanting to prepare text data in Data Wrangler for NLP use cases, Data Wrangler supports the NLTK library so that customers can prepare text data by authoring their custom transformations in Data Wrangler.

**Model Customization**
- You can use a customized model only in the Provisioned Throughput mode
- With the Provisioned Throughput mode, you can purchase model units for a specific base or custom model. The Provisioned Throughput mode is primarily designed for large consistent inference workloads that need guaranteed throughput. Custom models can only be accessed using Provisioned Throughput.

**Amazon SageMaker Clarify**
- Amazon SageMaker Clarify is a service provided by AWS (Amazon Web Services) that helps developers detect biases and explain the predictions made by machine learning models. It is part of the Amazon SageMaker suite of machine learning tools and focuses on enhancing transparency, fairness, and explainability in machine learning workflows.

**Amazon SageMaker Model Monitor**
- Amazon SageMaker Model Monitor is a service within the Amazon SageMaker suite that helps developers continuously monitor machine learning models deployed in production. It ensures that models maintain optimal performance and make accurate predictions over time by detecting data quality issues, concept drift, and other anomalies. Amazon SageMaker Model Monitor automatically detects and alerts you to inaccurate predictions from deployed models.

**Amazon Q** 
- Amazon Q is a generative AI–powered assistant for accelerating software development and leveraging companies' internal data. Amazon Q generates code, tests, and debugs. It has multistep planning and reasoning capabilities that can transform and implement new code generated from developer requests.

**AWS Trainium** 
- AWS Trainium is the machine learning (ML) chip that AWS purpose-built for deep learning (DL) training of 100B+ parameter models. Each Amazon Elastic Compute Cloud (Amazon EC2) Trn1 instance deploys up to 16 Trainium accelerators to deliver a high-performance, low-cost solution for DL training in the cloud.

**AWS Inferentia** 
- AWS Inferentia is an ML chip purpose-built by AWS to deliver high-performance inference at a low cost. AWS Inferentia accelerators are designed by AWS to deliver high performance at the lowest cost in Amazon EC2 for your deep learning (DL) and generative AI inference applications.

**MLflow with Amazon SageMaker**
- Track, organize, view, analyze, and compare iterative ML experimentation to gain comparative insights and register and deploy your best-performing models.

**Supervised Learning**
- Logistic Regression
- Linear Regression
- Decision Tree
- Neural Network

**Document classification** 
- This is an example of semi-supervised learning. Semi-supervised learning is when you apply both supervised and unsupervised learning techniques to a common problem. This technique relies on using a small amount of labeled data and a large amount of unlabeled data to train systems. When applying categories to a large document base, there may be too many documents to physically label. For example, these could be countless reports, transcripts, or specifications. Training on the unlabeled data helps identify similar documents for labeling.

**Association rule learning** 
- This is an example of unsupervised learning. Association rule learning techniques uncover rule-based relationships between inputs in a dataset. For example, the Apriori algorithm conducts market basket analysis to identify rules like coffee and milk often being purchased together.

**Few-shot Prompting**
- Few-shots prompting involves providing the model with examples that include both the user-input and the correct user intent. These examples help the model understand and learn how to map various user queries to their appropriate intents. By repeatedly seeing this pairing, the model can generalize from these examples and improve its ability to recognize user intent in new, unseen queries.

**Top K**
- Top K represents the number of most likely candidates that the model considers for the next token. Choose a lower value to decrease the size of the pool and limit the options to more likely outputs. Choose a higher value to increase the size of the pool and allow the model to consider less likely outputs.

**Top P** 
- Top P represents the percentage of most likely candidates that the model considers for the next token. Choose a lower value to decrease the size of the pool and limit the options to more likely outputs. Choose a higher value to increase the size of the pool and allow the model to consider less likely outputs.

**Stop sequences** 
- Stop sequences specify the sequences of characters that stop the model from generating further tokens. If the model generates a stop sequence that you specify, it will stop generating after that sequence.

**Hyperparameter tuning**
- Adjusts the settings that control the learning process of the model. By fine-tuning hyperparameters, such as increasing regularization or early stopping or adjusting dropout rates, the model can avoid overfitting to the training data and better generalize to new, unseen data in production. This approach helps improve the model's performance across various data distributions.

### Why does overfitting occur?
You only get accurate predictions if the machine learning model generalizes to all types of data within its domain. Overfitting occurs when the model cannot generalize and fits too closely to the training dataset instead. Overfitting happens due to several reasons, such as:
- The training data size is too small and does not contain enough data samples to accurately represent all possible input data values.
- The training data contains large amounts of irrelevant information, called noisy data.
- The model trains for too long on a single sample set of data.
- The model complexity is high, so it learns the noise within the training data.

### How can you prevent overfitting?
You can prevent overfitting by diversifying and scaling your training data set or using some other data science strategies, like those given below.
- **Early stopping**: Early stopping pauses the training phase before the machine learning model learns the noise in the data. However, getting the timing right is important; else the model will still not give accurate results.
- **Pruning**: You might identify several features or parameters that impact the final prediction when you build a model. Feature selection—or pruning—identifies the most important features within the training set and eliminates irrelevant ones. For example, to predict if an image is an animal or human, you can look at various input parameters like face shape, ear position, body structure, etc. You may prioritize face shape and ignore the shape of the eyes.
- **Regularization**: Regularization is a collection of training/optimization techniques that seek to reduce overfitting. These methods try to eliminate those factors that do not impact the prediction outcomes by grading features based on importance. For example, mathematical calculations apply a penalty value to features with minimal impact. Consider a statistical model attempting to predict the housing prices of a city in 20 years. Regularization would give a lower penalty value to features like population growth and average annual income but a higher penalty value to the average annual temperature of the city.
- **Ensembling**: Ensembling combines predictions from several separate machine learning algorithms. Some models are called weak learners because their results are often inaccurate. Ensemble methods combine all the weak learners to get more accurate results. They use multiple models to analyze sample data and pick the most accurate outcomes. The two main ensemble methods are bagging and boosting. Boosting trains different machine learning models one after another to get the final result, while bagging trains them in parallel.
- **Data augmentation**: Data augmentation is a machine learning technique that changes the sample data slightly every time the model processes it. You can do this by changing the input data in small ways. When done in moderation, data augmentation makes the training sets appear unique to the model and prevents the model from learning their characteristics. For example, applying transformations such as translation, flipping, and rotation to input images.


**Shapley values**
- Local interpretability method that explains individual predictions by assigning each feature a contribution score based on its marginal effect on the prediction. This method is useful for understanding the impact of each feature on a specific instance's prediction.

**Partial Dependence Plots (PDP)**
- Provides a global view of the model’s behavior by illustrating how the predicted outcome changes as a single feature is varied across its range, holding all other features constant. PDPs help understand the overall relationship between a feature and the model output across the entire dataset.

**Exploratory Data Analysis (EDA)**
- Examining the data through statistical summaries and visualizations to identify patterns, detect anomalies, and form hypotheses. This phase is crucial for understanding the dataset’s structure and characteristics. Tasks like calculating statistics and visualizing data are fundamental to EDA, helping to uncover patterns, detect outliers, and gain insights into the data before any modeling is done. EDA serves as the foundation for building predictive models by providing a deep understanding of the data.

**Data Preparation** 
- Data preparation involves cleaning and preprocessing the data to make it suitable for analysis or modeling. This may include handling missing values, removing duplicates, or transforming variables. 

**Data Augmentation** 
- Data augmentation is a technique used primarily in machine learning to artificially increase the size and variability of the training dataset by creating modified versions of the existing data, such as flipping images or adding noise. 

**Confusion matrix**
- Confusion matrix is a tool specifically designed to evaluate the performance of classification models by displaying the number of true positives, true negatives, false positives, and false negatives. This matrix provides a detailed breakdown of the model's performance across all classes, making it the most suitable choice for evaluating a classification model's accuracy and identifying potential areas for improvement. It provides a comprehensive overview of the model's performance by detailing how many instances were correctly or incorrectly classified in each category. This enables the company to understand where the model is performing well and where it may need adjustments, such as improving the classification of specific material types.

**Root Mean Squared Error (RMSE)** 
- Root Mean Squared Error (RMSE) is a metric commonly used to measure the average error in regression models by calculating the square root of the average squared differences between predicted and actual values.

**Mean Absolute Error (MAE)** 
- Mean Absolute Error (MAE) measures the average magnitude of errors in a set of predictions without considering their direction. MAE is typically used in regression tasks to quantify the accuracy of a continuous variable's predictions.

**Correlation matrix** 
- Correlation matrix measures the statistical correlation between different variables or features in a dataset, typically used to understand the relationships between continuous variables. A correlation matrix is not designed to evaluate the performance of a classification model.

### Hyperparameters
You can customize the hyperparameters of the training job that are used to fine-tune the model. The hyperparameters available for each fine-tunable model differ depending on the model.  
The following hyperparameters are common among models:
- **Epochs**: One epoch is one cycle through the entire dataset. Multiple intervals complete a batch, and multiple batches eventually complete an epoch. Multiple epochs are run until the accuracy of the model reaches an acceptable level, or when the error rate drops below an acceptable level.
- **Learning rate**: The amount that values should be changed between epochs. As the model is refined, its internal weights are being nudged and error rates are checked to see if the model improves. A typical learning rate is 0.1 or 0.01, where 0.01 is a much smaller adjustment and could cause the training to take a long time to converge, whereas 0.1 is much larger and can cause the training to overshoot. It is one of the primary hyperparameters that you might adjust for training your model. Note that for text models, a much smaller learning rate (5e-5 for BERT) can result in a more accurate model.
- **Batch size**: The number of records from the dataset that is to be selected for each interval to send to the GPUs for training.


**Continued pre-training**
- Continued pre-training in Amazon Bedrock enables you to teach a previously trained model on additional data similar to its original data. It enables the model to gain more general linguistic knowledge rather than focus on a single application. With continued pre-training, you can use your unlabeled datasets, or raw data, to improve the accuracy of foundation model for your domain through tweaking model parameters. For example, a healthcare company can continue to pre-train its model using medical journals, articles, and research papers to make it more knowledgeable on industry terminology.

**Fine-tuning**
- Fine-tuning is the process of taking a pre-trained FM, such as Llama 2, and further training it on a downstream task with a dataset specific to that task. The pre-trained model provides general linguistic knowledge, and fine-tuning allows it to specialize and improve performance on a particular task like text classification, question answering, or text generation. With fine-tuning, you provide labeled datasets—which are annotated with additional context—to train the model on specific tasks. You can then adapt the model parameters for the specific task based on your business context.
- You can implement fine-tuning on FMs with Amazon SageMaker JumpStart and Amazon Bedrock. 