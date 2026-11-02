# imgbed

个人图床仓库，存放 Markdown / 文档配图。

## 访问方式

图片通过 jsDelivr 加速访问：

```
https://cdn.jsdelivr.net/gh/adil-bit-hub/imgbed@main/img/<文件名>
```

原始地址（备用，国内直连可能不稳）：

```
https://raw.githubusercontent.com/adil-bit-hub/imgbed/main/img/<文件名>
```

## 上传

本机 PicGo 已配置为 GitHub 上传er，仓库 img/ 目录，PicGo 配置位于 ~/.picgo/config.json。
DeepSeek Harness 里可直接让我调用 picgo_upload 上传本地图片并返回链接。

## 注意

- 图片数量多了以后建议按年月分目录，避免仓库体积过大（GitHub 单仓库建议 < 1GB）。
- jsDelivr 对新文件有缓存延迟；若访问返回 301/404，可请求 https://purge.jsdelivr.net/gh/adil-bit-hub/imgbed@main/img/<文件名> 刷新。
