# AWS Notes



### AWS Backup and termination of Servers

* move on aws main page> elasticbean stalk
* right click on required server > move on image > select the option from boot or not
* select the option create image
* name and discription of image
* Make new user
* IAM > user > create new user > atach policy
* from above save the access key and secret access key with user name
* move the image to new user account
* EC2 > rightclick > permissions
* launch server for verification of our backup which we take
* Elasticbean stalk > security groups > edit > remove > save
* RDS > instance > view trailuser > right click > terminate

### Terminal Commands

* ssh -ipadress
* password
* cd /root /backup
* backup ls
* mkdir foldername
* `mysql username -u -p -h` ---for checking access to this database
* password
* show databases
* mysql dump -u name -p -h | foldername
* mkdir s3
* `sudo apt-get install s3cmd` ---install s3cmd
* `s3cmd --configure` --- configure the Access and screct key
* `s3cmd ls`
* `mkdir s3 name`
* `s3cmd sync s3://bucketname`
* `mv foldername/path foldername/path` 
* `cd path mv s3-*/path`---move all backup files to another directory
* `scp foldername/path username folderpath`

### General Notes
* Patching, security updates after specific time
* Main panel of AWS
  * where diffrent application run and we select according to our need
  * first OS then choose an instance type then configure instance detail then add storage  then instance tay and security
* Mail relog
  * AWS give services of ses (simple email service) you can just send email no inbox in this
