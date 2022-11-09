# custodian-policies

source custodian/bin/activate


custodian run invalidami.yml -s out


custodian report  invalidami.yml -s out --format grid -p ec2-invalid-ami