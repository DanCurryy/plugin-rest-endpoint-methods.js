---
name: Get the customization template for an OIDC subject claim for a repository
example: octokit.rest.actions.getCustomOidcSubClaimForRepo({ owner, repo })
route: GET /repos/{owner}/{repo}/actions/oidc/customization/sub
scope: actions
type: API method
---

# Get the customization template for an OIDC subject claim for a repository

Gets the customization template for an OpenID Connect (OIDC) subject claim.
You must authenticate using an access token with the `repo` scope to use this
endpoint. GitHub Apps must have the `organization_administration:read` permission to use this endpoint.

```js
octokit.rest.actions.getCustomOidcSubClaimForRepo({
  owner,
  repo,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>owner</td><td>yes</td><td>

The account owner of the repository. The name is not case sensitive.

</td></tr>
<tr><td>repo</td><td>yes</td><td>

The name of the repository without the `.git` extension. The name is not case sensitive.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/oidc#get-the-customization-template-for-an-oidc-subject-claim-for-a-repository).
