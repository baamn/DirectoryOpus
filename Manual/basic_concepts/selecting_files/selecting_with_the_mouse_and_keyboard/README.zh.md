# 使用鼠标和键盘进行选择

除了增强模式，在所有 [视图模式](../the_lister/view_modes.zh.md) 下，使用鼠标或键盘选择文件的方式与资源管理器类似。

##### 使用鼠标选择文件

- 左键单击单个文件以选择该文件并取消选择所有其他文件。
- <kbd>Ctrl</kbd>+左键单击某个文件将切换该文件的选定状态，而不会改变所有其他文件。
- <kbd>Shift</kbd>+左键单击某个文件以选择一系列文件。正常单击以选择该系列中的第一个文件，然后按住 <kbd>Shift</kbd> 键并再次单击该系列中的最后一个文件。两个文件（包括两个文件在内）之间的所有文件都将被选中。
- 使用 <kbd>Ctrl+Shift</kbd>+左键单击在已选定文件的基础上添加一个系列。
- 单击文件列表的空白部分（即不在某个文件上）以取消选择所有文件。
- 单击文件列表的空白部分，并在按住按钮（在此过程中）将鼠标移至外面拖出选择矩形。所有被你拖拽矩形的覆盖文件都将被选中。
- 单击以拖拽选择矩形并保持按住 <kbd>Ctrl</kbd>，任何现有选择都不会受到影响。此外，你拖拽覆盖的文件也会切换其选择状态。
- **中间**单击某个文件以切换其选择状态（相当于 <kbd>Ctrl</kbd>+左键单击）。你还可以使用中间按钮拖出一个选择矩形，该矩形会切换你拖拽覆盖文件的选择（相当于 <kbd>Ctrl</kbd>+左拖动）。
- 你还可以使用右键拖出一个选择矩形；在释放按钮后，将对此所有选定项显示上下文菜单。

##### 使用键盘选择文件

- <kbd>Ctrl+A</kbd> 是在列表中选择所有项的默认热键（与 **编辑/全选** 命令相同）。
- <kbd>Ctrl+I</kbd> 转换列表中所有项的选择状态（与 **编辑/反选** 相同）。
- 当文件列表具有输入焦点时，光标键（<kbd>向上</kbd>/<kbd>向下</kbd>/<kbd>向左</kbd>/<kbd>向右</kbd>，加上 <kbd>上翻页</kbd>/<kbd>下翻页</kbd> 和 <kbd>主页</kbd>/<kbd>结束</kbd>）可用于在文件列表中移动选定位置（并取消所有其他项目的选定）。
- 您可以将 <kbd>Shift</kbd> 与光标键组合以使用键盘执行范围选择 - 将选定位置移动到该范围中第一个文件，然后按住 <kbd>Shift</kbd> 并使用光标键将该范围扩展到最后一个项目。
- 按住 <kbd>Ctrl</kbd> 键可以移动焦点矩形而不更改选定内容。您可以使用它来选择多个不连续的文件。例如，使用光标键将选择放置在某个文件上。然后按住 <kbd>Ctrl</kbd> 键并使用光标键将焦点矩形移动到另一个文件 - 请注意，第一个文件并未取消选定。
- 当某个项目具有输入焦点时，<kbd>空格</kbd> 将选中它。通过按 <kbd>Ctrl+空格</kbd>，您可以切换当前聚焦项的选择。
- <kbd>Ins</kbd> 切换当前项的选择，并自动将输入焦点移动到列表中的下一项。
- 键入部分文件名将激活 [搜索即键入](../the_lister/find-as-you-type_field.zh.md) 字段并将选择放置在与输入字符串匹配的第一个文件上。

##### 中键

请注意，有些鼠标驱动程序默认将中键映射到另一个功能 - 如果您发现中键单击不能按预期工作，请参阅 [FAQ](https://resource.dopus.com/t/how-to-make-logitech-mid-back-forward-buttons-work-in-opus/2972) 了解一些提示以解决该问题。您还可以将 Opus 配置为将一次中键单击视为双击中键，这允许您获取类似于 Web 浏览器 (例如，一次中键单击在新标签页中打开文件夹) 的行为。请参阅 **[File Displays/Mouse](/Manual/preferences/preferences_categories/file_displays/mouse/README.zh.md)** 偏好设置页面以了解有关它的详细信息。

#####增强模式

在增强模式下，鼠标和键盘选择在默认情况下略有不同（虽然可以通过 **[文件列表模式/增强模式](/Manual/preferences/preferences_categories/file_display_modes/power_mode/README.zh.md)** 配置页面修改鼠标行为）。

##### 在增强模式下使用鼠标选择

- 左键单击单个文件将转换该文件的选定状态，但不会影响任何其他项的选定状态。
- 您可以通过仅仅单击并向上或向下拖拽来选择一系列文件（即按住鼠标按钮并将鼠标光标向上或向下移动）。如果您单击的第一个文件已被选中，则向上或向下拖拽将取消拖拽文件的所有被选中。
- 默认情况下，单击文件列表的空白部分不会取消任何文件的选择。您可以通过单击文件列表的空白部分并在按住按钮的情况下进行拖拽来拖拽选择矩形 - 选择矩形将转换您拖拽的任何项目的选择状态。
- 请注意，因为向上或向下拖拽用于选择文件，所以拖放操作只能通过向左或向右拖拽来启动。

##### 在增强模式下使用键盘选择

-增强模式主要是一个基于鼠标的界面，默认情况下，增强模式的文件列表不在“键盘模式”，所以按下光标键只会滚动列表（如果可以滚动）而不会选择任何文件。
- 按键 <kbd>Ctrl</kbd> 会在文件列表中切换键盘模式。在键盘模式下，会显示一个焦点指示器，光标键会将焦点指示器从一个文件移动到另一个文件（虽然它们本身不会导致任何文件被选中）。
- 在键盘模式下按 <kbd>空格</kbd> 会转换当前显示焦点指示器的文件的选择状态。
- 在键盘模式下，您可以通过按住 <kbd>Shift</kbd> 键并使用光标键移动焦点指示器来选择一系列文件。按 <kbd>Shift</kbd> 键时的第一个文件的状态决定应用的选择状态 - 如果第一个文件尚未选中，则该系列中的所有文件都将被选中，反之亦然。
- 当使用 <kbd>Shift</kbd> 范围选择时，反方向将撤消您刚才应用的选择。例如，如果您按 <kbd>Shift+向下</kbd> 四次以选择前四个文件，然后（在仍然按住 <kbd>Shift</kbd> 的情况下）按 <kbd>向上</kbd> 两次，则最后两个选定文件将被取消选择。
- <kbd>Ctrl+A</kbd> 和 <kbd>Ctrl+I</kbd> 的作用与其他视图模式中的作用相同（参见上文），[搜索即键入](../the_lister/find-as-you-type_field.zh.md) 字段亦然。

##### 增强模式选择是持久的

增强模式的默认行为是文件选择是持久的（也就是说，文件不会自动取消选中 - 您必须手动取消其选中）。在其他文件列表模式中，您可以简单地单击一个空白区域以取消所有文件的选中，但在增强模式下：

- 您可以按 <kbd>Ctrl+A</kbd>，然后按 <kbd>Ctrl+I</kbd>（全选，然后反选）以取消所有文件的选中，或
- 使用 **[自定义模式](/Manual/customize/README.zh.md)** 将 `选择无` 命令添加到您的工具栏（例如，在 **编辑** 菜单中）。这未包含在默认工具栏集中，但如果您要使用增强模式，则可以手动添加它并为其分配一个热键。
更多信息：  
[单击模式](/Manual/basic_concepts/selecting_files/selecting_with_the_mouse_and_keyboard/single-click_mode.zh.md)  
[复选模式](/Manual/basic_concepts/selecting_files/selecting_with_the_mouse_and_keyboard/checkbox_mode.zh.md)