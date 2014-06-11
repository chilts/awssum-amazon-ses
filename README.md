NOTE: AwsSum is now deprecated. Please use [aws-sdk](https://www.npmjs.org/package/aws-sdk) instead.

# awssum-amazon-ses #

This is an ```AwsSum``` plugin!

You'll need to add [awssum-amazon-ses](https://github.com/awssum/awssum-amazon-ses/) to your package.json
dependencies. Both [awssum](https://github.com/awssum/awssum/) and
[awssum-amazon](https://github.com/awssum/awssum-amazon/) are pulled in as peer dependencies.

## Example ##

List verified email addresses:

```
var fmt = require('fmt');
var amazonSes = require('awssum-amazon-ses');

var ses = new amazonSes.Ses({
    'accessKeyId'     : process.env.ACCESS_KEY_ID,
    'secretAccessKey' : process.env.SECRET_ACCESS_KEY,
    'region'          : amazonSes.US_EAST_1
});

ses.ListVerifiedEmailAddresses(function(err, data) {
    fmt.dump(err, 'err');
    fmt.dump(data, 'data');
});
```

## Operations ##

### DeleteIdentity ###

Docs: [DeleteIdentity on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_DeleteIdentity.html)

### DeleteVerifiedEmailAddress ###

Docs: [DeleteVerifiedEmailAddress on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_DeleteVerifiedEmailAddress.html)

### GetIdentityDkimAttributes ###

Docs: [GetIdentityDkimAttributes on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_GetIdentityDkimAttributes.html)

### GetIdentityNotificationAttributes ###

Docs: [GetIdentityNotificationAttributes on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_GetIdentityNotificationAttributes.html)

### GetIdentityVerificationAttributes ###

Docs: [GetIdentityVerificationAttributes on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_GetIdentityVerificationAttributes.html)

### GetSendQuota ###

Docs: [GetSendQuota on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_GetSendQuota.html)

### GetSendStatistics ###

Docs: [GetSendStatistics on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_GetSendStatistics.html)

### ListIdentities ###

Docs: [ListIdentities on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_ListIdentities.html)

### ListVerifiedEmailAddresses ###

Docs: [ListVerifiedEmailAddresses on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_ListVerifiedEmailAddresses.html)

### SendEmail ###

Docs: [SendEmail on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_SendEmail.html)

### SendRawEmail ###

Docs: [SendRawEmail on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_SendRawEmail.html)

### SetIdentityDkimEnabled ###

Docs: [SetIdentityDkimEnabled on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_SetIdentityDkimEnabled.html)

### SetIdentityFeedbackForwardingEnabled ###

Docs: [SetIdentityFeedbackForwardingEnabled on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_SetIdentityFeedbackForwardingEnabled.html)

### SetIdentityNotificationTopic ###

Docs: [SetIdentityNotificationTopic on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_SetIdentityNotificationTopic.html)

### VerifyDomainDkim ###

Docs: [VerifyDomainDkim on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_VerifyDomainDkim.html)

### VerifyDomainIdentity ###

Docs: [VerifyDomainIdentity on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_VerifyDomainIdentity.html)

### VerifyEmailAddress ###

Docs: [VerifyEmailAddress on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_VerifyEmailAddress.html)

### VerifyEmailIdentity ###

Docs: [VerifyEmailIdentity on AWS](http://docs.amazonwebservices.com/ses/latest/APIReference/API_VerifyEmailIdentity.html)



# Author #

Written by [Andrew Chilton](http://chilts.org/) - [Blog](http://chilts.org/blog/) -
[Twitter](https://twitter.com/andychilton).

# License #

* [Copyright 2011-2013 Apps Attic Ltd.  All rights reserved.](http://appsattic.mit-license.org/2011/)
* [Copyright 2013 Andrew Chilton.  All rights reserved.](http://chilts.mit-license.org/2013/)

(Ends)
