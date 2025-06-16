# Predicting-Future-Deep-Tech

This repository contains the code and supporting files for the Master's Semester Project on forecasting emerging technologies using Large Language Models (LLMs). The project explores two main distinct approaches to predict and evaluate the future emergence of technologies based on textual data and investment trends.

## 📁 Repository Structure
.

├── Approach1.ipynb # Implementation and validation code for Approach 1

├── Approach2.ipynb # Implementation and validation code for Approach 2

├── utils.py # Utility functions used in Approach 1

### 🔍 Overview of Approaches

- **Approach 1**:  
  Focuses on using a TF-IDF-based ground truth to generate and evaluate LLM predictions. Validation is done by comparing predicted rankings to true rankings using Kendall's tau correlation.  
  - Executed in Google Colab to make use of the T4 GPU for performance. We recommend using a GPU for certain sections of Approach 1 that are computationally intensive for a CPU.
  - The notebook was mounted to Google Drive for easier access to documents used for Retrieval-Augmented Generation (RAG) and the validation corpus. Ensure access to the required RAG documents and validation corpus. We suggest mounting your Google Drive in Colab for an easier access to the documents. Make sure to place the documents in your drive. You may need to adapt the file paths accordingly. 

  - utils.py contains reusable utility functions (for mainly for the manual RAG pipeline) used in Approach1.ipynb to improve modularity and maintainability.

- **Approach 2**:  
  Explores a forecasting method based on investment trends, where the LLM predicts investment figures for various technologies. Evaluation is based on normalized error metrics (MNAE and MNSE), which account for relative error across a wide range of investment values.

## 🛠 Requirements

To run the notebooks locally, install the required packages in the requirements file in your Colab environment or in a vritual environment if running in conda for instance. 
API keys are needed to use the different APIs: HF API, OpenAI API and Exa API.
