---
title: "マップ構造"
date: 2020-07-28T00:09:06+09:00
---

全てのXML定義ファイルは一つの `map` ノードが存在していなければなりません。また、ファイルの文字コードはUTF-8を使用してください。

```xml
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<map active="false">

    <name>CastleStoneNetwork</name>
    <version>1.0.0</version>
    <description>
        <text>Minecraftから</text>
        <text>新しい冒険を始めよう。</text>
    </description>

    <time>1800</time>
    <reward>1000</reward>
    <fee>0</fee>

    <world>csd_castlestone</world>

    <authors>
        <author name="the_karura" contribution="Owner, Administrator, Developer">db113963-10b7-41ec-b8a9-7d9fffd0cfc7</author>
        <author name="hayatarou_" contribution="Administrator, Developer">c65b1558-6410-4da7-9aef-cff42a2c1399</author>
    </authors>
</map>
```

### マップ名

説明文を設定します。 `Map Name` は文字列で指定してください。

```xml
<name>>Map Name</name>
```

### バージョン

説明文を設定します。 `Version` は文字列で `1.0.0` のようにコンマ区切りで数字を指定してください。

```xml
<version>Version</version>
```

### 説明文

説明文を設定します。 `Text` は文字列で指定してください。 `<text>` ノードで改行が可能です。

```xml
<description>
    <text>Text1</text>
    <text>Text2</text>
</description>
```

### 制限時間

制限時間を設定します。 `Second` は数値で指定してください。

```xml
<time>Second</time>
```

### 報酬

報酬を設定します。報酬は `Money` で支払われます。数値で指定してください。

```xml
<reward>Money</reward>
```

### 参加費

参加費を設定します。参加費は `Money` で徴収されます。数値で指定してください。

```xml
<fee>Money</fee>
```

### ワールドフォルダ

ワールドフォルダを設定します。 `World Folder` は `csd_[Map Name]` の形で指定してください。 `Map Name` は全て小文字で指定をしてください。

```xml
<world>World Folder</world>
```

### 製作者

#### `<author>`ノードの属性

| 属性 | 説明 | 値 |
|:----:|:----:|:----:|
| name | プレイヤーの名前です。 | 文字列 |
| contribution | 貢献内容を設定できます。 | 文字列 |

製作者を設定します。 `UUID` はPlayerUUIDを指定してください。

```xml
<authors>
    <author name="Player Name" contribution="Contribution">UUID</author>
</authors>
```
