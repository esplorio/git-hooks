# Esplorio git hooks

### pre-commit

Hook to run tests before any commit, making sure we either have all tests
passing, or know explicitly that they're failing.

Install by running the following code in the root of your Git repo:
`curl https://raw.github.com/esplorio/git-hooks/master/pre-commit -o .git/hooks/pre-commit && chmod +x .git/hooks/pre-commit`

**NOTE**: This will clobber any existing pre-commit hooks you have, so make
sure that if you do have any they're safely saved, using something like:
`cp .git/hooks/pre-commit .git/hooks/pre-commit.original`
