# mdBook 模板

该内容使用 [mdBook][mdbook] 构建 HTML 页面。

请修改根目录下的 `book.toml` 文件。

## 使用说明

- 下载 [mdBook][mdbook] 二进制文件，将路径添加进 `PATH` 环境变量；
- 切换到项目根目录，执行 `mdbook serve` 命令；
- 在浏览器中访问 [localhost:3000](http://localhost:3000) 即可阅览页面。

`mdbook serve` 默认侦听 `localhost:3000`。如需允许网络下其他设备访问，则允许 mdbook 通过防火墙，并将侦听地址设置为 `0.0.0.0`，端口可自定义。则其他设备可以通过在浏览器中访问 `http://[设备IP地址]:[端口号]` 浏览页面。

```
mdbook serve -n 0.0.0.0 -p 3000
```

亦可执行 `mdbook build` 命令，而后手动打开 `book` 目录下的 `index.html` 文件，开始阅览。

[mdbook]: https://github.com/rust-lang/mdBook
