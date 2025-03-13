# Resume-Keyword-Match-

This Python-based tool matches resumes with job descriptions using BERT embeddings and cosine similarity. It classifies resumes into four categories: -> Strong, Moderate, Bad, Poor Match. 
This tool helps job seekers optimize their resumes to align with job requirements, improving their chances of passing Applicant Tracking Systems (ATS).

Dataset: 
Contains 9,544 resumes, each with skills, experience, job position, and matched score. 
The match score (ranging from 0 to 1) determines the resume’s relevance to the job description. 
Sourced from Kaggle

Model Overview: 
Preprocessing 
Text Cleaning: Removing stopwords, special characters, and normalizing text. 
Tokenization: Converting text into tokens for BERT processing. 
TF-IDF Vectorization: Extracting important keywords from resumes and job descriptions.

Architecture: 
Keyword Extraction – Extracting relevant skills from resumes & job descriptions using NLP techniques. 
BERT Embeddings – Uses all-MiniLM-L6-v2 from Hugging Face’s sentence-transformers library to create semantic representations. 
Cosine Similarity Matching – Measures the similarity between job descriptions and resumes. 
Threshold-Based Classification: Exceptional Match (Score ≥ 0.85) Strong Match (Score 0.7 - 0.85) Moderate Match (Score 0.55 - 0.7) Weak Match (Score 0.4 - 0.55) Poor Match (Score < 0.4)

Training & Evaluation Feature Extraction – BERT sentence embeddings (all-MiniLM-L6-v2). TF-IDF Feature Extraction – Uses Term Frequency - Inverse Document Frequency. Similarity Calculation – Cosine similarity for resume-job matching. Handling Imbalanced Data – Random oversampling to balance the dataset. Threshold-Based Classification – Assigning match labels based on cosine similarity scores.

Results: 
![image](https://github.com/user-attachments/assets/d1a397f7-227a-4569-842f-8468f4c97166)

![image](https://github.com/user-attachments/assets/f59695e2-a544-4dfa-b481-da157b6d691d)

![image](https://github.com/user-attachments/assets/48622ad3-de35-4c16-9b4e-7625cc812254)





Sample Examples -> Example 1: Resume: Software engineer with 4 years of experience in Java, Spring Boot, and microservices. Job: Seeking a backend developer role requiring expertise in Java, Spring Boot, and cloud computing. Match Score: 0.6803 Classification: Moderate Match!

Example 2: Resume: Entry-level data analyst with knowledge of SQL, Excel, and basic Python. Job: Looking for a data analyst position where I can apply my skills in SQL, Python, and Tableau. Match Score: 0.7143 Classification: Strong Match!

Example 3: Resume: Mechanical engineer with experience in automotive design and CAD modeling. Job: Seeking a software development role leveraging my experience in Java, Spring Boot, and cloud computing. Match Score: 0.1822 Classification: Poor Match!

Example 4: Resume: Experienced chef skilled in Italian cuisine and pastry making. Job: Looking for opportunities to transition into blockchain development with expertise in Solidity and smart contracts. Match Score: 0.2878 Classification: Poor Match!

Example 5: Resume: AI engineer with Python, TensorFlow, and some knowledge of cloud computing. Job: Seeking a cloud engineering role where I can apply my knowledge of AWS, Docker, and basic ML concepts. Match Score: 0.5698 Classification: Moderate Match!

Example 6: Resume: Hardworking professional, good communication skills, and team player. Job: Looking for an ML engineering position focused on TensorFlow, NLP, and cloud deployment. Match Score: 0.1568 Classification: Poor Match!

Example 7: Resume: Expert in Python, machine learning, deep learning, and AI research. Job: Looking for a senior data scientist role that involves AI, ML, Python, and research-driven projects. Match Score: 0.6294 Classification: Moderate Match!

How to Run:

git clone https://github.com/Rajesh-M01/Resume-Keyword-Match-.git

Run the Jupyter Notebook (Resume Keyword Match.ipynb) in Kaggle through the link -> https://www.kaggle.com/code/rajeshm0/resume-keyword-match

Libraries Used 
Hugging Face Transformers (sentence-transformers) 
NLTK 
Scikit-learn 
Pandas 
Matplotlib & Seaborn

Key Learnings
How to match resumes with job descriptions using NLP and TF-IDF. 
Combining BERT & TF-IDF for resume-job matching. 
Understanding cosine similarity for text relevance scoring. 
Classifying resumes into Exceptional, Strong, Moderate, Weak, and Poor Matches.

Connect with Me If you liked this project, feel free to ⭐ the repository and connect with me on https://www.linkedin.com/in/rajesh-m-a42539317/ !
