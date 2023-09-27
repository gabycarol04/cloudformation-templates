# cloudformation-templates

## Cloudformation Anatomy

Below are the different sections that a cloudformation can have
The only required section is “Resources”

**AWSTemplateFormatVersion:** "Version date exm: 2010-09-09" 
**Description:** "A string to describe the template"
**Metadata:** "A list of object to provide aditional information"
**Parameters:** "A list of parameters"
**Mappings:** "A set of key and values which can operate as a lookup table"
**Conditions:** "Set conditions on whether certain resources are created"
**Transform:** "List of transforms that are use to process the template like snippets"
**Resources:** "All resources to create or update"
**Outputs:** "Create outputs"