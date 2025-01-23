## Recognize applications where AI/ML can provide value (for example, assist human decision making, solution scalability, automation).
**Assist Human Decision-Making**: AI/ML models analyze large datasets, identify patterns, and provide actionable insights, enhancing decision-making in fields like healthcare, finance, and supply chain management.

**Solution Scalability**: ML algorithms enable businesses to scale solutions rapidly, such as processing vast amounts of data or managing dynamic customer interactions in real-time.

**Automation**: AI/ML automates repetitive and time-intensive tasks, such as data entry, quality control, and customer service, improving efficiency and reducing errors.

**Predictive Analytics**: Forecasting trends, behaviors, or outcomes based on historical data, useful in marketing, demand planning, and risk management.

**Personalization**: Tailoring products, content, or services to individual user preferences, such as in e-commerce, streaming platforms, and online learning.

**Operational Efficiency**: Optimizing resource allocation, maintenance schedules, and logistics through AI-driven recommendations.

**Enhanced User Experience**: Improving interactions through AI-powered features like chatbots, voice recognition, and recommendation engines.

## Determine when AI/ML solutions are not appropriate (for example, cost-benefit analyses, situations when a specific outcome is needed instead of a prediction).
You do not need ML if you can determine a target value using simple rules, computations, or predetermined steps. You can program the steps without needing any data-driven learning. 

## Select the appropriate ML techniques for specific use cases (for example, regression, classification, clustering).
**Classification** is a supervised learning technique used to assign labels or categories to new, unseen data instances based on a trained model. The model is trained on a labeled dataset, where each instance is already assigned to a known class or category. The goal of classification is to learn patterns from the training data and use them to predict the class or category for new unlabeled data instances.  
Use cases include the following:
- Fraud detection
- Image classification
- Customer retention
- Diagnostics

**Regression** is a supervised learning technique used for predicting continuous or numerical values based on one or more input variable. It is used to model the relationship between a dependent variable (the value to be predicted) and one or more independent variables (the features or inputs used for prediction).  
Use cases include the following:
- Advertising popularity prediction
- Weather forecasting
- Market forecasting
- Estimating life expectancy
- Population growth prediction

**Clustering**: A common subcategory of unsupervised learning is clustering. This kind of algorithm groups data into different clusters based on similar features or distances between the data point to better understand the attributes of a specific cluster.  
For example, by analyzing customer purchasing habits, an unsupervised algorithm can identify a company as being large or small.  
Use cases include the following: 
- Customer segmentation
- Targeted marketing
- Recommended systems

**Dimensionality reduction** is an unsupervised learning technique used to reduce the number of features or dimensions in a dataset while preserving the most important information or patterns.  
Use cases include the following:
- Big data visualization
- Meaningful compression
- Structure discovery
- Feature elicitation

## Identify examples of real-world AI applications (for example, computer vision, NLP, speech recognition, recommendation systems, fraud detection, forecasting).
**Computer vision**:
- Autonomous Driving to make self-driving cars safer and more reliable.
- Healthcare or Medical Imaging can improve the accuracy and speed of medical diagnoses.
- Public Safety and Home Security  can swiftly identify unlawful entries or persons of interest, which fosters safer communities and works as a crime deterrent. 

**Natural language processing**:
- Insurance companies can use NLP to extract policy numbers, expiration dates, and other personal information.
- Telecommunication companies use NLP to analyze customer text messages and suggest personalized recommendations.
- In the education industry, students use Q&A chatbots to address questions.

**Intelligent document processing**:
- Financial services use IDP to extract important information from mortgage applications to accelerate customer response time. It also helps with the underwriting process by identifying incomplete loan packages, tax forms, pay stubs, and other missing data.
- IDP, along with other applications such as optical character recognition (OCR) and NLP, helps eliminate the manual effort of processing documents such as contractual documents, agreements, court filings, and legal dockets.
- Using IDP in healthcare can help expedite business quickly and accurately by processing various document types, such as claims and doctor’s notes. 

**Fraud detection**:
- Financial services use fraud detection for identity verification, payment fraud detection, transaction surveillance, and anti-money laundering (AML) sanctions.
- Fraud detection systems in the retail industry protect businesses from financial losses, safeguard customer accounts and data, and maintain trust and confidence in online transactions.


## Explain the capabilities of AWS managed AI/ML services (for example, SageMaker, Amazon Transcribe, Amazon Translate, Amazon Comprehend, Amazon Lex, Amazon Polly).
**Amazon SageMaker**: With SageMaker, you can build, train, and deploy ML models for any use case with fully managed infrastructure, tools, and workflows. SageMaker removes the heavy lifting from each step of the ML process to make it easier to develop high-quality models. SageMaker provides all the components used for ML in a single toolset, so models get to production faster with much less effort and at lower cost.

**Amazon Comprehend**: Amazon Comprehend uses ML and natural language processing (NLP) to help you uncover the insights and relationships in your unstructured data. This service performs the following functions:
- Identifies the language of the text  
- Extracts key phrases, places, people, brands, or events  
- Understands how positive or negative the text is  
- Analyzes text using tokenization and parts of speech  
- And automatically organizes a collection of text files by topic

**Amazon Translate**: Amazon Translate is a neural machine translation service that delivers fast, high-quality, and affordable language translation. Neural machine translation is a form of language translation automation that uses deep learning models to deliver more accurate and more natural-sounding translation than traditional statistical and rule-based translation algorithms. With Amazon Translate, you can localize content such as websites and applications for your diverse users, translate large volumes of text for analysis, and efficiently implement cross-lingual communication between users.

**Amazon Textract**: Amazon Textract is a service that automatically extracts text and data from scanned documents. Amazon Textract goes beyond optical character recognition (OCR) to also identify the contents of fields in forms and information stored in tables.

**Amazon Lex**: Amazon Lex is a fully managed AI service to design, build, test, and deploy conversational interfaces into any application using voice and text. Amazon Lex provides the advanced deep learning functionalities of automatic speech recognition (ASR) for converting speech to text, and natural language understanding (NLU) to recognize the intent of the text. This permits you to build applications with highly engaging user experiences and lifelike conversational interactions, and create new categories of products. With Amazon Lex, the same deep learning technologies that power Amazon Alexa are now available to any developer. You can efficiently build sophisticated, natural-language conversational bots and voice-enabled interactive voice response (IVR) systems.

**Amazon Polly**: Amazon Polly is a service that turns text into lifelike speech. Amazon Polly lets you create applications that talk, so you can build entirely new categories of speech-enabled products. Amazon Polly is an AI service that uses advanced deep learning technologies to synthesize speech that sounds like a human voice. Amazon Polly includes a wide selection of lifelike voices spread across dozens of languages, so you can select the ideal voice and build speech-enabled applications that work in many different countries.

**Amazon Transcribe**: Amazon Transcribe is an automatic speech recognition (ASR) service for automatically converting speech to text. The service can transcribe audio files stored in common formats, like WAV and MP3, with time stamps for every word so that you can quickly locate the audio in the original source by searching for the text. You can also send a live audio stream to Amazon Transcribe and receive a stream of transcripts in real time. Amazon Transcribe is designed to handle a wide range of speech and acoustic characteristics, including variations in volume, pitch, and speaking rate. Customers can use Amazon Transcribe for a variety of business applications, including the following:
- Transcription of voice-based customer service calls  
- Generation of subtitles on audio and video content  
- Conducting (text based) content analysis on audio and video content

**Amazon Rekognition**: Amazon Rekognition facilitates adding image and video analysis to your applications. It uses proven, highly scalable, deep learning technology that requires no ML expertise to use. With Amazon Rekognition, you can identify objects, people, text, scenes, and activities in images and videos, and even detect inappropriate content. Amazon Rekognition also provides highly accurate facial analysis and facial search capabilities. You can use it to detect, analyze, and compare faces for a wide variety of user verification, people counting, and public safety use cases.

**Amazon Kendra**: Amazon Kendra is an intelligent search service powered by ML. Amazon Kendra reimagines enterprise search for your websites and applications. Your employees and customers can conveniently find the content that they are looking for, even when it’s scattered across multiple locations and content repositories within your organization.

**Amazon Personalize**: Amazon Personalize is an ML service that developers can use to create individualized recommendations for customers who use their applications.  
With Amazon Personalize, you provide an activity stream from your application (page views, signups, purchases, and so forth). You also provide an inventory of the items that you want to recommend, such as articles, products, videos, or music. You can choose to provide Amazon Personalize with additional demographic information from your users, such as age or geographic location. Amazon Personalize processes and examines the data, identifies what is meaningful, selects the right algorithms, and trains and optimizes a personalization model that is customized for your data.  