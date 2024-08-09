Consists of: 
Version: policy lang version
Id: Identifier(optional)
Statement: {
	Sid: identifier
	Effects:  Allow or Deny
	Principal: account/user/role to which the policy applies to
	Action: actions that this policy allows or denies
	Resource: list of resources to which the actions applied to
	Condition: conditions for when the policy is in effect
}
![[Policy.json.png]]
