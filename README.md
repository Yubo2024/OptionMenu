Android 菜单设计总结
创建菜单资源文件：

在 res/menu/ 目录下创建 option_menu.xml。
使用 <menu> 标签定义菜单项 <item>，设置 id、title 等属性。
在 Activity 加载菜单：

在 MainActivity.kt 中重写 onCreateOptionsMenu() 方法，使用 menuInflater.inflate() 加载 XML 菜单。
处理菜单点击事件：

在 onOptionsItemSelected() 方法中，通过 item.itemId 判断点击的菜单项，并执行相应操作（如 Toast 提示）。
设置 Toolbar（如果使用自定义 Toolbar）：

在 activity_main.xml 中添加 Toolbar，并在 MainActivity.kt 里用 setSupportActionBar(toolbar) 绑定。
这样就能成功创建一个 Android 菜单！
