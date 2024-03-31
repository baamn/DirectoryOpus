# Directory Opus 13 - 详细发行说明

# 深色模式和外观

- 深色模式：
  - 内置，官方深色主题。
  - 如果 Windows 处于深色模式，自动使用。可以通过菜单或配置切换。
  - 支持为整个用户界面重新着色，包括对话框、提示和以前无法修改的面板以及网络和回收站等特殊文件夹。
  - 在深色模式下启用深色标题栏（Windows 10 及更高版本）。
  - 脚本对话框会自动变成深色。在大多数情况下无需更改代码。
  - 深色和浅色模式存储单独的颜色设置。你可以自定义两者并在它们之间切换（手动或通过 Windows 设置自动切换）。
  - 图标集可以为同一图标指定替代的深色和浅色图像。
  - *命令：* `Set DARKMODE`
  - *脚本：* 深色/浅色更改有新的脚本事件。（参见 [杂项脚本](misc_scripting.zh.md)）。
- 颜色：
  - 不限于“深色”和“浅色”。可以使用任何想要的颜色！
  - 对颜色配置进行了大规模修改。包括超过 700 种可配置颜色和相关选项。
  - 更改 Opus 中按钮、复选框、文本字段和其他标准控件的颜色。（不会影响其他进程。）
  - 大多数颜色更改会在你进行更改时生效，无需离开颜色选择器或单击应用。（你仍可以单击取消来撤消任何未保存的更改。）
  - 配置中的预览有助于理解不同颜色的作用并确保颜色组合可读。
  - 增强颜色选择器：右键菜单和拖放使编辑更轻松，并允许在深色和浅色模式之间重置或复制各个颜色。
  - 更严密地控制工具栏和菜单颜色（包括路径字段和地址栏），以及状态栏颜色、边框和调整大小控制柄。
  - 现在可以配置“热”文件背景的不透明度。
  - 现在每种颜色都有一个名称。命名颜色可用在状态栏等位置，而不是固定的 RGB 值。使用右键菜单即可获得它。
  - 命名颜色可以用在状态栏、信息提示和脚本日志输出中。例如 `<#%error_text>这通常是红色的</#>`。
  - Web 颜色名称也起作用。例如 `<#@magenta>...</#>` 或 `<font color="oldlace" bgcol="plum">...</#>`。
  - 可以使用 `<#xxxxxx #xxxxxx>` 作为设置文本和背景颜色的快捷方式，而不是 `<font color=#xxxxxx bgcol=#xxxxxx>`。
- 字体：
  - 更多可配置字体，包括配置、进度对话框、弹出提示、工具提示等使用的对话框字体。
  - 字体更改会在你进行更改时生效，无需单击应用。（例外：退出/重启后对话框字体更改。）
  - 可以定义一个默认工具栏字体，而不是必须为每个工具栏单独指定字体。（各个工具栏仍然可以覆盖默认值。）
  - 可以相对于主工具栏字体调整菜单标题字体大小。
  - 地址栏的字体也可以应用于它的工具栏以及“静态标题”模式。如果使用，则会覆盖更通用的工具栏字体。
  - 可以相对于主标签字体调整缩略图标签下尺寸等文本的大小。
  - 通过 Ctrl + 鼠标滚轮（或类似的热键）调整文件夹标签中的字体大小时，会显示一个“设为永久”按钮，将其保存为新的默认值（就像在配置中编辑大小一样）。
  - 可以为不同的文件夹配置不同的字体。
  - *命令：* `Set FONTSCALE`-- 新关键字“details”、“thumbnails”和“all”允许你指定要影响的视图模式。（默认情况下调整当前模式。）
- 主题：
  - 修改后的主题系统。现在位于配置中，紧挨着颜色本身。
  - 支持深色和浅色主题，在加载时更改模式。
  - 检查旧版本中的旧主题以确定它们看起来是浅色还是深色。（可以推翻。）
  - 主题现在可以包括颜色混合设置和大多数其他外观选项。
  - 主题不再包括声音和工具栏图标。（那些可以单独共享，很少被使用，并且往往会导致主题包含旧副本。）
  - 内置默认主题。还原为默认颜色和字体更加容易。
  - 在应用新主题之前选择保存备份主题，这样如果你不喜欢更改，可以恢复到原来的样子。
  - 清理按钮，可以删除旧主题备份和未使用的背景图像。
  - 现在可以双击 .dlt 主题文件将它们添加到你的配置中。
  - 命令：
    - `Prefs THEMENAME=!defaultdark THEMELOAD=all`-- 加载内置默认深色主题。
    - `Prefs THEMENAME="My Theme" THEMELOAD=all`-- 加载你制作或从网上获取的主题。
    - `Prefs THEMEIMPORT`-- 将所选主题文件复制到配置文件夹中。（与双击它相同。）
- Windows 11：
  - 选项，可在 Windows 11 上更改窗口角样式（普通圆角、较小圆角或方形）。
  - 文件夹标签现在默认为圆角（就像它们在 Windows 7 上一样），但可以覆盖这一点。（你也可以在较旧的操作系统上使用圆角选项）。
  - 当它们与底部窗口角落重叠时，过渡动画运行得更好。
  - 默认情况下，即使在浅色模式下，也会在 Opus 中覆盖用于滚动条和菜单的可视样式，因为 Microsoft 的普通样式在我们看来是不可接受的，不仅在美观方面，还在可用性方面。如果你不同意，可以更改此设置。
- 杂项：
  - 列表和工具栏的背景图像现在可以设置其 alpha/透明度级别。
  - 新的背景图像模式可以在不失真的情况下进行拉伸：
    - 宽高比填充使图像足够大，以覆盖区域的宽度或高度而不裁剪。
    - 宽高比填充使图像足够大，以覆盖整个区域，并在需要时裁剪图像。
  - 用于切换设置的菜单项通过复选标记覆盖物更清楚地显示其状态。
  - 新选项，“选择矩形重叠”：
    - 让你选择在使用视觉样式时相邻的已选项目是否应该略微重叠。
    - 关闭此选项，如果你不喜欢已选文件之间有线条，而更喜欢一个实心的颜色块。
    - （过去，你可能为此使用了“额外的行距”选项。我们建议现在改用此选项。）