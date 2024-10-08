# awscli
## to get the assigned role 
aws cli cmd : aws sts get-caller-identity
output: 
{
    "UserId": "AIDAxxx",
    "Account": "xxx",
    "Arn": "arn:aws:iam::xxx:user/ashrafDevOps"
}

### to get the roles details via cli
aws cli cmd : aws iam list-attached-role-policies --role-name ashrafDevOps
output:
{
  "AttachedPolicies": [
  {
    "PolicyName": "SomePolicy",
    "PolicyArn": "arn:aws:iam::aws:policy/xxx"
  },
  {
    "PolicyName": "AnotherPolicy",
    "PolicyArn": "arn:aws:iam::aws:policy/xxx"
  } ]
}

