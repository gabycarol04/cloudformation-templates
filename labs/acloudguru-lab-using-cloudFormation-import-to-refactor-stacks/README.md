# Import Resource to a template

For adding an existing resource to a AWS cloudformation template, we use the Import option, instead of the update option.

In this lab, we will create two diffetent stacks (The "Before" stacks). Then delete one dynamodb table from the Source stack, but the resource will not be deleted, because of a retain policy. So, we can import this resource, that is stackless to the Target stack with the import option.