# Data Science on AWS

## Description

This workshop shows AWS users how to use Amazon SageMaker and other associated services to build, train, and deploy generative AI models. These labs go through data science topics such as data processing at scale, model fine-tuning, real-time model deployment, and MLOps practices all through a generative AI lens.

Distributed data processing
---------------------------
In this workflow, we will use the [Amazon Customer Reviews Dataset](https://s3.amazonaws.com/dsoaws/amazon-reviews-pds/readme.html) for labs related to data processing as it contains a very large corpus of ~150 million customer reviews. This is useful for showcasing SageMaker's distributed processing abilities which can be extended to many large datasets. 

Fine-tuning FLAN-T5 for summarizing conversation dialog 
-------------------------------------------------------
After the data processing sections, we will build our FLAN-T5 based NLP model using the [dialogsum](https://huggingface.co/datasets/knkarthick/dialogsum) dataset from HuggingFace which contains ~15k examples of dialogue with associated summarizations.

## Table of Contents

### Setup 
-----------------------------------------------
* 00a. [Lab overview](./00a_Overview.ipynb)
* 00b. [Setup workshop dependencies](./00b_Setup_Dependencies.ipynb)

### PART 1: Distributed data processing
-----------------------------------------------
* 01a. [Register parquet data in S3 using AWS Glue and Amazon Athena](./01a_Register_Parquet_Glue_Athena.ipynb)
* 01b. [Visualize data with serverless distributed PySpark on SageMaker notebooks using Glue interactive sessions](./01b_Visualize_Reviews_Dataset_Glue_Spark.ipynb)
* 01c. [Analyze data quality with distributed PySpark on SageMaker Processing Jobs](./01c_Analyze_Data_Quality_ProcessingJob_Spark.ipynb)

### PART 2: Fine-tuning FLAN-T5 for summarizing conversation dialog (SageMaker Studio Notebook)
-----------------------------------------------
* 02a. [Analyze the impact of prompt engineering using a HuggingFace model](./02a_Generate_Text_Without_Fine_Tuning.ipynb)
* 02b. [Perform feature engineering on a raw text dataset using HuggingFace (Studio Notebook)](./02b_Prepare_Prompt_Dataset.ipynb)
* 02c. [Fine-tune a HuggingFace model for dialogue summarization (Studio Notebook)](./02c_Supervised_Fine_Tune_Generative_Model.ipynb)

### PART 3: Fine-tuning FLAN-T5 for summarizing conversation dialog (SageMaker Cluster)
-----------------------------------------------
* 03a. [Perform feature engineering on a raw text dataset using HuggingFace (SageMaker Processing Job)](./03a_Prepare_Prompt_Dataset_SageMaker_Cluster.ipynb)
* 03b. [Fine-tune a HuggingFace model for dialogue summarization (SageMaker Training Job)](./03b_Supervised_Fine_Tune_Generative_Model_SageMaker_Cluster.ipynb)

### PART 4: Automating fine-tuning workflows with SageMaker Pipelines
--------------------------------------------------------------------------------------
* 04a. [Create an automated end-to-end ML MLOps workflow with SageMaker Pipelines](./04a_Create_End_to_End_MLOps_Pipeline.ipynb)
* 04b. [Deploy a fine-tuned generative AI model to a real-time SageMaker Endpoint](./04b_Approve_and_Deploy_Model.ipynb)
* 04c. [Run inference on a SageMaker Endpoint in real time](./04c_Generate_Text_with_Fine_Tuning.ipynb)

### PART 5: Advanced fine-tuning with PEFT and RLHF
-----------------------------------------------
* 05a. [Parameter-efficient fine-tuning with LoRA](./05a_LoRA_PEFT_Fine_Tune_Generative_AI_Model.ipynb)
* 05b. [Fine-tuning for human alignment using reinforcement learning with human feedback (RLHF)](./05b_RLHF_Fine_Tune_Model_to_Detoxify_Summaries.ipynb)

## O'Reilly Books: Generative AI on AWS and Data Science on AWS
This workshop is based on the O'Reilly Books, "Generative AI on AWS" and "Data Science on AWS" by Chris Fregly, Antje Barth, and Shelbee Eigenbrode @ AWS.

### Generative AI on AWS
[![Generative AI on AWS](img/gaia_book_cover.png)](https://www.amazon.com/Generative-AI-AWS-Multimodal-Applications/dp/1098159225/)

#### Related Links
* Website: https://generativeaionaws.com
* Meetup: https://meetup.generativeaionaws.com
* GitHub Repo: https://github.com/generative-ai-on-aws/
* YouTube: https://youtube.generativeaionaws.com
* O'Reilly Book: https://www.amazon.com/Generative-AI-AWS-Multimodal-Applications/dp/1098159225/

### Data Science on AWS
[![Data Science on AWS](img/book_full_color_sm.png)](https://www.amazon.com/Data-Science-AWS-End-End/dp/1492079391/)

#### Related Links
* Website: https://datascienceonaws.com
* Meetup: https://meetup.datascienceonaws.com
* GitHub Repo: https://github.com/data-science-on-aws/
* YouTube: https://youtube.datascienceonaws.com
* O'Reilly Book: https://www.amazon.com/Data-Science-AWS-End-End/dp/1492079391/

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

