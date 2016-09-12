# autosnap
Automatically takes daily snapshots of your EBS volumes and delete expired snapshots.

Installation:

1) Copy the two zip files to an S3 bucket

2) Create a stack using the autosnap_template.json file

3) Give it the name of your S3 bucket

4) create your stack

After stack creation tag each of your EBS volumes to be backed up:

Name: Backup     Value: True

Name: Retention  Value: number of days' backups to retain

