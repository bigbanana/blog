---
layout: post
title: '安装及配置sublime作为文本编辑器'
category: 编辑器
tags: 编辑器 sublime 
---

### 1. 安装
[官方下载](http://www.sublimetext.com/3)

### 2. 汉化

运行SublimeText3 点击 Preferneces -> Browse Packages 会打开 X:\Program Files\Sublime Text\Data\Packages 目录，点击向上并找到X:\Program Files\Sublime Text\Data\Installed Packages目录，从附件中下载汉化包并解压，复制Default.sublime-package到这个目录，无需重启即可直接看到汉化效果。

[中文语言包](http://bigbanana.github.com/web/files/Sublime_Text_CN_3059.zip)

注：汉化前先安装package-control不然会有奇怪的错误。

### 3. 添加许可证

运行SublimeText3 点击 帮助 -> 添加许可证 输入以下代码。

```
—– BEGIN LICENSE —–
Andrew Weber
Single User License
EA7E-855605
813A03DD 5E4AD9E6 6C0EEB94 BC99798F
942194A6 02396E98 E62C9979 4BB979FE
91424C9D A45400BF F6747D88 2FB88078
90F5CC94 1CDC92DC 8457107A F151657B
1D22E383 A997F016 42397640 33F41CFC
E1D0AE85 A0BBD039 0E9C8D55 E1B89D5D
5CDB7036 E56DE1C0 EFCC0840 650CD3A6
B98FC99C 8FAC73EE D2B95564 DF450523
—— END LICENSE ——
```

### 4. 安装Package Control

按组合键 `ctrl+~` 打开命令行输入以下代码回车

```python
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

### 5. 完成

现在你可以去安装一些常用插件来提高开发效率了。
