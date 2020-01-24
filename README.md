### Set AWS account billing alerts using the Serverless framework.

This serverless framework project creates a cloudformation stack with [budgets](https://docs.aws.amazon.com/zh_tw/AWSCloudFormation/latest/UserGuide/aws-resource-budgets-budget.html "budget") for monthly and annual spending. It creates email alerts for each budget.
- [Enable billing alerts](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html#turning_on_billing_metrics "Enable billing alerts") from the root account.
- Update the ***custom*** section of serverless.yml to suit your needs.
- Deploy using an AWS profile/account with IAM permissions to create a budget resource. This is typically the root account.


------------


#### Instructions ####

Run the following command `sls deploy -v`


------------


#### Confirm deployment ####

In the AWS console, go to `My Billing Dashboard` > `Budgets`

You should see 2 new budget resources.



