This policy will use to check empty SNS topics and delete them.

It will check for **all** of the following conditions, and if match, Cloud Custodian will report and/or take action accordingly

* `SubscriptionsConfirmed`	= `0`
* `SubscriptionsPending`	= `0`
* `SubscriptionsDeleted`	= `0`

The above conditions essentially means there are no subscriptions in a particular topic.
