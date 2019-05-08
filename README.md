# ![LOGO](logo.png) GraphRbacManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the GraphRbacManagementClient API (version 1.6).

Generated from: https://api.apis.guru/v2/specs/windows.net/graphrbac/1.6/swagger.json<br/>
Generated at: 2019-05-07T17:44:57+03:00

## API Description

The Graph RBAC Management Client

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists applications by filter parameters.

*Tags:* `Application`

#### Input Parameters
* `$filter` - _optional_ - The filters to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Create a new application.

*Tags:* `Application`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Delete an application.

*Tags:* `Application`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Get an application by object ID.

*Tags:* `Application`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Update an existing application.

*Tags:* `Application`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Add an owner to an application.

*Tags:* `ApplicationOwners`

#### Input Parameters
* `applicationObjectId` - _required_ - The object ID of the application to which to add the owner.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Remove a member from owners.

*Tags:* `ApplicationOwners`

#### Input Parameters
* `applicationObjectId` - _required_ - The object ID of the application from which to remove the owner.
* `ownerObjectId` - _required_ - Owner object id
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Get the keyCredentials associated with an application.

*Tags:* `ApplicationKeyCredentials`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Update the keyCredentials associated with an application.

*Tags:* `ApplicationKeyCredentials`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Directory objects that are owners of the application.

> The owners are a set of non-admin users who are allowed to modify this object.

*Tags:* `ApplicationOwners`

#### Input Parameters
* `applicationObjectId` - _required_ - The object ID of the application for which to get owners.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Get the passwordCredentials associated with an application.

*Tags:* `ApplicationPasswordCredentials`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Update passwordCredentials associated with an application.

*Tags:* `ApplicationPasswordCredentials`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a list of deleted applications in the directory.

*Tags:* `deletedApplications`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Hard-delete an application.

*Tags:* `Application`

#### Input Parameters
* `applicationObjectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Restores the deleted application in the directory.

*Tags:* `deletedApplications`

#### Input Parameters
* `objectId` - _required_ - Application object ID.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a list of domains for the current tenant.

*Tags:* `Domain`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a specific domain in the current tenant.

*Tags:* `Domain`

#### Input Parameters
* `domainName` - _required_ - name of the domain.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets the directory objects specified in a list of object IDs. You can also specify which resource collections (users, groups, etc.) should be searched by specifying the optional types parameter.

*Tags:* `Objects`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets list of groups for the current tenant.

*Tags:* `Group`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Create a group in the directory.

*Tags:* `Group`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Add a member to a group.

*Tags:* `Group`

#### Input Parameters
* `groupObjectId` - _required_ - The object ID of the group to which to add the member.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Remove a member from a group.

*Tags:* `Group`

#### Input Parameters
* `groupObjectId` - _required_ - The object ID of the group from which to remove the member.
* `memberObjectId` - _required_ - Member object id
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Delete a group from the directory.

*Tags:* `Group`

#### Input Parameters
* `objectId` - _required_ - The object ID of the group to delete.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets group information from the directory.

*Tags:* `Group`

#### Input Parameters
* `objectId` - _required_ - The object ID of the user for which to get group information.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Add an owner to a group.

*Tags:* `GroupsOwners`

#### Input Parameters
* `objectId` - _required_ - The object ID of the application to which to add the owner.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Remove a member from owners.

*Tags:* `GroupsOwners`

#### Input Parameters
* `objectId` - _required_ - The object ID of the group from which to remove the owner.
* `ownerObjectId` - _required_ - Owner object id
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a collection of object IDs of groups of which the specified group is a member.

*Tags:* `Group`

#### Input Parameters
* `objectId` - _required_ - The object ID of the group for which to get group membership.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets the members of a group.

*Tags:* `Group`

#### Input Parameters
* `objectId` - _required_ - The object ID of the group whose members should be retrieved.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Directory objects that are owners of the group.

> The owners are a set of non-admin users who are allowed to modify this object.

*Tags:* `GroupOwners`

#### Input Parameters
* `objectId` - _required_ - The object ID of the group for which to get owners.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Checks whether the specified user, group, contact, or service principal is a direct or transitive member of the specified group.

*Tags:* `Group`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets the details for the currently logged-in user.

*Tags:* `SignedInUser`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Get the list of directory objects that are owned by the user.

*Tags:* `SignedInUser`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Queries OAuth2 permissions grants for the relevant SP ObjectId of an app.

*Tags:* `OAuth2PermissionGrant_List`

#### Input Parameters
* `$filter` - _optional_ - This is the Service Principal ObjectId associated with the app
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Grants OAuth2 permissions for the relevant resource Ids of an app.

*Tags:* `OAuth2PermissionGrant_Create`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Delete a OAuth2 permission grant for the relevant resource Ids of an app.

*Tags:* `OAuth2PermissionGrant_delete`

#### Input Parameters
* `objectId` - _required_ - The object ID of a permission grant.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a list of service principals from the current tenant.

*Tags:* `ServicePrincipal`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Creates a service principal in the directory.

*Tags:* `ServicePrincipal`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Deletes a service principal from the directory.

*Tags:* `ServicePrincipal`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal to delete.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets service principal information from the directory. Query by objectId or pass a filter to query by appId

*Tags:* `ServicePrincipal`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal to get.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Updates a service principal in the directory.

*Tags:* `ServicePrincipal`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal to delete.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Get the keyCredentials associated with the specified service principal.

*Tags:* `ServicePrincipalKeyCredentials`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal for which to get keyCredentials.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Update the keyCredentials associated with a service principal.

*Tags:* `ServicePrincipalKeyCredentials`

#### Input Parameters
* `objectId` - _required_ - The object ID for which to get service principal information.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Directory objects that are owners of this service principal.

> The owners are a set of non-admin users who are allowed to modify this object.

*Tags:* `ServicePrincipalOwners`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal for which to get owners.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets the passwordCredentials associated with a service principal.

*Tags:* `ServicePrincipalPasswordCredentials`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Updates the passwordCredentials associated with a service principal.

*Tags:* `ServicePrincipalPasswordCredentials`

#### Input Parameters
* `objectId` - _required_ - The object ID of the service principal.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets list of users for the current tenant.

*Tags:* `User`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply to the operation.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Create a new user.

*Tags:* `User`

#### Input Parameters
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets a collection that contains the object IDs of the groups of which the user is a member.

*Tags:* `User`

#### Input Parameters
* `objectId` - _required_ - The object ID of the user for which to get group membership.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Delete a user.

*Tags:* `User`

#### Input Parameters
* `upnOrObjectId` - _required_ - The object ID or principal name of the user to delete.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Gets user information from the directory.

*Tags:* `User`

#### Input Parameters
* `upnOrObjectId` - _required_ - The object ID or principal name of the user for which to get information.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

### Updates a user.

*Tags:* `User`

#### Input Parameters
* `upnOrObjectId` - _required_ - The object ID or principal name of the user to update.
* `api-version` - _required_ - Client API version.
* `tenantID` - _required_ - The tenant ID.

## License

**flow**ground :- Telekom iPaaS / windows-net-graphrbac-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
