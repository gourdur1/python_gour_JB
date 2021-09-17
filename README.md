# python_gour_JB

Clone this repo and execute the command: pip install -r requirements.txt

create a new AWS user and then store the new credentials.
To create a new user go to your AWS account, then go to Services and select IAM. Then choose Users and click on Add user,
Give the user a name and Enable programmatic access. This will ensure that this user will be able to work with any AWS supported SDK or make separate API calls.

choose the preconfigured AmazonS3FullAccess policy. With this policy, the new user will be able to have full control over S3

Click on 
"Next: Review"

Click on
"Create user"

A new screen will show you the user’s generated credentials. Click on the Download .csv button to make a copy of the credentials.

Create a credentials file by executing : touch ~/.aws/credentials

Open the file and paste the structure below. Fill in the placeholders with the new user credentials you have downloaded (save the file afterwards):

[default]

aws_access_key_id = YOUR_ACCESS_KEY_ID

aws_secret_access_key = YOUR_SECRET_ACCESS_KEY




Create a new file by executing the command : touch ~/.aws/config
Add the following and replace the placeholder with the region you have copied (save the file afterwards):

[default]

region = YOUR_PREFERRED_REGION
