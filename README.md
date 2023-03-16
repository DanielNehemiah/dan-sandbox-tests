# dan-sandbox-tests

These tests were run on an Amazon EC2 G4 instance of size g4dn.4xlarge

## Common Commands Used

- Initial command to SSH `ssh -i file.pem  ec2-user@ipaddress`
- To check os version `cat /etc/*-release`

## Installing git

- Update package manager sources `sudo yum update -y`
- Install git with yum package manager `sudo yum install git -y`
- Check version after installation `git version`
