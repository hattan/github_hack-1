# Personal Access Tokens

* Service Accounts created in AD and generate PAT against those

* GitHub Enterprise Server will discontinue the OAuth Authorizations API, which is used by integrations to create personal access tokens and OAuth tokens, and you must now create these tokens using our web application flow. The OAuth Authorizations API will be removed on November, 13, 2020. For more information, including scheduled brownouts, see the blog post.

## Octokit
https://github.com/octokit/go-octokit

## Findings
* No way to rotate a PAT automatically. Must create a new PAT.

## Demo:
* Create a new "service account user in GitHub Enterprise"
* Create TWO PATS A/B.
* Build s aimple App that uses PAT A and falls back to B.
* GitHub App to start a workflow.

### References
* https://docs.github.com/en/enterprise-server@3.0/developers/apps/authorizing-oauth-apps#device-flow
* https://docs.github.com/en/enterprise-server@3.0/rest/reference/oauth-authorizations#get-or-create-an-authorization-for-a-specific-app
* https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token
* https://docs.github.com/en/github/authenticating-to-github/about-authentication-with-saml-single-sign-on
* https://docs.github.com/en/github/authenticating-to-github/authorizing-a-personal-access-token-for-use-with-saml-single-sign-on
