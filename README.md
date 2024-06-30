# Cryman (NTHook)

## 使用

1. 安装本体

如果你使用插件框架，直接将本体扔到 `plugins` 文件夹内即可；

不适用插件框架的话，在 `launcher.js` 里直接 `require('本repo的src/index.js')` 即可

2. 将 protoc 扔进 src 文件夹

protoc 在这里下载： <https://github.com/protocolbuffers/protobuf/releases>

如果不想扔 src 文件夹，也可以通过环境变量 `DEVTOOLS_PROTOC` 指定 protoc 的位置

3. 将 build 文件夹扔进 src 文件夹

build 文件夹在这里下载： <https://github.com/bakyrd/ipcman/releases/tag/v0.1.3>

下载 `devtools.zip` 解压后里面就有 build 文件夹

如果不想扔 src 文件夹，也可以通过环境变量 `DEVTOOLS_BUILD_PATH` 指定 build 文件夹位置

4. 将 `crychiccat/packages/pb` 文件夹扔进 src 文件夹（可选）

注意扔进去之后，src 内的目录结构应该类似： `src/crychiccat/packages/pb`

如果不想扔 src 文件夹，也可以通过环境变量 `DEVTOOLS_CRYCHICCAT_PACKAGES` 指定上述 `packages`
文件夹位置，注意要指定的是 `crychiccat/packages` 文件夹

这个文件夹不扔也可以，不扔看不到字段名称但不影响运行

## 各 Hook 版本区别

Hook 版本|收|发
-|-|-
v1|仅消息|不支持消息
v2|完美|Inst/Seq 需要分别处理
v3|完美|完美
