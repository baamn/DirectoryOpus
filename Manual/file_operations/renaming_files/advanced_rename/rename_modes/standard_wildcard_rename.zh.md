# 标准通配符重命名

*标准通配符重命名* 模式可让您使用一个简单的通配符系统批量重命名文件。\* 字符（星号）用来指定现有文件名要保留在新名称中的一个或多个部分。

![](/Manual/images/media/13/standard_rename.png)

在上面的示例中，可以看到原始文件名有一部分混合了 *Img\_* 和 *IMG\_* 前缀，并且文件扩展名也混合了大小写。

*img\_\*.jpg* 的 **旧名称** 模式告诉 Opus 匹配以 *img\_* 开头且以 .jpg 结尾的任意文件名（大小写无关，因为未启用 **区分大小写** 选项）。模式中的 \* 用于标记将延续到新名称的文件名部分。**忽略扩展名** 选项已关闭，以便通配符可以在包含文件扩展名的整个文件名上操作。

只要 **旧名称** 字段中的实例数至少和新名称一样多，您可以在模式中使用任意多个 \* 字符的实例。例如，如果您想保留上述示例中文件扩展名的格式，则可以为 **旧名称** 模式指定 *img\_\*.\**，为 **新名称** 模式指定 *IMG\*.\**。

如果您想更改指定字符串的顺序，就无法使用该系统（因为一个星号看起来非常像另一个星号）——要做到这一点，您需要使用 *[正则表达式](regular_expressions.zh.md)* 模式，该模式可让您按编号引用指定字符串。