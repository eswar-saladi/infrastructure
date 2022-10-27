# infrastructure

AWS CLI: https://docs.aws.amazon.com/cli/latest/reference/cloudformation/index.html

Create stack

```sh
aws cloudformation create-stack --stack-name myvpc --template-body file://network.yaml --profile produser
```

Delete stack

```sh
aws cloudformation delete-stack --stack-name myvpc  --profile produser
```

Update stack

```sh
aws cloudformation create-stack --stack-name myvpc --template-body file://s3_rds_network.yaml --profile devuser --capabilities CAPABILITY_NAMED_IAM
```

aws cloudformation create-stack --stack-name myvpc2 --template-body file://s3_rds_network.yaml --profile devuser --capabilities CAPABILITY_NAMED_IAM

aws cloudformation create-stack --stack-name myvpc3 --template-body file://s3_rds_network.yaml --profile devuser --capabilities CAPABILITY_NAMED_IAM