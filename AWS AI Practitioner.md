AWS Certified AI Practitioner (AIF-C01)

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
Aws Bedrock -> Managed service for Generative AI for models and hosting-> Guardrails to filter inappropiate content
Aws Sagemaker(any kind of AI except generative) -> custom LLM and training -> clarify(detect bias and disparities)explainability
 automated resource management, algorithm and framework support, data wrangler(clean and balance data to prevent bias, data augmentation)
import data->clean data->augment data->export data


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
Aws Aurora and Aws RDS for postgresql pgvector
Aws Neptune ML->Graph neural networks(GNNs) enhance predictions using complex graph relationships
Aws A21-> human review of AI predictions->handling low-confidence inferences and randoms audits



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
ROUGE(recall-oriented understudy for gisting evaluation)->evaluates summarization quality
BLEU(bilingual evaluation understudy)-> assesses machine transalation
GLUE(General language understanding evaluation)->natural language tasks for model evaluation, tasks include sentiment analysis, question answering and more
superGLUE->multi
MMLU(massive multitask language understanding)->evaluates models knowledge and problem-solving ability across multiple subjects
Big-bench(beyond the imitation game benchmark)->focus on tasks beyond current LLM capabilities, tasks includes math, biology,reasoning, software development and bias detection
HELM(holistic evaluation of language models)->improving model transparency, evaluates tasks such summarization, question answering,sentiment analysis and bias detection
kinds of models-> VAES[unsupervised learning], GANS[generating images], Autoregressive models[sequential tasks]
AI metrics->Accuracy-efficiency-conversion rate

Training techniques--
to reduce bias-> data autmentation, fariness tools
Ethical AI
inside Foundational model ----
Inference Parameters---
Temperature->lower predictable and focused, higher diverse and more creative
Top-K-> 5-fewer words, -50 wider range of words
Top-P->limits word choice to more certain options, expands word choices to include more possibilities adding creativity
-----------------------------------
In context Learning




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

vector databases store data as embeddings, wich are numerical representations of data like text and images to be searched on a semantic search
search strategies -> k-nearest neighbors (k-NN) for efficient vector queries
Storing Techniques---------
Graph DB = Relationships
Vector DB = Meaning

Store things that need semantic search:
Ticket descriptions
Comments
Logs
Stack traces
Documentation
Runbooks

Example:
Ticket:
"Checkout timeout after deployment"
Embedding
↓
Finds
"Checkout API hangs after release"
even though the wording is different.

Multi-step tasks-----------------------------------------

** Agent[single narrow-broad expertise][orchestrate](agno,langchain) ->uses Foundational model(gpt-5-mini)->that uses RAG(tickets,wikis-all vectorized),MCPs(general purpose functions)
Agno(self-managed decitions)
Langchain(workflows defined A → B → C → D)
                    User
                      │
                      ▼
        Agent (Agno / LangGraph)
      (orchestration + memory + state)
                      │
      ┌───────────────┼────────────────┐
      │               │                │
      ▼               ▼                ▼
 Foundation LLM      RAG             MCP Tools
 (GPT-5 Mini)   (Knowledge)      (Functions/APIs)
      │               │                │
      │         Tickets              SQL
      │         Wikis                OMS
      │         SOPs                 Cart Services
      │         Docs                 Payments
      │         FAQs                 Inventory
      │
      └───────────────┬────────────────┘
                      ▼
              Final Response



** prompting----

task/instruction-> write a product description for a ...
context-> focus on ...
negative prompt-> do not include..

model latent space-> stores the knowledge a model learns during training

zero-shot prompting->prompt
few-shot prompting->prompt + examples
chain of thought prompting->breaks down reasoning processes into intermmediate steps(transparency and explainability)
prompt templates->predefined instructions(skills)

prompt-tuning->fine-tunes the model by optimizing the prompt continuous embedding during training


Guardrails in Prompt Engineering----
block specific words
threshold for filtering harmful content
protect against prompt injections

Fine-Tuning----
improves model performance for specific tasks
balance fine-tuning between tasks
fine-tuning->task-specific learning with labeled examples
pre-training->general-purpose learning from unstructured data
Parameter-Efficient Fine-Tuning (PEFT)--
Freeze most parameters
Fine-tune small layers
Techniques : 
LoRA(Low-Rank Adaptation)->Freezes original weights except for low-rank weights, adds trainable low-rank matrices
ReFT(Rpresentation Fine-tuning)->modified model representations rather than weights
multi-task-fine tuning
Domain-Specific Fine-tuning
**Reinforcement learning from human feedback(RLHF)
https://drive.google.com/file/d/1mFFGOc1cWyQ469kVjUx-wiQ6fJvNcL_V/view?usp=drive_link

Data privacy and security risks
PII data sensitive information may appear in model outputs unintentionally



Evualuating Foundation Model Performance ----


Legal risks in gen ai------
Offensive and inappropiate AI outputs
content guardrails



**Responsible AI------
Fairness-> bias, where a data has a distinct group but shouldnt look at it
Explainability->why the decition
Robustness->handle unexpected circumstances without crashing or hallucinating
Privacy and security->protect user data and prevent exposure of personally identifiable information (PII)
Governance->meeting industry standards and legal compliance requirements, risk stimation and mitigation
Transparency->provide clear information about capabilities and risks
Address bias and variance->demographic disparities and unqeual treatments


**Data curation for balanced datasets----
labeling-cleaning-augmenting-balancing
choose relevant informormation for training
periodically check datasets for bias
ensure ongoing fairness and accountability

interpretability->simple models with clear rules
explainability->complex models viewed as black boxes
open-source AI - Enhancing Transparency projects->transparency and safety
partial dependence plots


Human-Centered Design(HCD)- Importance


IAM Policies and Permissions------
policies define permissions for resources
JSON-based, enabling least privilege access
root access has access to all resources
IAM Groups for efficient permission management-> create multiple groups with shared policies
on Sagemaker role manager for ml permissions groups -> data scientist, MLops and Compute
on a Load balancer can be set up to encrypt/decrypt https request with TLS
all AWS service endpoints supports TLS for secure https connections
Virtual Private Cloud(VPC)->allow to make endpoints private travel throught a private subnet
enhanced security by controlling network traffic with security groups,network access lists and firewalls

Aws CloudTrail->Activity Logging and auditing
Aws Key management service(KMS)->manage encryption keys tls tsl
Aws PrivateLink


Machine LEarning - Need for tracking artifacts------

Source codes
datasets
container images
model versions for reproducibility
sagemaker model registry for model versioning includes metrics and hyperparameters
Sagemaker Model Cards->Intended uses, risk assessments, training details, evaluation Results[compliance and transparency]
Sagemaker Lineage-> tracking of the lineage of the machine learning workflow
Sagemaker Feature Store->centralized store for reeusable ML features


**Secure data Engineering---------------
network security configuration
access control implementation
data privacy assurance
data integrity verification

Aws Virtual Private Cloud
Aws Macie-> Notifies users of detected PII in data sources, enabling propmt removal and improving data privacy
Aws Sagemaker

vpc-> private/public subnet->network access control list-> security group instance
VPC-Only mode for Sagemaker->restric all network traffic to the vpc, prevents access to public endpoints, enhances security by using private connections for resources

Remove PII during training 
Assessing data quality->accuracy-completeness-relevance
data cleaning and preprocessing->removing errors-handling missing values-formatting data

least-privilege permissions

AI Security-------------
Data poisoning->manipulated data
model inversion and reverse engineering threats->attackers can infer training data by repeatedly queryng the model and reverse engineering creates a model with similar behaviour
prompt injection
model monitor->detect performance drift to identify potential attacks or data quality issues(this can be done with Aws Cloudwatch)



tickets
codigo
logs

- ------------------------------------------------------------------------------------------------------------------------

To dos identify must haves / nice to haves to accomplish a Goal, and who is the target user?(Support L2 and Devs)
consultation then execute actions(modify)
support L2 only consult , Devs can consult and execute

cart services and payments mcp actions/functions
decision_guide.json and business_glossary.json





generate knowledges md from code sources agents and implement OKF
instaleap, oms, vtex
subscriptions


security and error handling

DEV keys on all and azure PAT and board

bugs terminology on organization means something different because they are attached to a parent HU, we need to create a new "issue" card

playbook simple of tickets, orders and customerdbs

Check how can i use the large datasets we have on DWH on ecommerce for training

check how to access comme logs on an efficient way

In context Learning

Subscriptions knowledge search to then investigate logs(ftp)

Session in prompting

Safety and Responsible use of data ISO

documentar palabras clave busqueda para guardar solucion de un ticket : resolucion o solucion

Add Role-based-permission to execute x actions(devs only can execute modify) on Agno and mcp server being fed by front the role and jwt
{
  "tool": "refund_order",
  "required_roles": [
    "manager",
    "admin"
  ]
}

explore minimax on foundry throught fireworks AI 
https://azure.microsoft.com/en-us/pricing/details/ai-foundry-models/aoai/

That means if you invoke MiniMax through Microsoft AI Foundry Serverless, your data is handled under Azure's data processing commitments rather than being sent directly to MiniMax's own cloud.
If Microsoft states that prompts are not shared with the publisher, that significantly reduces one of the common enterprise concerns.
From a procurement and governance perspective:
Some organizations have policies that prohibit or restrict the use of AI models developed by companies headquartered in certain countries, regardless of where inference is hosted.
Others permit them after a security and legal review.
Many private companies focus on Microsoft's contractual guarantees rather than the model developer's country of origin.


logs comme a 
Option 1: The Open-Source Way – Grafana Loki (Recommended)(Azure blob storage)
Option 2: Azure table storage(2 index)