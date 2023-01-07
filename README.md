# npm-monorepo-oclif-test
An npm workspace monorepo that includes a simple oclif app

# Run test

Install the project:
```
npm install
```

Followed by:
```
npm pack --ws
```

You will notice a tar file gets generated, but without the actual node_modules dependencies listed in `bundledDependencies`.
