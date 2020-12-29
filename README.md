# AWS Machine Learning Cheat Sheet

<a href="https://www.linkedin.com/in/ryanxjhan/" target="_blank">LinkedIn</a>

### Table of Contents

* [Overview](#overview)
* [Data Engineering](#engi)
* 

<a name="overview"/>

### Overview

| Duration | Questions    | Formats                             |
| -------- | ------------ | ----------------------------------- |
| 170 mins | 65 questions | Multiple choice & multiple response |

 

<a name="engi"/>

### Data Engineering

#### Data Repositories

1. *AWS Lake Formation*

   AWS Lake Formation is a service that makes it easy to set up a secure data lake in days. 

* With Lake Formation, you can move, store, catalog, and clean your data faster.
* You can use Lake Formation to centrally define security, governance, and auditing policies in one place.
* With Lake Formation you build a data catalog that describes the different data sets that are available along with which groups of users have access to each.

![3](img/3.png)

2. *AWS S3*

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance.

![2](img/2.png)

| Storage Classes | Use cases                              | Availability Zones | Access  Time     |
| --------------- | -------------------------------------- | ------------------ | ---------------- |
| S3 Standard     | For active, frequently accessed data   | >= 3               | Milliseconds     |
| S3 INT          | For data with changing access patterns | >= 3               | Milliseconds     |
| S3 S-IA         | For infrequently accessed data         | >= 3               | Milliseconds     |
| S3 1Z-IA        | For re-creatable, less accessde data   | 1                  | Milliseconds     |
| Amazon Glacier  | For archive data                       | >=3                | Minutes or hours |

* Amazon S3 with Amazon SageMaker

  You can use Amazon S3 while you’re training your ML models with Amazon SageMaker. Amazon S3 is integrated with Amazon SageMaker to store your training data and model training output.

3. *Amazon FSx for Lustre*

   ![1](img/1.png)

   When your training data is already in Amazon S3 and you plan to run training jobs several times using different algorithms and parameters, consider using Amazon FSx for Lustre, a file system service. FSx for Lustre speeds up your training jobs by serving your Amazon S3 data to Amazon SageMaker at high speeds. The first time you run a training job, FSx for Lustre automatically copies data from Amazon S3 and makes it available to Amazon SageMaker. You can use the same Amazon FSx file system for subsequent iterations of training jobs, preventing repeated downloads of common Amazon S3 objects.



#### Data Ingestion

#### Data Transformation

