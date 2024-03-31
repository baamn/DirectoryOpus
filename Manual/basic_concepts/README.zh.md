# 基本概念

在 Opus 中有一些可能与您使用过的其他文件管理器不同的概念。虽然我们试图避免使用术语或极客术语，但本帮助文件中使用了一些您可能不太熟悉的术语；我们建议快速浏览“基本概念”部分，以熟悉其中的一些概念。

- **[列表](/Manual/basic_concepts/the_lister/README.zh.md)**：列表可能是您所说的 Opus 的“主窗口”——在传统的文件管理器中，它们是主窗口。列表（此名称有历史渊源）包含文件列表（其中显示目录的内容）、文件夹树（以树结构显示您的文件系统以简化导航）、工具栏以及各种可选“窗格”，例如预览窗格、元数据窗格等。您可以打开任意数量的列表。
- **[资源管理器替换](/Manual/basic_concepts/explorer_replacement.zh.md)**：Opus 具有以资源管理器替换模式操作的选项。在此模式下，通常会导致打开资源管理器窗口的大多数操作（按 <kbd>Win+E</kbd> 键、双击桌面上的图标等）将改为打开 Opus 列表。这是我们建议您运行的模式。
- **[源和目标](/Manual/basic_concepts/source_and_destination.zh.md)**：除了您可能习惯使用的传统复制/剪切/粘贴文件管理方法之外，Opus 还提供了一种替代方法，该方法使用“源”和“目标”文件夹的概念。此替代方法无需浏览到您要复制的文件、将其复制到剪贴板，然后浏览到目标文件夹并将其粘贴，而是允许您同时显示源文件夹和目标文件夹（使用两个独立的列表或使用处于双栏模式的单个列表）并在一项操作中将文件从一个复制到另一个。
- **[选择文件](/Manual/basic_concepts/selecting_files/README.zh.md)**：有多种方法可以选择要操作的文件；除了使用键盘或鼠标的标准方法外，您还可以使用文件名上的通配符匹配来进行选择，或使用过滤器按属性或元数据来选择文件。Opus 还支持复选模式，该模式允许您操作文件（通过双击或拖放）而不影响其选择状态。
- **[搜索和过滤](/Manual/basic_concepts/searching_and_filtering/README.zh.md)**：搜索是定位当前查看位置可能不存在的文件或文件夹的过程——Opus 支持 Windows 搜索以进行索引搜索，以及它自己的强大搜索引擎，它允许您构建复杂查询以查找基于属性和元数据以及文件名的文件。过滤是隐藏或屏蔽当前查看位置的文件和文件夹的过程。Opus 提供了多种方法来执行此操作——最简单的方法是过滤栏，它允许您只需在文件列表中键入通配符模式即可快速显示文件的子集。
- **[排序和分组](/Manual/basic_concepts/sorting_and_grouping/README.zh.md)**：文件列表可以按一个字段或多个字段进行排序，您还可以按任何字段对文件列表进行分组，并具有可折叠组。
- **[文件夹格式](/Manual/basic_concepts/folder_options/README.zh.md)**：这是一个强大的系统，允许您确切控制文件夹的显示方式——您可以定义视图模式、排序和分组选项等，并将其永久分配给文件夹、文件夹及其子项、基于磁盘类型的“类型”的文件夹或文件夹内容，或使用通配符的多个文件夹。
- **[可扩展文件夹](/Manual/basic_concepts/expandable_folders.zh.md)**：Opus 允许您在主文件列表中展开文件夹，就像在树中一样，因此您可以在不更改位置的情况下查看子文件夹的内容。
- **[平面视图](/Manual/basic_concepts/flat_view.zh.md)**：平面视图系统允许您“折叠”当前位置的所有子文件夹的内容，并使它们看起来好像它们都在同一物理位置一样。平面视图可以显示所有子文件夹的真正平面列表，或者可以以层次结构显示子文件夹的内容。
- **[文件夹大小](/Manual/basic_concepts/folder_sizes.zh.md)**：查看文件夹的大小就像查看文件的大小一样。Opus 与 [voidtools 的 Everything](https://voidtools.com) 集成以便快速计算文件夹大小。
- **[虚拟文件系统](/Manual/basic_concepts/virtual_file_system/README.zh.md)**：真正的文件系统是您存储文件和文件夹的位置——通常包含在您的硬盘驱动器、USB 驱动器等中。虚拟文件系统是 Opus 用来描述没有以这种传统方式存储的文件系统的概念。例如，文件集合是一个虚拟文件系统，因为它们是存储在传统媒体上的文件集合，而不是它们本身的基础文件夹。有一些概念是特定于特定虚拟文件系统的——文件集合、库、压缩包和 FTP 都在此部分中进行了描述。