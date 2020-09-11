---
title: "スクリプト定義"
date: 2020-09-11T00:00:00+09:00
---

スクリプト定義はJavaScriptを使います。
前提としてXML定義に対し記述されている状態でなければなりません。

```xml
<?xml version="1.0" encoding="UTF-8" standalone="none"?>
<map active="false">

    <!-- 必要定義は省略します。 -->

    <!-- タグにスクリプトを記述する形式 -->
    <script>
        console.log('hello world.');
    </script>

    <!-- 外部ファイルを呼び出す形式 -->
    <script src="./script/hoge.js"/>

</map>
```


