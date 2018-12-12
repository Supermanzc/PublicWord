#### 安装准备
* 1、找到菜单栏：Preferences → Package Control → Package Control:Install Package
* 2、没有找到Package Control，需要点击安装
   ```
   import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp  = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try           manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
   ```

#### 安装git
* 打开 Package Control 后搜索 git 回车即可，
```
{
    "git_command": "git安装目录\\Git\\cmd\\git.exe"
}
```

#### 安装 MarkdownEditing 插件 以及 Markdown Preview 方法同上
> MarkdownEditing安装的时候会出错，到时候拿下载一个 Markdown.sublime-syntax。
> 命令的使用ctrl+shift+p  md preview

#### 