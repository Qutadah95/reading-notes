# Introduction to Amazon S3

## What is Amazon S3?


Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance.

## Features of Amazon S3

1. Storage classes
2. Storage management
3. Access management
4. Data processing


## Storage logging and monitoring

* Automated monitoring tools

1. Amazon CloudWatch metrics for Amazon S3

2. AWS CloudTrail 

* Manual monitoring tools

1. Server access logging
2. AWS Trusted Advisor

## Analytics and insights


Amazon S3 offers features to help you gain visibility into your storage usage, which empowers you to better understand, analyze, and optimize your storage at scale.

* Amazon S3 Storage Lens
* Storage Class Analysis
* S3 Inventory with Inventory reports 

## Strong consistency


Amazon S3 provides strong read-after-write consistency for PUT and DELETE requests of objects in your Amazon S3 bucket in all AWS Regions

## How Amazon S3 works


Amazon S3 is an object storage service that stores data as objects within buckets. An object is a file and any metadata that describes the file.

## Buckets

A bucket is a container for objects stored in Amazon S3. You can store any number of objects in a bucket and can have up to 100 buckets in your account

## Objects

Objects are the fundamental entities stored in Amazon S3.

## Keys

An object key (or key name) is the unique identifier for an object within a bucket.

## S3 Versioning

You can use S3 Versioning to keep multiple variants of an object in the same bucket. 

## Version ID

When you enable S3 Versioning in a bucket, Amazon S3 generates a unique version ID for each object added to the bucket.

## Bucket policy

A bucket policy is a resource-based AWS Identity and Access Management (IAM) policy that you can use to grant access permissions to your bucket and the objects in it. 

## Access control lists (ACLs)

As a general rule, we recommend using S3 resource-based policies (bucket policies and access point policies) or IAM policies for access control instead of ACLs

## S3 Access Points

Amazon S3 Access Points are named network endpoints with dedicated access policies that describe how data can be accessed using that endpoint. 

## Regions

You can choose the geographical AWS Region where Amazon S3 stores the buckets that you create.
