# s3_versioning_and_deleting_markers.dynamic_site_host_with_ec2
How to utilize s3 versioning and also host dynamic site with ec2 on AWS 

S3 VERSIONING, DELETING MARKERS AND HOSTING DYNAMIC WEBSITES

If someone alters a file, versioning allows you to have multiple copies in your s3 bucket. If a file is unintentionally or intentionally deleted, a delete marker would be placed on the deleted file inside your s3 bucket when versioning is enabled.

Create an s3 bucket

    • Search s3 in the AWS services
    • Select s3 and Create bucket.
    • Name the bucket
    • Assign a region and uncheck “block all public access” for the website to the publicly accessible.
    • Enable server-side encryption.
    • Disable static website hosting.
    • After configuring settings, upload your text files.
    • Make sure it accessible on the website
    • Select the text file, delete it
    • Enable show versioning to view the deleted version with other copies.
    • To restore file back, delete the file with the delete marker
    • Edit the text file and see both the old and new file present in the s3 bucket
    • To permanently delete a file, enable show version and select delete.

To host a dynamic site using MobaXterm
    • First create a role, a role allows a service in AWS communicate with another.
    • Go to the IAM console
    • Select roles and select create role
    • Name the role you want to create
    • Attach policy to the role
    • Review and Create
    • Create an s3 bucket
    • Name it, configure settings
    • Upload source code.

Launch an ec2.
Ec2 is a virtual machine or a server in AWS
    • Search ec2 in the all services in the management console
    • Select launch instance
    • Configure instance setting like the network, OS, Storage, Tags and Security Group
    • Launch instance

