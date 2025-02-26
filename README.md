# GraphRAG_Neo4j_Chinese
Experimenting use of GraphRAG and Neo4j to create knowledge base and support queries on Chinese documents.

Copy GraphRAG_Neo4J_Chinese.ipynb to Google colab, open the notbook file, do the following:
1. Make a copy of .env.example and rename to .env
2. Create a folder ./input in colab, and copy hetangyuese_zhuziqing_utf8.txt in input folder to ./input in colab. This is a Zhu Ziqing's essay 《荷塘月色》int text format in UTF8 encoding.
3. Create a neo4j account. Use the free default instance, or create a trial or paid instance. From the credentials file downloaded when creating the instnace, copy appropriate values to set values for NEO4J_URI,
NEO4J_USERNAME, and NEO4J_PASSWORD. 
4. Run the cells. 
5. More questions can be asked by composing queries and calling chain.invoke(input="<query>")

# Automated Evaluation of GraphRAG Applications
The notebook graphrag_evaluation.ipynb is an example of automated evaluation of GraphRAG applications using Giskard. It uses a set of Chinese documents (朱自清的三篇散文：《荷塘月色》，《背影》，《桨声灯影里的秦淮河》）to build a knowledge base. A set of questions are automatically generated, and used to evaluate the model under test for knowledhe base, retrieval, question rewrite, routing, and generation.  
