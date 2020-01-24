### Set AWS account billing alerts using the Serverless framework.

This serverless framework project creates a cloudformation stack with [budgets](https://docs.aws.amazon.com/zh_tw/AWSCloudFormation/latest/UserGuide/aws-resource-budgets-budget.html "budget") for monthly and annual spending. It creates email alerts for each budget.
- Update the ***custom*** section of serverless.yml to suit your needs.
- Update the region, stage and profile in the `provider` section of serverless.yml.
- Deploy using an AWS profile/account with IAM permissions to create a budget resource. This is typically the root account.


------------


#### Instructions ####

Run the following command`sls deploy -v`


------------


#### Confirm deployment ####

In the AWS console, go to `My Billing Dashboard` > `Budgets`

You should see 2 budget resources.



