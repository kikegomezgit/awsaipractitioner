AWS AI Practitioner

Concepts

Artificial Intelligence -> sense, reason, act, and adapt

Visual perception, speech recognition, decision-making, language translation



Machine Learning -> Algorithm whose performance improve as they are exposed to more data over time

Custom LLM models

Statistical models

Training data. Patterns and predictions

	Rule-based-> straightforward conditions
	Ml-systems-> probability, patterns

Predictions,forecast ->ml

Development lifecycle of a ML

Business Goal->define whats the purpose because this is a measured objective

Data collection and preparation->
https://drive.google.com/file/d/1vKAJFId84FIb-fdcI0-F5tYsAOzdrbW4/view?usp=drive_link

data storage(s3,rds)->aws glue(preprocessing-transform)->sagemaker(ML)
Data augmentation->Artificially increase dataset size through transformations(best for image recognition)
splitting data for training,validation and testing
80(train) 10(testing and tune) 10(testing pre prod)


training->
hyperparameter tuning -> automatic model tuning (amt)-> auto optimize models by running multiple training jobs
evualuating model performance(different way to measure)
accuracy - precision - recall - F1 Score

deployment-monitoring
real-time and batch
Evaluating ML models - Confusion Matrix -> predicted vs results -> accuracy, precision and recall

precision -> measures correct positive predictions; minimizes false positives
recall -> captures actual positives; vital for medical diagnoses
F1 Score -> Balances precision and recall; useful for false positive/negative trade-offs

https://drive.google.com/file/d/1yr8KdzII2U_voVtA5MwqBcFH6CvzW7Sc/view?usp=drive_link
AUC -> Area under curve for binary classification
ranges from 0.5 to 1(perfect prediciton)
Mean Squared Error(MSE) in Regression models





Deep Learning ->Subset of ML in which multi-layered neural networks learn from a vast amount of data

Neural networks
	input layer -> hidden layers -> output layer


Inference -> reasoning and creating a truth based on this
	types: 	real-time inferencing(sagemaker)
			batch inferencing -> bulk process on scheduled intervals(sagemaker)


Artificial Narrow Intelligence (ANI) -> limited AI for specific tasks


Data types
	numerical -> quantitive 0 and 1 , can be sorted ask and desc
	categorical -> categories or groupings (gender, product type, regions)
	text
	Audio data
	images -> preprocessing(resizing, normalization, augmentation)->AI model -> output
	unstructured data -> images, videos 


	labeled data -> supervised learning ->confirms the inference (classification and regression)
	unlabeled data -> unsupervised learning -> doesn’t confirms the inference(anomaly detection and grouping)->model finds patterns in unlabeled data
	reinforcement learning -> Model learns through trial and error by receiving rewards or penalties
	time-series data -> data over certain times->long short-term memory networks(lists), arima
	imbalanced data -> oversampling-undersampling ->roc-auc(helps mitigates this)
	handling missing data-> algorithms to fill like the average of current data imputation technique used mean and median

Rule of thumb : supervised learning(structured data) , unsupervised learning(unstructured data)
Decision trees
CNN’s
RNN’s


Big data and ai -> large and complex datasets that require advanced tools for processing-> used for deeper insights, tran better models and predict trends

One-hot Encoding	 -> allows you to convert categorical to numerical
NLP ->natural language processing
Preprocessing->cleaning, encoding, scaling	

Generative AI
Foundation Models
Security,Compliance and governance



IAS MLOPS
https://drive.google.com/file/d/1QPmQDQ_uVTEUW70j-VumlvEN5s7NIJJ2/view?usp=drive_link

Compliance and Auditability in MLOPS
documented and versioned ML lifecycle steps
tracks model training, data usage, and deployment
Supports regulated industries like healthcare and finance
Demonstrates compliance with regulations






Aws services------------------
AWS CloudFormation === Terraform(IAS)
Aws Bedrock -> Managed service for Generative AI for models and hosting-> 
Aws Sagemaker(any kind of AI except generative) -> custom LLM and training ->
 automated resource management, algorithm and framework support
hyperparameter tuning -> automatic model tuning (amt)-> auto optimize models by running multiple training jobs
built in tools evaluate models and track performance against business metrics
monitor throught model monitor and amazon cloudwatch
logs and audits the model training and deployment process
monitors fairness and bias, ensuring models are accurate
MLOPS inside sagemaker, can be orchestrated with apache airflow
Model versioning(as a code) with model registry
Automates retraining as new data comes in
define threshold
with Clarify monitors fariness and bias 

Amazon Rekognition->image and video preprocess
AWS Comprehend-> raw text -> tokenization, stop word removal -> NLP model -> sentiment analysis and text classification
Aws transcribe -> speech to text service
Aws Prophet
Aws Athena -> like presto, query data from multiple sources
Aws Elastic MapReduce(EMR) -> 
Aws Transcribe -> Speech to text(stt)
Aws Textract -> extract text from a document like pdf
Aws Polly->vocalize(TTS)
Aws Lex -> Pre-trained model to enable quick Ai integration(virtual assistants-conversational framework)(natural language understanding NLU and ASR automatic speech recognition)
Aws Glue(preprocessing-transform) ->Databrew(data visualization and transformation with recipes)
Aws Augmented AI(AAI) -> Built in Human Review workflows
AWS Quicksight -> graphs from data and analysis for interactive dashboards -> SPICE(super fast, parallel, in memory calculation engine)
Azure Machine Learning === sagemaker
Aws Titan-> aws house model
Aws PartyRock -> Amazon Bedrock Playground for generative AI
Aws Amazon Q-> Advanced querying with AI
Aws Inferentia->optimized for ML. faster inference performance with lower latency
Aws Trainium->training machine learning models
Aws kendra -> Vector database semantic search
Aws OpenSearch -> managed service for vector databases


On demand vs reserved instances
Artificial intelligence -> Learns from data then make predictions
Generative AI->Creates new solutions(code,text,images) based on learned data


General AI concepts ---
Context windows -> memory span available when its generating text and portion of input data that a model process at time
transformer network-> neural network arch to process input in parallel
tokens-> smallest unit of data(words)
tokenization->process of breaking down input to tokens
Embedding-> numeric representations of words or phrases that capture their meaning
Vectors->Ordered lists of numbers that represent data features
Chunking->Used to handle large amounts of data by breaking it down into smaller, more manageable pieces called chunks, important to choose the right chunk size for precision 
LLMS(Large language models) -> generative AI models trained
Prompt-> input given to the model
techniques:
	Zero-shot learning-> no data trained
	One-Shot learning->one example
	few-shot learning-> learn from few examples and can recognize new instances
multimodal models-> can handle videos,text,images
diffusion models->can only handle images,audio,video

behind Generative AI
GAN->generative adversarial network
VAE->variational autoencoder
transformers

Foundational Model{GPT-4}
fine-tuning-> identify recurring tasks-gather preferences-understand business needs
ROUGE->evaluates summarization quality
BLEU-> assesses transalation
kinds of models-> VAES[unsupervised learning], GANS[generating images], Autoregressive models[sequential tasks]
AI metrics->Accuracy-efficiency-conversion rate

Training techniques--
to reduce bias-> data autmentation, fariness tools
Ethical AI

Inference Parameters---
Temperature->lower predictable and focused, higher diverse and more creative
Top-K-> 5-fewer words, -50 wider range of words
Top-P->limits word choice to more certain options, expands word choices to include more possibilities adding creativity


Python ML frameworks->
Tensorflow Hub, Pytorch Hub, Hugghing face
Interpretability-> Simple models like linear regression
--important to understand thinking ->Explainability->Methods for understanding complex models--
LIME
SHAP->https://shap.readthedocs.io/en/latest/example_notebooks/overviews/An%20introduction%20to%20explainable%20AI%20with%20Shapley%20values.html

Real time decision-making -> KNN Model
Modal->Type of input data a model can process
architecture of a model
CNN(convolutional neural networks)->Image recognition
RNN(Recurrent neural networks)-> natural language processing tasks
Performance metrics
Accuracy - Precision(consistent) - Recall(false positives and false positives) - F1 Score

vector databases store data as embeddings, wich are numerical representations of data like text and images



To dos before monday

Agno - 
* check differences with gpt-5.4-nano vs gpt-5.4-mini on performance on fine-tunning
playbook simple of tickets, orders and customerdbs








