## setup

This repo is exactly the autogenerated code from `vue create demo` (version 3.10.0) with default everything, plus one linting error introduced.

## how to reproduce

```bash
mkdir "bug"
cd bug
git clone git@github.com:npfoss/vue-lint-bug.git demo
cd demo
yarn install
yarn run lint # finds the issue (mixed tabs/spaces). good!

cd ../..

mkdir "bu(g)"
cd "bu(g)"
git clone git@github.com:npfoss/vue-lint-bug.git demo
cd demo
yarn install
yarn run lint # says everything is fine. bad!
```
