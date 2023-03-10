## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_instance.bastion](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_security_group.bastion_sg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ami"></a> [ami](#input\_ami) | Ami for our bastion host | `string` | `"ami-0aa7d40eeae50c9a9"` | no |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | instancetype of our EC2 | `string` | `"t2.micro"` | no |
| <a name="input_tag_bastion"></a> [tag\_bastion](#input\_tag\_bastion) | n/a | `string` | `"Bastion"` | no |
| <a name="input_vpc_subnet_id"></a> [vpc\_subnet\_id](#input\_vpc\_subnet\_id) | It provides subnet ID from VPC | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aws_instance_bastion"></a> [aws\_instance\_bastion](#output\_aws\_instance\_bastion) | Provides an EC2 instance resource. This allows instances to be created |
| <a name="output_aws_security_group_bastion_sg"></a> [aws\_security\_group\_bastion\_sg](#output\_aws\_security\_group\_bastion\_sg) | This sg allows to access our bastion host |
