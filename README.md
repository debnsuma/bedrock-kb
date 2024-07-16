# Web to Wisdom: Transforming Web Content with Amazon Bedrock for Knowledge Bases

This repository contains the code used in the blog post [Web to Wisdom: Transforming Web Content with Amazon Bedrock for Knowledge Bases](https://community.aws/content/2j7MGeRCVUMb00EXlqIi1jk3lUa/web-to-wisdom-transforming-web-content-with-amazon-bedrock-knowledge-bases). The blog explores how to integrate web URL data with Amazon Bedrock to enhance Retrieval-Augmented Generation (RAG) applications.

## Overview

The blog post and the accompanying code demonstrate how to:

1. Create a vector store using Amazon OpenSearch Serverless (OSS).
2. Create a Knowledge Base (KB) with Amazon Bedrock.
3. Integrate web URLs as data sources for the KB.
4. Use the RetrieveAndGenerate and Retrieve APIs to fetch and generate responses from the KB.

## File Structure

- `KB_Bedrock_Web_URL.ipynb`: Jupyter Notebook containing all the code and steps described in the blog post.

## Getting Started

To run the code in this repository, you'll need:

- An AWS account with the necessary permissions to create and manage Amazon Bedrock and OpenSearch resources.
- The AWS SDK for Python (boto3) installed in your environment.
- Access to the seed URLs you wish to crawl and integrate into your KB.

### Steps

1. **Create the Vector Store**:
    - Follow the steps to create OSS policies and collections.
    - Initialize the OpenSearch client and create the vector index.

2. **Create the Knowledge Base**:
    - Set up the configuration for OpenSearch Serverless, chunking strategy, web URL, and embedding model.
    - Create the Knowledge Base using the configurations.

3. **Create a Web URL Data Source**:
    - Associate the created KB with a web URL data source.

4. **Data Sync**:
    - Start the data sync to fetch, preprocess, chunk, and store the web data in the vector store.

5. **Test the Knowledge Base**:
    - Use the RetrieveAndGenerate API to test the KB and generate responses.
    - Use the Retrieve API to fetch relevant context.

### Example Usage

Refer to the Jupyter Notebook `KB_Bedrock_Web_URL.ipynb` for detailed code and usage examples. The notebook provides a step-by-step guide on how to set up and use the new Web Crawler feature with Amazon Bedrock.

## Conclusion

Integrating web and enterprise data sources with Amazon Bedrock significantly enhances the capabilities of your RAG applications. With new data connectors for Atlassian Confluence, Microsoft SharePoint, and Salesforce, alongside web data sources and Amazon S3, you can streamline data workflows and improve the accuracy and relevance of AI-powered responses.

For more detailed instructions and explanations, please refer to the [blog post](https://community.aws/content/2j7MGeRCVUMb00EXlqIi1jk3lUa/web-to-wisdom-transforming-web-content-with-amazon-bedrock-knowledge-bases).
