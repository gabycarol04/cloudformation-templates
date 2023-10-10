# Guide and examples for cloudformation templates

AWS CloudFormation is a service that helps you model and set up your AWS resources. You create a template that describes all the AWS resources that you want (like Amazon EC2 instances or Amazon RDS DB instances), and CloudFormation takes care of provisioning and configuring those resources for you. You don't need to individually create and configure AWS resources and figure out what's dependent on what; CloudFormation handles that.

## Cloudformation Anatomy

Below are the different sections that a cloudformation can have. The only required section is “Resources”

- **AWSTemplateFormatVersion:** "Version date exm: 2010-09-09"
- **Description:** "A string to describe the template"
- **Metadata:** "A list of object to provide aditional information"
- **Parameters:** "A list of parameters"
- **Mappings:** "A set of key and values which can operate as a lookup table"
- **Conditions:** "Set conditions on whether certain resources are created"
- **Transform:** "List of transforms that are use to process the template like snippets"
- **Resources:** "All resources to create or update"
- **Outputs:** "Create outputs"