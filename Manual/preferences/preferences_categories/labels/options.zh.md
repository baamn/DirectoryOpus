# 选项

此页面包含与 [标记](/Manual/file_operations/labels.zh.md) 相关的常规选项。

##### 在文件系统中启用标记存储

Opus 具有两种方式来存储分配给特定文件或文件夹（与通配符或基于过滤器的标记相对）的标记。

- 在文件系统中：在 NTFS 格式化的驱动器（现今最常见的类型）上，标记信息与实际文件本身存储在备用数据流中。这样做的好处是，复制、移动或重命名文件时，标记也会随之移动。
- 在配置中：在其他文件系统上，或如果文件系统中存储标记的选项已关闭，标记文件的完整文件名和路径将存储在 Opus 配置中。这意味着，如果你移动已标记的文件，标记将不会随之移动。

如果 **启用文件系统中的标记存储** 已启用，Opus 将尝试将标记存储在 NTFS 数据流中，并且仅在必要时回退到配置。如果发生这种情况，**如果标记无法存储在文件系统中，发警告** 将使 Opus 向你展示警告。

##### 将通配符和过滤器标记应用于明确标记的文件

默认情况下，明确应用的标记将覆盖通配符标记，但此选项允许通配符标记堆叠在明确指定的标记之上。