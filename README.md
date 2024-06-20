# Ansible Role: AWS EC2

This Ansible role creates an AWS EC2 instance and deploys a JAR artifact.

## Variables

- `aws_key_name`: The name of the AWS key pair.
- `aws_instance_type`: The EC2 instance type.
- `aws_image_id`: The AMI ID to use for the instance.
- `aws_region`: The AWS region.
- `aws_subnet_id`: The subnet ID.
- `aws_security_group`: The security group ID.
- `aws_instance_name`: The name tag for the instance.
- `jar_artifact_path`: The local path to the JAR artifact.

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - ansible-role-aws-ec2

### Usage
To use this role, include it in your playbook:

```yaml
- hosts: localhost
  roles:
    - ansible-role-aws-ec2
#use the below commad

#ansible-playbook {playbook-name}
