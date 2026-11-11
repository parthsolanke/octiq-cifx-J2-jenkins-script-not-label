# CI detection fixture

`sh label: 'Run tests', script: 'npm test'` - the command must come from `script:`, never from `label:`. Regression for commit ce17fa9.

Expected verdict line in the Octiq chat:

    Tests required - CI runs `npm test`   (NOT 'Run tests')
