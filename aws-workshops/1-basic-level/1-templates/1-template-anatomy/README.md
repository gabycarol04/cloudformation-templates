# **Template anatomy**

An AWS CloudFormation template is a declaration of the AWS resources that make up a stack. The template is stored as a text file in either JavaScript Object Notation (JSON) or YAML format. Because they are just text files, you can create and edit them in any text editor and manage them in your source control system with the rest of your source code.

The following example shows an AWS CloudFormation YAML template structure and its top-level objects:

| **Section** | **Description** | **isRequired** |
| --- | --- | --- |
| AWSTemplateFormatVersion | version of the CloudFormation template. Only accepted value is '2010-09-09'  | optional |
| Description | a text description of the Cloudformation template | optional |
| Metadata | objects that provide additional information about the template | optional |
| Parameters | a set of inputs used to customize the template | optional |
| Rules | a set of rules to validate the parameters provided at deployment/update | optional |
| Mappings | a mapping of keys and associated values | optional |
| Conditions | conditions that control whether certain resources are created | optional |
| Transform | for serverless applications  | optional |
| Resources | set of resources: a list of components of your infrastructure | **required** |
| Hooks | Used for ECS Blue/Green Deployments | optional |
| Outputs | values that are returned whenever you view your stack's properties  | optional |

**The only required top-level object is the Resources object**, which must declare at least one resource. The definition of each of these objects can be found in the online Template Anatomy  documentation

# **Stack**

A stack is a deployment of a CloudFormation template. You can create multiple stacks from a single CloudFormation template. A stack contains a collection of AWS resources that you can manage as a single unit. All the resources in a stack are defined by the stack's AWS CloudFormation template.

AWS CloudFormation will create, update or delete a stack in its entirety:

If a stack cannot be created or updated in its entirety, AWS CloudFormation will roll it back, and automatically delete any resources that were created.
If a resource cannot be deleted, any remaining resources are retained until the stack can be successfully deleted.