# Perform Foundational Data, ML, and AI Tasks in Google Cloud


As a junior data engineer in Jooli Inc. and recently trained with Google Cloud and a number of data services you have been asked to demonstrate your newly learned skills. The team has asked you to complete the following tasks.

You are expected to have the skills and knowledge for these tasks so don’t expect step-by-step guides.

### Task 1: Run a simple Dataflow job

You have used Dataflow in the quest to load data into BigQuery from Pub/Sub, now use the Dataflow batch template Text Files on Cloud Storage to BigQuery under "Process Data in Bulk (batch)" to transfer data from a Cloud Storage bucket (gs://cloud-training/gsp323/lab.csv). The following table has the values you need to correctly configure the Dataflow job.

You will need to make sure you have:

- Create a BigQuery dataset called BigQuery Dataset Name.
- Create a Cloud Storage Bucket called Cloud Storage Bucket Name

![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/bc8c9a2d-3c04-4405-96d6-14be33f1ec39)

Answer:

bq mk lab_191
gsutil mb gs://qwiklabs-gcp-00-9e1d8866bc92-marking
gsutil cp gs://cloud-training/gsp323/lab.csv .
gsutil cp gs://cloud-training/gsp323/lab.schema .
cat lab.schema


####  Create table in BigQuery
![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/0f9a09d0-783b-4e84-8bd8-f2b7f3083e0e)


#### Create a Job in DataFlow
![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/13e83dd4-8042-47b7-bb89-4b1739494cb2)

Template
![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/e6aae793-8727-483e-8c7a-8f806179d09e)

Machine Type

![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/05de103c-9977-4205-b92d-c2598569fb17)



### Task 2: Run a simple Dataproc job
You have used Dataproc in the quest, now you must run another example Spark job using Dataproc.

Before you run the job, log into one of the cluster nodes and copy the /data.txt file into hdfs (use the command hdfs dfs -cp gs://cloud-training/gsp323/data.txt /data.txt).

![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/d8b99a01-1767-4881-aa27-6046bfc50969)

#### Create a cluster on Compute Engine

Region

![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/645bb195-90c4-4926-a76e-86dc2065391e)


Nodes

![image](https://github.com/moniquecardoso25/Google-Cloud/assets/140358716/084e09da-5369-4535-a60c-ce3097642005)






### Task 3: Use the Google Cloud Speech API

Use Google Cloud Speech API to analyze the audio file gs://cloud-training/gsp323/task3.flac. Once you have analyzed the file, upload the resulting file to: Cloud Speech Location






### Task 4: Use the Cloud Natural Language API
Use the Cloud Natural Language API to analyze the sentence from text about Odin. The text you need to analyze is "Old Norse texts portray Odin as one-eyed and long-bearded, frequently wielding a spear named Gungnir and wearing a cloak and a broad hat." Once you have analyzed the text, upload the resulting file to: Cloud Natural Language Location





