# custodian-policies

python3 -m venv custodian

source custodian/bin/activate

pip install c7n


custodian run invalidami.yml -s out


custodian report  invalidami.yml -s out --format grid -p ec2-invalid-ami

///////////////////////////////////////////////////////

python3 -m venv custodian
source custodian/bin/activate
pip install c7n
# export AWS_DEFAULT_REGION=ap-south-1
# git clone https://github.com/jyothiadevops/custodian-policies.git
#custodian report  invalidami.yml -s out --format grid -p ec2-invalid-ami
cd custodian-policies
#custodian run invalidami.yml -s out --format grid -p ec2-invalid-ami
#custodian run -s out --region ap-south-1 invalidami.yml
custodian run -s out --region ap-south-1 *.yml


