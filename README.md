# ChatPdf
### **Langchain Ask PDF: A Step-by-Step Guide**

This Python-based application allows users to upload a PDF file and ask questions about its content in natural language. The system leverages a **Large Language Model (LLM)** to process the document and generate relevant responses. However, it is designed to provide answers strictly related to the uploaded PDF and will not respond to unrelated queries.

---

## **How the Application Works**

1. **Reading and Splitting the PDF Content:**  
   - The application first loads the PDF and extracts its textual content.  
   - Since a full document might be too large for processing at once, the text is divided into smaller sections or **chunks**.  

2. **Generating Vector Representations:**  
   - Each chunk is converted into a vector representation using **OpenAI embeddings**.  
   - These embeddings allow the application to understand the meaning of the text and compare different sections semantically.

3. **Finding Relevant Chunks Based on the Question:**  
   - When the user asks a question, the system searches for the chunks that are most **semantically similar** to the question.  
   - This ensures that only the most relevant portions of the PDF are considered when generating a response.

4. **Generating a Response:**  
   - The retrieved text chunks are fed into the LLM.  
   - The LLM then formulates a coherent and contextually accurate response based on the information present in the document.  

5. **User Interface:**  
   - The application uses **Streamlit**, a Python framework for creating interactive web applications, to build a user-friendly interface.  
   - Users can upload their PDF, type in questions, and receive AI-generated responses in real time.

---


## **How to Use the Application**

Once the installation is complete, launch the application using Streamlit:

```bash
streamlit run app.py
```

This command will start a local web server where you can interact with the application through your browser.

### **Using the Interface**
1. Upload a PDF file.  
2. Enter a question in the input field.  
3. The system will analyze the document and return a response based on the most relevant text sections.

---

## **Contributing**
This project is intended as a learning resource and is not actively maintained for contributions. It is designed to accompany a **YouTube tutorial**, which provides a step-by-step guide to building this application from scratch.

---

## **Result**
![Image](https://github.com/user-attachments/assets/cc85a1f6-710d-487d-be34-1ff48f7a4c3a)

---

