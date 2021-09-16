# 更改PC机的背景桌面

- win+R → 输入“regedit”
- 在注册表编辑器中一次展开：HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\ 
- 设置背景桌面：
  1. 如果在Policies下没有System项，在该注册表项下建一个名为 System（文件夹）
  2. 在右侧栏，右键新建两个字符串值：“名称”为“Wallpaper”和“WallpaperStyle”
  3. 右键单击Wallpaper打开”编辑字符串“对话框，在”数值数据“栏输入桌面壁纸图片的路径，然后点击确定即可。
  4. 也可以通过此方法修改WallpaperStyle中”数值数据“的值，WallpaperStyle 有三个可以定义的值: 0=居中 ，1=平铺 ，2=拉伸，
- 删除桌面背景：删除变量“Wallpaper”和“WallpaperStyle”即可，或者直接删除HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\下的System项

