# FOLKSONOMY MINING - Topic Modeling Analysis on Twitter Data Using Llama-2

## Overview

Our project focuses on analyzing extensive Twitter data to extract meaningful topics using advanced machine learning models. The main components of the project include data preparation, model training, and evaluation.

## File Information

**SWM_LLama2.ipynb**: Contains the code for preprocessing the data, training the Llama-2 model, and visualizing the topics.

## Data Preparation

- **Data Source**: The dataset consists of multiple CSV files capturing tweet data on racial issues in the United States, collected between May 14th and 31st, 2023.
- **Preprocessing**: Tweets are grouped by language, unnecessary columns are dropped, and tweets with less than two characters are removed.
- **Data Storage**: Preprocessed data is stored in Amazon S3 buckets and further processed using AWS Glue and Athena.

## Model Training

- **Model Used**: Llama-2-13b-chat-hf variant, optimized and quantized using QLORA.
- **Embedding Calculation**: Sentence transformers are used to generate numerical representations of sentences for downstream applications.
- **Dimensionality Reduction**: UMAP model reduces the dimensionality of sentence embeddings, followed by clustering using the HDBScan model.

## Evaluation

- **Qualitative Measure**: Manual evaluation of selected tweet subsets to ensure relevance and coherence.
- **Quantitative Measure**: Metrics like perplexity and coherence are used to evaluate the model's performance.

## Visualizations

- **Topic Visualization**: Topics are represented in a 2D space, with inter-topic distances depicting relationships between topics.
- **Document Visualization**: Interactive plots allow users to explore the distribution of documents across topics.

## Conclusion

The project demonstrates the effectiveness of using advanced topic modeling techniques to analyze large-scale Twitter data. The results provide valuable insights into dynamic conversations on Twitter, with applications across various domains.

