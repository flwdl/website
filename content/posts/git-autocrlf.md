---
title: "git 自动转换换行符"
date: 2021-02-01T19:00:00+08:00
draft: false
---

纯文本文件的换行符分为两种，LF 和 CRLF。不同操作系统使用的换行符有不同，*nix 操作系统使用 LF，Windows 使用 CRLF。为了避免一些麻烦，一个 repository 中，文件的换行符应当保持统一。在 Git 中，就有自动转换换行符的功能，由 `core.autocrlf` 来设置。

`autocrlf` 有三个值，`true`、`false`、`input`。将 `core.autocrlf` 的值设置为 `<value>` 可以使用命令

    git config core.autocrlf <value>

如果其值为 `true`，将会用 CRLF 替换文件中的 LF；如果为 `false`，会保持文件中的换行符；如果为 `input`，会用 LF 替换文件中的 CRLF。

在本站的源码中，文件换行符统一使用 LF。
