# URL Product Extraction

[![Powered by Veridion](https://example.com/path/to/veridion-logo.png)](https://veridion.com)

### Description
- This project was developed as part of the "Hacking Big Numbers 2" Hackathon. Our aim is to extract information about products and categories from a list of URLs. The project can be particularly useful for e-commerce companies and other industries that need to quickly and accurately extract information from URLs.

### Steps that we followed

##### 1. Filtering Heuristics with Keywords
- We developed a set of heuristics based on keywords to filter out invalid or irrelevant URLs. This step helps us eliminate noise and focus on URLs likely to contain product information.

##### 2. Deep Learning-Based Classifier
- After applying the initial filtering heuristics, we used a deep learning-based classifier to further refine our list of URLs. This classifier was trained to identify URLs with higher probability of containing valuable product data.

##### 3. NER Model for Product Extraction
- Next, we wanted to use a Named Entity Recognition (NER) model to extract product names from the URLs that passed the previous filters. This model was designed to recognize product names and other relevant entities within the URL structure, but it didn't work as planed and we had to improvise because of the Hackathon time preasure. It was made with euristics.

##### 4. Assigning Product Categories with a Transformer-Based Model
- Finally, we applied a transformer-based model to assign product categories. This model cross-referenced extracted product names with a predefined list of categories, allowing us to categorize each product accurately.

##### 5. Parallel Training with a GPT-4 API Dataset
- To improve the performance and accuracy of our models, we trained them in parallel using a dataset generated with the GPT-4 API. This dataset provided a robust training ground, enhancing our models' ability to extract, classify, and categorize product information from URLs.