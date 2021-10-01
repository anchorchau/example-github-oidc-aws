# Testing AWS Federation in Github Action
This repo is used to test whether IAM role assumption is working without using AWS IAM access key. 

## Requirement
- OIDC provider setup in AWS IAM. The issued URL will be *vstoken.actions.githubusercontent.com*
- Target Git repo URL. E.g: https://github.com/anchorchau/test_AWSRoleAssumption
- AWS Role ARN which will be assumed by.

## Result
It's totally doable although it's not officially published by Github yet. Probably, there will be the proper command to pass the token into AWS Web Identity Token file in the future.

## Reference
- https://github.com/glassechidna/ghaoidc
- https://awsteele.com/blog/2021/09/15/aws-federation-comes-to-github-actions.html
