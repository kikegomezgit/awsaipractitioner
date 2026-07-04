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
Bedrock -> Managed service for Generative AI for models-> 
Sagemaker(any kind of AI except generative) -> custom LLM and training ->
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


















To dos before monday

Agno - playbook simple of tickets, orders and customerdbs
front- move to advanced the force only consult on








