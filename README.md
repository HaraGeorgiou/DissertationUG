# **AI-Enhanced Recruitment Platform for Job Matching and AI Skill Acquisition**

## **Overview**
This repository contains the source code and documentation for my dissertation project, **"Empowering the Workforce: Developing an AI-Enhanced Recruitment Platform for Job Matching and AI Skill Acquisition."** The project aims to improve job-role matching and AI skill acquisition using **Natural Language Processing (NLP)** and **machine learning models**.

## **Project Motivation**
Traditional recruitment methods often fail to align job descriptions with actual job requirements, leading to inefficiencies. This project addresses these challenges by leveraging **Sentence Transformers** to enhance the precision of job-role matching. The platform also integrates AI-driven **skill recommendations** to assist job seekers in bridging competency gaps.

## **Key Features**
- **AI-Powered Job Matching:** Uses **Sentence Transformers** and **cosine similarity** to match job descriptions with UK occupational standards.
- **AI Skill Recommendation:** Integrates with **Claude (LLM by Anthropic)** to provide skill improvement suggestions.
- **Ethical AI Implementation:** Ensures fairness in hiring decisions using the **AREA framework**.
- **User-Friendly Web Interface:** Built using **Flask, HTML, and CSS** for seamless interaction.

## **Project Structure**
```
📂 ai-recruitment-platform
│── 📂 data                 # Processed job descriptions & occupational standards
│── 📂 models               # Trained NLP models (Doc2Vec, Sentence Transformers)
│── 📂 scripts              # Python scripts for AI processing
│── 📂 webapp               # Flask-based web interface
│── README.md               # Project documentation (this file)
│── requirements.txt        # Dependencies and libraries
│── app.py                  # Main Flask application
│── similarity_matcher.py    # Job matching logic using AI models
│── claude_interaction.py    # Claude API integration for AI skill suggestions
│── ifate_api_client.py      # Fetching job standards from IFATE API
```

## **Technologies Used**
- **Programming Language:** Python
- **Frameworks:** Flask, Jupyter Notebook
- **Machine Learning Models:** Sentence Transformers (all-MiniLM-L6-v2), Doc2Vec
- **NLP Libraries:** NLTK, SpaCy, Pandas
- **Frontend Technologies:** HTML, CSS
- **APIs Used:** IFATE API for occupational standards, Claude LLM for AI skill recommendations

## **Installation & Setup**
### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/ai-recruitment-platform.git
cd ai-recruitment-platform
```

### **2. Set Up a Virtual Environment**
```bash
python -m venv env
source env/bin/activate   # On Mac/Linux
env\Scripts\activate      # On Windows
```

### **3. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **4. Run the Web Application**
```bash
python app.py
```
The application should now be accessible at **http://127.0.0.1:5000/**.

## **How It Works**
1. **Input Job Description**: The user enters a job description or resume into the web interface.
2. **AI Matching Algorithm**: The **Sentence Transformer model** processes the text and compares it against **UK occupational standards** from **IFATE API**.
3. **Skill Recommendation**: The system queries **Claude LLM** for AI skill development suggestions.
4. **Results Displayed**: The user receives **job matching insights and AI skill improvement recommendations**.

## **Evaluation Metrics**
- **Precision, Recall, and F1-Score** for job matching accuracy.
- **Mean Reciprocal Rank (MRR)** and **Mean Average Precision (MAP)** for ranking performance.
- **User feedback surveys** to assess system usability.

## **Future Enhancements**
- Real-time labor market data integration.
- Expansion to support multiple languages.
- More advanced **bias mitigation techniques** in AI recruitment.

## **Author**
📌 **Hara Georgiou**  
📌 **BSc Computer Science, Newcastle University**  
📌 **Supervisor:** Dr. Matthew Forshaw  
