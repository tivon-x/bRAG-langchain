# Retrieval-Augmented Generation (RAG) Project

This repository contains a comprehensive exploration of Retrieval-Augmented Generation (RAG) for various applications.
Each notebook provides a detailed, hands-on guide to setting up and experimenting with RAG from an introductory level to advanced implementations, including multi-querying and custom RAG builds.

![rag_detail_v2](assets/img/rag-architecture.png)

## Project Structure

### [1]\_rag_setup_overview.ipynb

This introductory notebook provides an overview of RAG architecture and its foundational setup.
The notebook walks through: 
- **Environment Setup**: Configuring the environment, installing necessary libraries, and API setups.
- **Initial Data Loading**: Basic document loaders and data preprocessing methods.
- **Embedding Generation**: Generating embeddings using various models, including OpenAI's embeddings.
- **Vector Store**: Setting up a vector store (ChromaDB/Pinecone) for efficient similarity search.
- **Basic RAG Pipeline**: Creating a simple retrieval and generation pipeline to serve as a baseline.

### [2]\_rag_with_multi_query.ipynb

Building on the basics, this notebook introduces multi-querying techniques in the RAG pipeline, exploring: 
- **Multi-Query Setup**: Configuring multiple queries to diversify retrieval.
- **Advanced Embedding Techniques**: Utilizing multiple embedding models to refine retrieval.
- **Pipeline with Multi-Querying**: Implementing multi-query handling to improve relevance in response generation.
- **Comparison & Analysis**: Comparing results with single-query pipelines and analyzing performance improvements.

### [3]_Customizing_RAG_Pipeline_Part1.ipynb
`notebook wip - coming soon`

This notebook delves deeper into customizing a RAG pipeline.
It covers: 
- **Custom Document Loaders**: Building loaders to handle specialized data formats.
- **Advanced Text Splitting**: Optimizing text chunking for better retrieval performance.
- **Fine-Tuned Embedding Models**: Customizing embeddings for domain-specific applications.
- **Enhanced RAG Pipeline**: Constructing a RAG pipeline that better suits the custom dataset and retrieval needs.

### [4]_Customizing_RAG_Pipeline_Part2.ipynb
`notebook wip - coming soon`

Continuing from the previous customization, this notebook explores: 
- **Custom Retriever Logic**: Designing retriever algorithms for improved search relevancy.
- **Contextual Prompting**: Crafting prompts dynamically based on retrieved content for better generation.
- **Evaluation Metrics**: Implementing metrics to evaluate retrieval accuracy and response quality.
- **Intermediate Testing**: Testing the pipeline's performance on a range of queries and gathering initial results.

### [5]_Scaling_and_Deploying_RAG_Pipeline.ipynb 
`notebook wip - coming soon`

This final notebook brings together the RAG system components, with a focus on scalability and optimization: 
- **Optimized Indexing**: Techniques to speed up indexing and retrieval in large datasets.
- **Scalability Testing**: Stress testing the pipeline under high query loads.
- **Advanced Fine-Tuning**: Fine-tuning both retriever and generator models for peak performance.
- **Pipeline Deployment**: Preparing the RAG pipeline for deployment, including API setup and server configuration.

## Getting Started

1.  **Clone the repository**:

    ```{bash}
    git clone https://github.com/yourusername/RAG_Project.git 

    cd RAG_Project
    ```

2.  **Install dependencies**: Make sure to install the required packages listed in `requirements.txt`.

    `pip install -r requirements.txt`

3.  **Run the Notebooks**:
    Begin with `[1]_rag_setup_overview.ipynb` to get familiar with the setup process. Proceed sequentially through the other notebooks to build and experiment with more advanced RAG concepts.

4.  **Set Up Environment Variables**:

    -   Duplicate the `.env.example` file in the root directory and name it `.env` and include the following keys (replace with your actual keys):

        ```         
        #LLM Modal
        OPENAI_API_KEY="your-api-key"

        #LangSmith
        LANGCHAIN_TRACING_V2=true
        LANGCHAIN_ENDPOINT="https://api.smith.langchain.com"
        LANGCHAIN_API_KEY="your-api-key"
        LANGCHAIN_PROJECT="your-project-name"

        #Pinecone Vector Database
        PINECONE_INDEX_NAME="your-project-index"
        PINECONE_API_HOST="your-host-url"
        PINECONE_API_KEY="your-api-key"
        ```

5.  **Notebook Order**:
    To follow the project in a structured manner:

    -   Start with `[1]_rag_setup_overview.ipynb`

    -   Proceed with `[2]_rag_with_multi_query.ipynb`

    `more coming soon`
    
    <!-- -   Then go through `rag_from_scratch_10_and_11.ipynb` -->

    <!-- -   Continue with `rag_from_scratch_12_to_14.ipynb` -->

    <!-- -   Finish with `rag_from_scratch_15_to_18.ipynb` -->

## Usage

After setting up the environment and running the notebooks in sequence, you can:

1.  **Experiment with Retrieval-Augmented Generation**:
    Use the foundational setup in `[1]_rag_setup_overview.ipynb` to understand the basics of RAG.

2.  **Implement Multi-Querying**:
    Learn how to improve response relevance by introducing multi-querying techniques in `[2]_rag_with_multi_query.ipynb`.

<!-- 3.  **Customize the RAG Pipeline**:
    Tailor the RAG pipeline to handle specific datasets and custom retrieval requirements, as explored in `rag_from_scratch_10_and_11.ipynb` and subsequent notebooks.

4.  **Evaluate and Optimize**:
    Test, evaluate, and deploy the optimized RAG pipeline in `rag_from_scratch_15_to_18.ipynb` for scalable applications. -->

<!-- ## Citations and Resources

Each notebook references relevant documentation and research materials:

-   **LangChain Documentation**: [LangChain Docs](https://langchain.readthedocs.io/en/latest/)

-   **OpenAI API Documentation**: [OpenAI API](https://beta.openai.com/docs/)

-   **ChromaDB Documentation**: Chroma Documentation

-   **Pinecone Documentation**: Pinecone Docs

-   **Multi-Query Retrieval**: [LangChain Multi-Query Example](https://langchain.readthedocs.io/en/latest/modules/retrievers/examples/multi_query.html)

-   **OpenAI Embeddings**: [Embedding Models Overview](https://beta.openai.com/docs/guides/embeddings)

-   **Fine-Tuning in RAG**: [Research Paper](https://arxiv.org/abs/2005.11401)

-   **RAG Evaluation and Metrics**: [Evaluation Metrics](https://arxiv.org/abs/2005.11401)

-   **Scalability Options**: [LangChain Scalability](https://langchain.readthedocs.io/en/latest/modules/scalability.html)

-   **Deployment Best Practices**: [LangChain Deployment Guide](https://langchain.readthedocs.io/en/latest/modules/deployment.html) -->

<br>

    Contributor: Taha Ababou