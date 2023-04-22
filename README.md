# Data Science on AWS

## Description

This workshop shows AWS users how to use Amazon SageMaker and other associated services to build, train, and deploy generative AI models. These labs go through data science topics such as data processing at scale, model fine-tuning, real-time model deployment, and MLOps practices all through a generative AI lens.

Distributed data processing
---------------------------
In this workflow, we will use the [Amazon Customer Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/readme.html) for labs related to data processing as it contains a very large corpus of ~150 million customer reviews. This is useful for showcasing SageMaker's distributed processing abilities which can be extended to many large datasets. 

Fine-tuning FLAN-T5 for summarizing conversation dialog 
-------------------------------------------------------
After the data processing sections, we will build our FLAN-T5 based NLP model using the [dialogsum](https://huggingface.co/datasets/knkarthick/dialogsum) dataset from HuggingFace which contains ~15k examples of dialogue with associated summarizations.

## Table of Contents

Setup 
-----
0. [Lab overview](./00_Overview.ipynb)
1. [Setup workshop dependencies](./01_Setup_Dependencies.ipynb)

Distributed data processing
---------------------------
[HIDDEN] 2. [Register parquet data in S3 using AWS Glue and Amazon Athena](./wip/02_Register_Parquet_Glue_Athena.ipynb)
[HIDDEN] 3. [Visualize data with serverless distributed PySpark on SageMaker notebooks using Glue interactive sessions](./wip/03_Visualize_Reviews_Dataset_Glue_Spark.ipynb)
[HIDDEN] 4. [Analyze data quality with distributed PySpark on SageMaker Processing Jobs](./wip/04_Analyze_Data_Quality_ProcessingJob_Spark.ipynb)

Fine-tuning FLAN-T5 for summarizing conversation dialog 
-------------------------------------------------------
5. [Analyze the impact of prompt engineering using a HuggingFace model](./05_Generate_Text_Without_Fine_Tuning.ipynb)
6. Perform feature engineering on a raw text dataset using HuggingFace
   1. [Option A: Notebook processing in SageMaker studio](./06_Prepare_Prompt_Dataset.ipynb)
   2. [Option B: SageMaker Processing Job](./06b_Prepare_Prompt_Dataset_SageMaker_Cluster.ipynb)
7. Fine-tune a HuggingFace model for dialogue summarization
   1. [Option A: Jupyter notebook training in SageMaker studio](./07_Supervised_Fine_Tune_Generative_Model.ipynb)
   2. [Option B: SageMaker Training Job](./07b_Supervised_Fine_Tune_Generative_Model_SageMaker_Cluster.ipynb)
8. [Create an automated end-to-end ML MLOps workflow with SageMaker Pipelines](./08_Create_End_to_End_MLOps_Pipeline.ipynb)
9. [Deploy a fine-tuned generative AI model to a real-time SageMaker Endpoint](./09_Approve_and_Deploy_Model.ipynb)
10.[Run inference on a SageMaker Endpoint in real time](./10_Generate_Text_With_Fine_Tuning.ipynb)

## O'Reilly Book:  Data Science on AWS
This workshop is based on the O'Reilly Book, "Data Science on AWS", by Chris Fregly and Antje Barth @ AWS.

![Data Science on AWS](dsoaws_book_cover_sm.png)

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

