# My Sublime3-Config（In Win10）

# 一、安装 PackageControl 

您可以到 [https://packagecontrol.io/installation](https://packagecontrol.io/installation) 上查看相关信息。

## 1. 自动安装

打开Sublime的Console，快捷键是 ctrl + ` （Tab上方的键），或者点击菜单栏中 View-Show Console，然后输入以下内容，敲回车，不过注意了，需要Python的支持。

**Sublime 3 （由packagecontrol.io提供）**

``import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)``

**Sublime 2（用于备忘）**

``import urllib2,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')``

还可以从 [http://sublime.wbond.net](http://sublime.wbond.net) 上面获取资源，或者获取Github上的资源。

具体可参考资料 [Sublime Text 3 安装 Package Control](http://jingyan.baidu.com/article/925f8cb817fd49c0dce05653.html) 。

## 2. 手动安装

可以至 [https://packagecontrol.io/installation](https://packagecontrol.io/installation) 右边，进行下载，当然亦可以到github上获取资源。

Github资源地址： [https://github.com/wbond/package_control](https://github.com/wbond/package_control)

具体可参考资料 [Sublime Text 3 安装 Package Control](http://jingyan.baidu.com/article/925f8cb817fd49c0dce05653.html) 。

# 二、使用 PackageControl 

## 1. 安装插件
	
	ctrl+shift+p 调出命令窗口：输入install package （当然可以模糊匹配，比如可以输入pci或者install等）

	插件列表：

		AdvancedNewFile
		ConvertToUTF8
		DocBlockr
		Emmet
		Git
		Package Control
		RailsCasts Colour Scheme
		SyncedSideBar

## 2. 移除插件

	ctrl+shift+p 调出命令窗口：输入remove 选择Remove Package 并回车

	再选择需要删除的插件即可

## 3. 更新插件

	ctrl+shift+p 调出命令窗口：输入upgrade 选择Upgrade Package 并回车

	如果没有需要更新的插件，则会提醒

	如果有更新的插件，则选择相应的插件即可

## 作者 (About)

- Stark Li

- Blog：[http://www.litianhua.net/](http://www.litianhua.net/)

- Email：starkli@126.com

- Github：[https://github.com/litianhua/](https://github.com/litianhua/)

- Git@OSC： [http://git.oschina.net/skyli/](http://git.oschina.net/skyli/)