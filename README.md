# Resume-Analysis-and-Chatbot-Application
Sure! Here’s a structured overview of your project, including a README, project title, approach, and achievements.

### Project Title
**Resume Analysis and Chatbot Application**

### README

#### Project Overview
The Resume Analysis and Chatbot Application is a comprehensive tool designed to assist in analyzing resumes and assessing their compatibility with job descriptions. Leveraging advanced natural language processing and machine learning techniques, this application allows users to upload resumes, analyze them against job descriptions, and interact with the analyzed data through a chat interface.

#### Features
- **Upload Resumes**: Supports uploading resumes in PDF format.
- **Analyze Resumes**: Compares resumes with job descriptions to provide detailed compatibility analysis.
- **Chat Interface**: Enables interaction with the analyzed resume data through a conversational interface.
- **Vector Store Integration**: Utilizes a vector store to manage and retrieve document embeddings efficiently.
- **Customizable Prompts**: Uses customizable prompts to tailor the analysis and interactions.

#### Installation
To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/resume-analyzer.git
   cd resume-analyzer
   ```

2. **Install Dependencies**:
   Ensure you have Python installed and run the following command:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**:
   Create a `.env` file in the project root directory and add your API keys:
   ```
   GROQ_API_KEY=your_groq_api_key
   ```

4. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

#### Usage
1. Upload a resume in PDF format.
2. Enter the job description in the provided text area.
3. Click on "Analyze Resume" to start the analysis.
4. Use the chat interface to ask questions about the analyzed resume.

### Project Approach
1. **Data Ingestion**: Load and split PDF resumes into manageable chunks using `PyPDFLoader` and `RecursiveCharacterTextSplitter`.
2. **Vector Store Creation**: Generate embeddings for the text chunks using `HuggingFaceEmbeddings` and store them in a `FAISS` vector store.
3. **Resume Analysis**: Analyze the resume against the job description using a pre-defined template and a language model (`ChatGroq`).
4. **Chat Interface**: Provide a chat interface that allows users to interact with the analyzed data using contextual and retrieval-based mechanisms.

### Project Achievements
- **Efficient Resume Processing**: Successfully implemented a robust pipeline for processing and analyzing resumes.
- **Seamless Integration**: Integrated advanced NLP models and vector stores for efficient data retrieval and analysis.
- **Interactive User Experience**: Developed a user-friendly chat interface to interact with the analyzed resume data.
- **Scalability**: Designed the application to handle large datasets, ensuring scalability and performance.
- **Customization**: Enabled customizable prompts and configurations to adapt to various use cases and requirements.


