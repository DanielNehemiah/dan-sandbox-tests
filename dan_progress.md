## 16th March 2023 4pm to 6pm
1. Connected to instance
2. Installed git
3. Setup a git repo
4. Connected on Filezilla
5. Installed conda
    - Created an env with python 3.10
    - Installed cuda torch
6. Realized gpu drivers are not installed

### Todo
- Install transformers
- Test torch GPU
- Try inference with a roberta model


## 23rd March 2023 11.15am to 11.45am
1. Verified GPU availability: `lspci | grep -i nvidia`
2. Installed GCC as a pre-requisite to install CUDA `https://devcoops.com/install-gcc-on-amazon-linux-2/`
3. Installed updated kernel headers `sudo yum install kernel-devel-$(uname -r) kernel-headers-$(uname -r)`
    - uname -r
    - 5.10.167-147.601.amzn2.x86_64
    - Installed:
    - kernel-devel.x86_64 0:5.10.167-147.601.amzn2
4. Installed CUDA Toolkit https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&Distribution=CentOS&target_version=7&target_type=rpm_network
5. Tried to install NVIDIA drivers
    - `sudo yum install nvidia-driver-latest-dkms`
    - `sudo yum install cuda-drivers`
    - `sudo yum install nvidia-driver-latest-dkms`
    - `sudo yum install cuda`
    - `sudo yum install cuda-drivers`
6. Failed to install NVIDIA drivers
7. Suggested sagar to setup a different AMI with nvidua already set up


## 23rd March 2023 03.15pm to 5pm
1. Tried the new instance
2. Created an environment, installed torch and tested gpu with torch (`source dan/d_env/bin/activate`)
3. Installed and setup jupyter lab https://medium.com/analytics-vidhya/jupyterlab-on-aws-ec2-d6b2cb945e54
4. Installed transformers and tested roberta inference
5. Tested ESG-BERT inference
