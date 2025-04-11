# Create Rule

## Introduction
This prompt is to provide instructions on how to create a new rule.

## Instructions
1. Ask for the name of the rule
2. Create a yaml file under ../Rules with the rule name pascale case with extension .yam;
3. Use the template from ../Rule Templates/RuleTemplate.md
4. Ask for a description and add it under the Description section. Proof read it but don't chnage it.
5. Understand the schema and create a payloadtemplate that includes only field required from files from ..\schema
6. Give each field an appropriate name
7. Crteate the conditions that use the field name and meet the criteria from the description
8. Do NOT add any additional sections until requested.

## Example
rule:
  id: 
  name: <RuleName>
  description: <RuleDescription>
  payloadtemplate:
    - field: "gender"
      reference: "gppb_gender"    
  conditions:
    - field: "gender"
      operator: "equals"
      value: "Male"

[back](../Prompt.prompt.md)