# Bash Shell Wrapper For Github Search

Allows you to retrieve all the search results for a search query
using Github API v4, their GraphQL API.

# How to use it

You have to put in the organization as a separate argument. Otherwise
any valid GitHub search query should work.

For instance:

    bin/repo_search '10 days ago' 'my-organization' 'is:merged'

Would find all repos merged since 10 days ago.

## Limitations

1. Only has been tested on private repos.

