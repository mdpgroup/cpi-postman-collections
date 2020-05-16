# CPI Postman Collections

This repository contains Postman collection templates for SAP Cloud Platform Integration APIs.

Advantages of using these collections and the environment structure:

- Easy to switch between tenants, you can use the same environment information also for your Flows.
- A standardized and easy way to use CSRF token for the APIs that use `POST`, `PUT`, `DELETE` methods.
- Requests and responses are JSON by default. You can remove `Accept` and `Content-Type` headers to switch to XML.

## Available collections

### [Common Environment Template](cpi-tenant-template.postman_environment.json)

- [Download the environment](/../../raw/master/cpi-tenant-template.postman_environment.json)

### [Partner Directory](cpi-partner-directory.postman_collection.json)

- [Download the collection](/../../raw/master/cpi-partner-directory.postman_collection.json)
- API documentation: <https://api.sap.com/api/PartnerDirectory/resource>

## Installation & Usage

- Download the environment and the collection files
- Click import button in the top-left corner to import the collection.
- Use environment settings (gear icon) on the top-right corner to import the environment.
- For each tenant, you should duplicate the environment template and enter the specific URL, username, and password.
- You can also duplicate and rename collections to clearly separate request data between tenants.
- Choose the environment you defined earlier and start using collections.
- You should call `Get CSRF` request once before using e.g. `POST` methods in the collections. If you get a `403` response after a timeout period you can call `Get CSRF` request again.

## Contribution

This repo is open to contribution. You can send pull requests or open issues.

## License

Released under MIT license.
See the [LICENSE](LICENSE.md) file for license rights and limitations.

Brought to you by [MDP Group IT consulting](https://mdpgroup.com/en/)
