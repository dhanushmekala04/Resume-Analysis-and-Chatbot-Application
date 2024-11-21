#**Resume Analysis and Chatbot Application**

### README

#### Project Overview
The Resume Analysis and Chatbot Application is a robust tool designed to streamline the process of analyzing resumes and assessing their compatibility with job descriptions. Leveraging advanced natural language processing and machine learning techniques, this application enables users to upload resumes, perform detailed analysis, and interact with the data through a chatbot interface.

#### Features
- **Upload Resumes**: Supports PDF resume uploads.
- **In-Depth Analysis**: Compares resumes with job descriptions to provide compatibility analysis.
- **Interactive Chatbot**: Allows users to ask questions and get responses based on the analyzed data.
- **Advanced NLP and Machine Learning**: Utilizes state-of-the-art models and vector stores for efficient data retrieval and analysis.

#### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/dhanushmekala04/Resume-Analysis-and-Chatbot-Application.git
   cd Resume-Analysis-and-Chatbot-Application
   ```

2. **Unzip Backend and Frontend Files**:
   ```bash
   unzip backend.zip
   unzip frontend.zip
   ```

3. **Install Dependencies**:
   Ensure you have Python installed and then run:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**:
   Create a `.env` file in the project root directory and add your API keys:
   ```
   GROQ_API_KEY=your_groq_api_key
   ```

5. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

#### Usage
1. **Upload a Resume**: Upload a resume in PDF format through the sidebar.
2. **Enter Job Description**: Enter the job description in the provided text area.
3. **Analyze Resume**: Click the "Analyze Resume" button to start the analysis.
4. **Interact**: Use the chat interface to ask questions about the analyzed resume.

### Project Approach
1. **Data Ingestion**: Load and split PDF resumes into manageable chunks using `PyPDFLoader` and `RecursiveCharacterTextSplitter`.
2. **Vector Store Creation**: Generate embeddings for the text chunks using `HuggingFaceEmbeddings` and store them in a `FAISS` vector store.
3. **Resume Analysis**: Compare resumes against job descriptions using a pre-defined template and a language model (`ChatGroq`).
4. **Chat Interface**: Provide a chat interface that allows users to interact with the analyzed data using contextual and retrieval-based mechanisms.

### Project Achievements
- **Efficient Resume Processing**: Successfully implemented a robust pipeline for processing and analyzing resumes.
- **Seamless Integration**: Integrated advanced NLP models and vector stores for efficient data retrieval and analysis.
- **Interactive User Experience**: Developed a user-friendly chat interface to interact with the analyzed resume data.
- **Scalability**: Designed the application to handle large datasets, ensuring scalability and performance.
- **Customization**: Enabled customizable prompts and configurations to adapt to various use cases and requirements.

### File Structure Overview

#### backend.zip
Contains the backend logic and processing scripts for the application. It includes:
1. **pdf_ingestion.py**: Handles loading and splitting PDF documents into manageable chunks.
2. **vector_store.py**: Creates and manages the vector store for storing embeddings.
3. **analysis.py**: Contains the logic for analyzing resumes against job descriptions using a language model.

#### frontend.zip
Contains the frontend components of the application. It includes:
1. **main_app.py**: Manages the main application interface, including uploading resumes and displaying analysis results.
2. **chat_interface.py**: Handles the chat interface, enabling interaction with the analyzed resume data.

#### app.py
Acts as the entry point for the Streamlit application, setting up the layout and integrating the backend and frontend components. It orchestrates the overall flow of the application.

### Example Usage

To run the application:
1. **Unzip the `backend.zip` and `frontend.zip` files**:
   ```bash
   unzip backend.zip
   unzip frontend.zip
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**:
   Create a `.env` file in the project root directory and add your API keys:
   ```bash
   echo "GROQ_API_KEY=your_groq_api_key" > .env
   ```

4. **Run the application**:
   ```bash
   streamlit run app.py
   ```

