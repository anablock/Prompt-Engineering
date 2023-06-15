# Authorize an Org Using the JWT Bearer Flow

* `"sfdcLoginUrl": "https://test.salesforce.com"`

## Run the auth:jwt:grant CLI command
Specify the client identifier from your connected app (also called the consumer key), the path to the private key file (server.key), and the JWT authentication username. When you authorize a Dev Hub org, set it as the default with the --setdefaultdevhubusername parameter. For example:

```
sfdx auth:jwt:grant --clientid 04580y4051234051 \
--jwtkeyfile /Users/jdoe/JWT/server.key --username jdoe@acdxgs0hub.org \
--setdefaultdevhubusername --setalias my-hub-org
```

This example shows how to use the --instanceurl parameter to specify an org hosted on https://test.salesforce.com rather than the default https://login.salesforce.com:

```
sfdx auth:jwt:grant --clientid 04580y4051234051 \
--jwtkeyfile /Users/jdoe/JWT/server.key --username jdoe@acdxgs0hub.org \
--instanceurl https://test.salesforce.com
```

## Resources
* https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_auth_jwt_flow.htm
* https://benahm0.medium.com/sfdx-org-authorization-%EF%B8%8F-a75b54861b54