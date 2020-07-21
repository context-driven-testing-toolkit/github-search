# Bash Shell Wrapper For Github Search

Allows you to retrieve all the search results for a search query
using Github API v4, their GraphQL API.

This script requires some custom `jq` functions. To enable them
download `stdlib.jq` using the command shown below. Rename `stdlib.jq`
to `.jq` and place it in your `$HOME` directory:

    curl -sO https://raw.githubusercontent.com/context-driven-testing-toolkit/jq-stdlib/master/lib/jq/stdlib.jq

    cp stdlib.jq ~/.jq


# How to use it

You have to put in the organization as a separate argument. Otherwise
any valid GitHub search query should work.

For instance:

    repo_search '10 days ago' 'my-organization' 'is:merged'

Would find all repos merged since 10 days ago.

## Limitations

1. Only has been tested on private repos.
1. Results are sorted by last-updated.
