# AWS Infrastructure as Code

Infrastructure-as-Code definitions for AWS resources.

## Structure

```
.
├── CloudFormation/     # CloudFormation templates (*.yaml)
└── (future)            # CDK apps, Terraform, etc.
```

Templates are organized by tooling — each directory holds resource definitions deployable via the respective IaC tool.

## Deploying

```bash
# CloudFormation
aws cloudformation create-stack \
  --stack-name my-stack \
  --template-body file://CloudFormation/<template>.yaml
```
