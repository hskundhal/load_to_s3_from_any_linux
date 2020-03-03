# load_to_s3_from_any_linux


# install AWS CLI on the machine
sudo apt install awscli
#or
brew install awscli

# configure AWS
# create access_key and secret key on AWS and use them here

aws configure


# list all s3 buckets
aws s3 ls

# copy file to s3 bucket
aws s3 cp pathtofile s3://bucketname

# create s3 bucket
aws s3 mb s3://bucketname

# remove s3 bucket
aws s3 rb s3://bucket

# specify files to include exclude during uploading
aws s3 cp filedirectory s3://bucket --recursive --exclude "*.log"  --include "*.txt"


