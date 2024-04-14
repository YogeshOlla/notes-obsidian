This file will contian github management using terminal

Prerequisits
1. Github API key
2. SSH added to github

### List repositories
curl -H "Authorization: token YOUR_TOKEN" https://api.github.com/user/repos

### Create a repository
curl -X POST -H "Authorization: token YOUR_TOKEN" -d '{"name": "new-repo", "private": true}' https://api.github.com/user/repos

### Get repository information
curl -H "Authorization: token YOUR_TOKEN" https://api.github.com/repos/OWNER/REPO_NAME

### Update repository (e.g., change repository description)
curl -X PATCH -H "Authorization: token YOUR_TOKEN" -d '{"description": "New description"}' https://api.github.com/repos/OWNER/REPO_NAME

### Delete repository
curl -X DELETE -H "Authorization: token YOUR_TOKEN" https://api.github.com/repos/OWNER/REPO_NAME
