lerna init
- check version
配置lerna.json(https://github.com/lerna/lerna)
 - npmClientArgs --no-package-lock 不生成package.lock.json

lerna create tian-test1
lerna create tian-test2
lerna add lodash --scope tian-test1
lerna add lodash --scope tian-test2
lerna bootstrap
lerna clean
