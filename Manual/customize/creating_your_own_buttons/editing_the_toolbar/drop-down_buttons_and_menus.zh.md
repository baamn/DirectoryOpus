# 下拉按钮和菜单

下拉按钮是一种特殊类型的按钮，可以显示菜单。菜单可以包含一个或多个按钮，这些按钮本身也可以是下拉按钮。这使你可以创建级联菜单。下拉菜单的层级不受限制。

有两种不同类型下拉按钮：

- 菜单：下拉菜单是一个仅用于显示菜单的按钮。

![](/Manual/images/media/drop-down_menu.png)

单击按钮会显示菜单。

- 菜单按钮：下拉菜单按钮类似于常规按钮和菜单的组合。

![](/Manual/images/media/menu_button_1.png)

菜单按钮有两个不同的部分。较大的一部分 - 在上例中标记为 Rename - 充当常规按钮。可以为其定义函数，单击按钮部分将运行函数。

![](/Manual/images/media/menu_button_2.png)

较小的一部分 - 包含箭头字形 - 显示下拉菜单。单击按钮的箭头部分会下拉菜单。

![](/Manual/images/media/menu_button_3.png)

下拉按钮在自定义模式中像其他按钮一样进行编辑 - 请参阅 [编辑工具栏]() 页面，了解如何编辑工具栏上按钮的完整说明。在处理下拉按钮时有一些细微差别：

- 您可以将一种类型下拉按钮转换为另一种下拉按钮，然后反向转换。右键单击菜单或菜单按钮，然后从上下文菜单中选择 **转换** 命令。将菜单转换为菜单按钮时，菜单中的第一个按钮将变为菜单按钮的“按钮”部分。相反，菜单按钮的“按钮”部分将变成菜单中的第一个按钮。 
  \* 要编辑下拉按钮，您必须右键单击按钮，然后从上下文菜单中选择 **编辑** 命令 - 双击按钮不起作用。 
  \* 要编辑菜单内的按钮（适用于任何类型下拉按钮），首先单击按钮一次，打开菜单。再次单击按钮将关闭菜单。

工具栏顶层的下拉按钮会响应其标记中的和号 (**&**) 字符。这可以用来将按钮标记中的一个字母标记为一种热键 - 按 **Alt** 加该字母将打开菜单，便可使用键盘访问其内容。

![](/Manual/images/media/menu_button_edit.png)     

此屏幕截图显示了默认工具栏上 **重命名** 菜单按钮的定义。您可以看到按钮的标记实际上设置为 *Re&name* - 尽管在工具栏上显示为 *重命名*。标记中的“n”已被和号标记，这使您可以按 **Alt+N** 打开附加到 **重命名** 按钮的下拉菜单。按钮还定义了热键 (**Ctrl+3**) - 这适用于菜单按钮的“按钮”部分。按 Ctrl+3 将运行按钮的命令 (**高级重命名**) - 与单击“按钮”部分且没有下拉菜单相同。

  
如果您想在按钮的标记中使用文字和号，则必须在符号后加一个双 **&**（例如 *备份 && 恢复*）。