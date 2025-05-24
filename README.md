# RNN_PhishingSiteDetection
We are in the era where humans are evolving with technology. Each and every work which is used to done manually is digitalizing. From the booking of train and flights, to the using phone for online payments. Multiple manual operations which are required human to insert the record have transferred to digital platform by using computer, smartphones and internet. But with evolving technology the risk of cyber attack also evolving. And in today’s world most common cyber attack to steal the user information including username, passwords, bank account numbers, Digital Banking Pin is Phishing. 
Phishing attack is type of cyber-attack in which attacker pose themselves as legitimate entities using deceptive communications like email, text, etc. and trick individual to reveal victims’ sensitive information including there password, credit card details, and other personal information and creates threat to CIA. 
The project aim to develop an intelligent phishing site detection model using the machine learning based approach by implementing Recurrent Neural Network (RNN) to build the model. Which is suited for actively analyses the URLs and accurately classify as legitimate or phishing. 
The proposed system uses the RNN model to predict the results. The system uses the embeddings which are generated with the help of language modelling technique to capture the structural and contextual characteristic of each URL. Uses tokenization (domain, have_ip, have_@, length, redirection) and Mistral model from Ollama, which gives the vector embedding for training the model. 
Experimental evaluation of RNN model when combined with vector embeddings, outperform traditional algorithms in term of accuracy and predictive capability. 
This project can contribute in development of advanced cybersecurity solutions capable of classifying phishing URLs and safeguards the cyber space.
1.1 Introduction and Problem Summary
In the digital age, phishing has emerged as a major cybersecurity issue, targeting individuals and organization. Try deceptive web design and steal the crucial information of an organization or person. These web sites appear legitimate and these are crafted to trick the user. They often try to steal the username, passwords, OTP’s, credit card details and other sensitive information. Because of their dynamic and evolving nature they are able to evade the security mechanism.
The main problem which is addressed in this project is the detection and classification of phishing sites. Traditional system also use Machine Learning models, but have some drawbacks regarding accuracy because dynamic nature of URL’s. These could lead to high false positive results and slow response. So, there is requirement of new model which can help to solve this issue for traditional machine learning approach. [5]
Therefore, this project proposes a progressive way to classify the URL’s, using Recurrent Neural Network (RNN). The RNN complemented the vector embedding to learn contextual and sequential dependencies in URL’s.  
 




**Aim of project**
The aim is to developed an intelligent phishing detection system that uses Recurrent Neural Network (RNN) and vector embedding representation for analysing and accurate classification of URL’s as legitimate or phishing. 
**Objectives of the Project**
•	To collect and preprocess the dataset containing labelled data
•	Extracting the features from URL such as presence of IP address, length, domain name, etc.
•	Generate the embedded vector using language models. 
•	Compare the performance with traditional machine learning models
•	To evaluate the accuracy, precision, recall of models
**Scope of the Project**
The project is mainly focused on classification of phishing using a deep learning model of machine learning based approach. The scope include embedding of URL’s to extract the features. The study uses labelled dataset of URL’s as type either legitimate (0) or phishing (1).
The model aims to support the real time classification of URL, which helps to prevent the phishing attack. Helps to identify the sites if they are legitimate or phishing, results protection of individual or organization from phishing attacks. Leads to reduce the loss in terms of reputation and finance. 
Traditional phishing detection models are primarily based on static feature detection. These system train on labelled data, it compares the incoming URL against the dataset and predict. As traditional machine learning model like Decision Tree, Support Vector Machine(SVM) can be also used to classify the URL, but these models have less accuracy while prediction the new URL.
However, traditional machine learning models uses URL- based feature which are not sufficient for proper prediction. They typically use tokenization of URLs like domain name, presence of iframe, special characters, presence of HTTPS which is not really sufficient to draw the actual feature relationship. Result in  more False Positive outcomes.
After the feature extraction , the features are presented as input to standard machine learning classifier.As this traditional machine learning uses algorithm like Random Forest ,Decision Tree, Support Vector Machine(SVM), and many more , but dynamic nature of phishing site required more advanced technique to classify the URLs.
These models are evaluated as relatively simple, computationally lightweight. Which makes them useful for classifying the input data. 


**Feasibility Study**
**Technical Feasibility**
The implementation of this project is technically viable with the wide availability of open source deep learning framework and libraries. Python along with Keras or TensorFlow, provides support for building and training RNN model. URL dataset is publicly available which is used to train the model. Embedding techniques like Mistral language model help to convert text-based URLs into dense vector format. Which is suitable for deep learning input. (10)
Even with limited hardware support (e.g. CPU-only systems), models can be trained on optimized sequences.

**Operational Feasibility**
Operationally, the system requires minimal user interaction and can be deployed as an automated detection module. It is suitable for integration into browser extension, email filters, or security appliances. The learning-based nature of model allows it to learn to changing techniques by malicious phishing site over time, making it future-proof and scalable for large deployments.

**Vector Embedding**
For vector embedding we uses LLM (Large Language Model). Mistral LLM is used in for vectorizing the URL. Vectorizing means converting the data into numerical format(vectors) that a machine learning, or deep learning model can understand and process.

Attribute	Details
Model Name :	Mistral
Type	: Open-source Large Language Model (LLM)
License :	Apache
Version	: 2.0
ID :	f974a74358d6
Size	: 4.1 GB
Architecture :	Llama
Parameters	: 7.2 Billion
Embedding Length	: 4096


**Advantages/Unique Features**
The proposed phishing detection system, powered by a Recurrent Neural Network (RNN), offers several advantages over traditional methods:
•	Sequence Awareness: Unlike classical ML models that treat features independently, RNNs can understand the sequential structure of URLs, making them ideal for detecting obfuscated or cleverly crafted phishing links.
•	Automatic Feature Learning: The model does not rely on manual feature engineering. Instead, it learns relevant patterns directly from raw URL sequences.
•	Improved Detection Accuracy: The RNN model demonstrated better generalization to zero-day phishing URLs by recognizing suspicious patterns even in previously unseen inputs.
•	Real-time Detection: Once trained, the model can provide quick predictions with minimal computational resources, suitable for browser plugins or email gateways.
•	Scalable Architecture: The modular design allows easy integration with larger systems and supports retraining with updated datasets for continuous learning.

**Conclusion**

In this project, we developed a robust phishing site detection model with help of advanced Recurrent Neural Network (RNN) model with LSTM layers. The traditional model like Logistic Regression, Multinomial Naïve Bayes provides decent performance with relatively low computational overhead. However, their accuracy was limited due to their inability to effectively capture complex sequential patterns and contextual relationships within the input features.
In contrast, the RNN-based model significantly outperformed these classical approaches. Leveraging LSTM units, the deep learning model was able to learn temporal dependencies and intricate patterns in the dataset, especially when enriched with embedded vectors generated from the Mistral language model.
The RNN-based model achieved approximately 99% accuracy and exhibited strong precision and recall metrics across both phishing and legitimate classes. Overall, the integration of deep learning and vector embeddings has proven to be a powerful approach in enhancing phishing site detection

Kaggle. (n.d.). Phishing website datasets. Retrieved from https://www.kaggle.com/datasets/
TensorFlow: TensorFlow. (n.d.). An end-to-end open source machine learning platform. Retrieved from https://www.tensorflow.org/
Keras. (n.d.). Keras: The Python Deep Learning API. Retrieved from https://keras.io/
Ollama. (n.d.). Mistral LLM. Retrieved from https://ollama.com/library/mistral
Scikit-learn: Scikit-learn. (n.d.). Machine Learning in Python. Retrieved from https://scikit-learn.org

