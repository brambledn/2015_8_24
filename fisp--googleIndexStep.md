# fisp学习——google主页
 fisp的官方demo中只给出关于demo 的各种操作，初学fisp类型框架的孩纸不禁想如何能从零建一个项目？其实关键在于，根据目录规范（如下图）建立自己的各个文件夹，然后根据每个文件夹再开发出相应功能的文件，例如common是指通用库／基础库，就是放些复用性强的文件，如菜单组件等，common中又有几个子文件，page（模版页面，主要用于继承的模版页面，就是整个项目都需要用的部分）、widget（组件资源，如导航等、意在将页面内容聚合度较高的部分整合成一块）、static（能整合的块整合之后，剩下来的零散的资源）、plugin（用于存放smarty插件）、fis-conf.js（包括fisp的压缩打包等其他配置）
    |---site
     |     |---common #通用子系统
     |     |      |---config #smarty配置文件
     |     |      |---page #模板页面文件目录，也包含用于继承的模板页面
     |     |            └── layout.tpl
     |     |      |---widget #组件的资源目录，包括模板组件,JS组件,CSS组件等
     |     |      |     └── menu   #widget模板组件
     |     |      |     |    └── menu.tpl
     |     |      |     |    └── menu.js
     |     |      |     |    └── menu.css
     |     |      |     └── ui   #UI组件
     |     |      |          └── dialog  #JS组件
     |     |      |          |    └──dialog.js
     |     |      |          |    └──dialog.css
     |     |      |          └── reset #CSS组件
     |     |      |               └── reset.css
     |     |      |---static #非组件静态资源目录，包括模板页面引用的静态资源和其他静态资源
     |     |      |---plugin #模板插件目录(可选，对于特殊需要的产品线，可以独立维护)
     |     |      |---fis-conf.js #fis配置文件
     |     |---module1 #module1子系统
     |     |      |---test
     |     |      |---config
     |     |      |---page
     |     |            └── index.tpl
     |     |      |---widget
     |     |      |---static
     |     |      |     └── index #index.tpl模板对应的静态资源
     |     |      |          └── index.js
     |     |      |          └── index.css
     |     |      |---fis-conf.js #fis配置文件
   <pre><code>tell application "Foo"
    beep
end tell
</code></pre> var make=rr;
