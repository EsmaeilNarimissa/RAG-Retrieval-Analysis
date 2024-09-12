# **RAG System Performance Analysis**

This repository contains research code and analysis for evaluating the performance of Retrieval-Augmented Generation (RAG) systems, with a focus on document retrieval, splitting methods, and retrieval effectiveness across different document types. The study explores the impact of various retrieval and document-splitting techniques on RAG system accuracy and efficiency, using advanced metrics to assess the system's performance.

## **Project Overview**

The primary goal of this research is to assess the performance of RAG systems when retrieving information from three types of documents: textbooks, articles, and novels. We analyze how different document-splitting techniques (Recursive Character Splitter vs. Token-based Splitter) influence retrieval outcomes across two retrieval models:
- **OpenAI's text-embedding-3-small** model
- **LM Studio's bge-large-en-v1.5-gguf** model

### **Key Features**
- Comparative analysis of RAG performance across document types.
- Evaluation of document-splitting methods and their effect on retrieval efficiency.
- Use of multiple performance metrics (SequenceMatcher, BLEU, METEOR, and BERT Score) to thoroughly assess retrieval accuracy.

## **Repository Contents**
- `RAG_System_Performance_Analysis.ipynb`: A Jupyter Notebook containing the full exploratory analysis, performance comparison, and conclusions drawn from the study. This notebook:
  - Describes the setup of the RAG system using OpenAI and LM Studio models.
  - Analyzes the performance of Recursive Character Splitter vs. Token-based Splitter on different document types.
  - Provides visualizations of performance results.
  - Includes statistical analysis to validate findings.

- `requirements.txt`: Contains a list of all dependencies required to run the notebook, including:
  - Python libraries such as `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `jupyter`, and others needed for the notebook.

## **Installation Instructions**

### **Prerequisites**
- Python 3.x
- Jupyter Notebook installed (optional but recommended for running the `.ipynb` file)

### **Steps to Set Up the Environment**
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/RAG-System-Performance-Analysis.git
   cd RAG-System-Performance-Analysis
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the notebook `RAG_System_Performance_Analysis.ipynb` and run the cells to reproduce the analysis.

## **Usage**
This project analyzes RAG system performance across different retrieval models and document types. It can be used to:
- Assess the effectiveness of different retrieval and document-splitting methods.
- Perform statistical validation of retrieval outcomes.
- Adapt RAG systems for better performance depending on document types and retrieval objectives.

## **Results Summary**
1. **Document Types**: Articles typically perform better due to their concise structure, while textbooks and novels pose challenges due to their complexity and expansive narrative styles.
2. **Splitting Methods**: The Recursive Character Splitter consistently outperforms the Token-based Splitter across all document types, particularly in maintaining contextual integrity.
3. **Retrieval Models**: OpenAI's retrieval model excels in semantic understanding, while LM Studio's model shows strength in handling structured, technical content.

## **Future Directions**
- Further optimization of chunk and overlap sizes in document splitting.
- Exploration of hybrid retrieval models combining strengths from both OpenAI and LM Studio.
- Application of the novel evaluation methodology across a broader range of document types and RAG system configurations.

## **Contributing**
Contributions are welcome! If you'd like to contribute to this project, feel free to fork the repository and submit a pull request.

## **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

