# Cloud Infrastructure
> Web instances, databases, and Amazon Web Service apps.

## EC2 Instances
 - Elastic Compute Cloud: we can set up instances (which are like Virtual Machines) that run from remote server centers.
 * Navigating: aws.amazon.com > Services > EC2 > Launch Instance

    - choose your AMI (Amazon Machine Image / OS), Instance Type (which speaks to vCPU cores and ram)

## S3 Storage ("Buckets")
- After your bucket is created, edit your bucket policy with this json:
> {
    
    "Version": "2012-10-17",

    "Statement": [

        {

            "Effect": "Allow",

            "Principal": "*",

            "Action": [

            "s3:GetObject"

        ],

        "Resource": "arn:aws:s3:::YOUR_BUCKET_NAME/*"

        }

     ]

    }

-- Uploaded objects can be accessed and used via amazon hosted urls.