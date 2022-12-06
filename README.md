# cla-assistant-test
Test repository for configuring CLA assistant

How to test:
- Open pull request to the repository
- Wait for the bot to comment
- Sign your pull request via adding a comment
- After PR is merged, new signature will be added to https://github.com/5afe/cla-assistant-test-signatures and the PR will be locked.

How to configure:
- See the https://github.com/5afe/cla-assistant-test/blob/main/.github/workflows/cla.yml for an example
- Add 'PERSONAL_ACCESS_TOKEN' secret to the repository containing a classic GitHub personal access token with "repo" scope. This way the bot can update its comments and add signatures to the signature repository.

Notes:
- signatures repository can be private
- signatures can be stored in the same repository
- personal access token will have an expiration date and will have to be updated after it expires for the CLA checks to work.
