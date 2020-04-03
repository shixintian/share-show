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

关联内部模块
- lerna add tian-test2 --scope tian-test1
- 修改代码 tian-test1 引入tian-test2
- node 跑代码
- lerna changed  lerna diff
- 发布一次 npm publish
- npmjs.com 查看package

单独开发某个模块
- 修改 tian-test2
- node跑一下
-
