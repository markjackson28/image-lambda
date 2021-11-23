# image-lambda

## Current LAB - 17

## AWS: S3 and Lambda

AWS Lambda allows writing code that is triggered in the cloud, without thinking about maintaining servers. We’ll use it today to automatically run some processing on image files after they’re uploaded to an S3 Bucket

- Create an S3 Bucket with “open” read permissions, so that anyone can see the images/files in their browser
- A user should be able to upload an image at any size, and update a dictionary of all images that have been uploaded so far
- When an image is uploaded to your S3 bucket, it should trigger a Lambda function which must:
  - Download a file called “images.json” from the S3 Bucket if it exists
  - The images.json should be an array of objects, each representing an image. Create an empty array if this file is not present
  - Create a metadata object describing the image
    - Name, Size, Type, etc.
  - Append the data for this image to the array
    - Note: If the image is a duplicate name, update the object in the array, don’t just add it
  - Upload the images.json file back to the S3 bucket

### Author: Mark Thanadabouth

### Collaborators: Alex and the whole class

### Reflections and Comments
If I were to be completely honest, I did not understand what the goal of the lab was. The only part I was able to do on my own was link up s3 and lambda to trigger an event. The rest of the lab made zero sense to me.

In class, I was mostly confused on what we were trying to do. It seems like we were able to get the `images.json` file but were not able to alter it. So during class, we got stuck at the buffer section. Also another transparent thing, I had no idea what the buffer was or what it was supposed to do. It seemed like it was just returning integers. Not sure what we were supposed to do with that buffer. Overall, this lab really made no sense to me. I hope we get a solution to this lab.
