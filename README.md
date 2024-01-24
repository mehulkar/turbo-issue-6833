# turbo-issue-6833

Repro steps:

1.Clone
1. `npm install`
1. `npx turbo run build`
1. `npx turbo run build`

Expect a cache hit the second time

You can delete caches to start over with: `git clean -fdx && npm install`
