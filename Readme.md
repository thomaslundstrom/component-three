Component Three
===============

This module is used to test jspm installation via a npm registry

Since this is a dummy module, I recommend using a private npm repository, i.e.
something like https://github.com/rlidwka/sinopia to make sure you don't publish
to the real npm repo.

# Bumping a version

Some pointers, mainly stolen from https://gist.github.com/coolaj86/1318304.

1. Change the code that you wish to change and commit that
1. Bump version in package.json and commit that
1. Remember to do a git tag if you wish to go back and patch that version
1. Make sure you interface with the localhost npm repository, i.e. run
`npm set registry http://localhost:4873/`.
1. Publish the package to the repo by cd'ing into that directory and doing a
`npm publish ./`.
