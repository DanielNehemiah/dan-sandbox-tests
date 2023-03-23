# dan-sandbox-tests

These tests were run on an Amazon EC2 G4 instance of size g4dn.4xlarge

## Common Commands Used

- Initial command to SSH `ssh -i file_name.pem  ubuntu@ipaddress`
- To check os version `cat /etc/*-release`

## Way to access files on Filezilla
https://stackoverflow.com/questions/16744863/connect-to-amazon-ec2-file-directory-using-filezilla-and-sftp

## Create a kernel from an environment
`ipython kernel install --name "local-venv" --user`

## Starting jupyterlab to run in the background
`jupyter-lab --no-browser`
