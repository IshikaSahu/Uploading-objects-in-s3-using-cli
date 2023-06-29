# Uploading-objects-in-s3-using-cli

1. Open Git bash and configure aws using your access key and secret key.
2. Create an S3 Bucket
   
   aws s3api create-bucket --bucket your-bucket-name --region your-region --create-bucket-configuration LocationConstraint=your-region
   in my case
   aws s3api create-bucket --bucket ish-b-10 --region ap-south-1 --create-bucket-configuration LocationConstraint=ap-south-1

![image](https://github.com/IshikaSahu/Uploading-objects-in-s3-using-cli/assets/71627396/6600d0b2-2744-4791-9834-9f9484a9223a)

As we go to s3 service we will find that our bucket is ready

![image](https://github.com/IshikaSahu/Uploading-objects-in-s3-using-cli/assets/71627396/1ebcdfd7-b077-4205-b4a3-d8244ce5f1a9)


3. Now we will upload file to s3 bucket
   
   aws s3 cp path/to/local/file s3://your-bucket-name/new-object-name.txt

![image](https://github.com/IshikaSahu/Uploading-objects-in-s3-using-cli/assets/71627396/8aa0aa36-661a-4ad9-a4a0-b0471d8fe5c4)

![image](https://github.com/IshikaSahu/Uploading-objects-in-s3-using-cli/assets/71627396/b272bd2c-3767-40fa-9116-fa1ed168ac23)


