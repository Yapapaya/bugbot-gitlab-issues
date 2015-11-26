# Bugbot Github Issues

A small library for working with Github Issues.

### Dev Setup

Create a file `.env` in the root and set the following:

```
GITHUB_CLIENT_SECRET=your secret here
GITHUB_CLIENT_ID=your app id here
NODE_ENV=development
TOKEN=""
```

Use a repl or the tests to exchange a register link callback code for a token which you can add to `.env` for convenience.

### Test

    npm test


## API

```
  github
    describe
    register((err, link)=>)
    token(code, (err, token)=>)
    repos(token, (err, repos[])=>)
    issues(token, repoID, (err, issues[])=>)
```