rule:
  id: <RuleID>
  name: <RuleName>
  description: <RuleDescription>
  payloadtemplate:
    - field: "gender"
      reference: "gppb_gender"    
  conditions:
    - field: "gender"
      operator: "equals"
      value: "Male"