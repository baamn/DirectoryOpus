# Blob

A **Blob** object represents a chunk of binary data. Scripting languages like *VBScript* and *JScript* have no built-in support for binary data - this object can be used to allocate a chunk of memory and manipulate it in a similar way to low-level languages like C. You can use **Blob** objects in conjunction with the **[File](file.md)** object to read or write binary data from or to disk files.

**Blob** objects are convertible to and from two types of ActiveX arrays - a *SAFEARRAY* of type *VT_UI1* (known as an **array**) and a *SAFEARRAY* of type *VT_VARIANT*, with each variant holding a *VT_UI1* (known as a **VB array**). You can initialize a **Blob** with either of these two types of array (either when creating it via the **DOpusFactory.Blob** method or with the **Blob.CopyFrom** method), and you can also convert a **Blob** back to an array with the **ToArray** and **ToVBArray** methods. Support for these array types is dependent on the scripting language.

You can read and write individual bytes within the **Blob** by indexing the byte offset starting from 0. For example, *my_blob(5) = 128* would set the value of the sixth byte in the blob to 128.

| Property Name | Return Type | Description |
| --- | --- | --- |
| size | *object:***[FileSize](filesize.md)** | Returns a **[FileSize](filesize.md)** object representing the size of this **Blob** in bytes. |

| Method Name | **Arguments** | Return Type | Description |
| --- | --- | --- | --- |
| Compare | \<<Blob:source>\>  <br />\<int:to\>  <br />\<int:from\>  <br />\<int:size\> | *int* | Compares the contents of this **Blob** against another **Blob** (or array). By default the entire contents of the two blobs are compared. The optional parameters that let you configure the operation are:<br /><br />to - specifies the byte offset within this **Blob** to compare against. Defaults to 0.  <br />from - specifies the byte offset within the source **Blob** to compare with. Defaults to 0.  <br />size - specifies the number of bytes to compare. Defaults to the full size of the source **Blob**.<br /><br />The return value is **0** if the two blobs are the same. A value of **-1** indicates this blob is less than the other blob, and **1** indicates this blob is greater than the other blob. |
| CopyFrom | \<<Blob:source>\>  <br />\<int:to\>  <br />\<int:from\>  <br />\<int:size\><br /><br />*or*  <br />   <br />\<string\>  <br />\<type\> | *none* | Copies data from the source **Blob** (or array) into this **Blob**. By default the entire contents of the source **Blob** will be copied over the top of this one. The optional parameters that let you configure the operation are:<br /><br />to - specifies the byte offset within this **Blob** to copy to. Defaults to 0.  <br />from - specifies the byte offset within the source **Blob** to copy from. Defaults to 0.  <br />size - specifies the number of bytes to copy. Defaults to the full size of the source **Blob**.<br /><br />As well as copying from another **Blob**, you can use this method to initialise a **Blob** from a string. By default the **Blob** will be set to the Unicode form of the string; if you pass **"utf8"** as the second parameter it will initialise the **Blob** with the UTF8-encoded form of the string.<br /><br />If this **Blob** is not currently large enough to contain the copied data it will be resized automatically. |
| Find | \<<Blob:search>\>  <br />\<int:from\>  <br />\<int:size\> | *object:***[FileSize](filesize.md)** | Searches the contents of this **Blob** for the data contained in another **Blob** (or array). By default the entire contents of this **Blob** are searched. The optional **from** parameter lets you specify the starting position for the search, and the optional **size** parameter lets you specify the length of data in this Blob to search through.  <br />The return value is -1 if the search data were not found, otherwise the offset from the start of the **Blob** data is returned. |
| Free | *none* | *none* | Frees the memory associated with this **Blob** and resets its size to 0. |
| Init | *none* | *none* | Initialises the contents of the **Blob** (every byte within the blob will be set to 0). Equivalent to *Set(0)*. |
| Resize | \<int:size\> | *none* | Resizes the **Blob** to the specified number of bytes. |
| Reverse | *none* | *none* | Reverses the contents of the **Blob**. |
| Set | \<byte:value\>  <br />\<int:to\>  <br />\<int:size\> | *none* | Sets the contents of the **Blob** to the specified byte value (every byte within the blob will be set to that value). By default the whole **Blob** will be affected. The option *to* parameter lets you specify a byte offset to start at, and the optional *size* parameter lets you control the number of bytes affected. |
| ToArray | \<int:from\>  <br />\<int:size\> | SAFEARRAY of  <br />VT_UI1 | Converts the contents of this **Blob** to a *SAFEARRAY* of type *VT_UI1*. By default the entire contents of the **Blob** will be copied to the array. The optional parameters that let you configure the operation are:  <br />from - specifies the byte offset within the source **Blob** to copy from. Defaults to 0.  <br />size - specifies the number of bytes to copy. Defaults to the full size of the source **Blob**. |
| ToVBArray | \<int:from\>  <br />\<int:size\> | SAFEARRAY of  <br />VT_VARIANT | Converts the contents of this **Blob** to a *SAFEARRAY* of type *VT_VARIANT*. Each variant in the array contains a *VT_UI1*. By default the entire contents of the **Blob** will be copied to the array. The optional parameters that let you configure the operation are:<br /><br />from - specifies the byte offset within the source **Blob** to copy from. Defaults to 0.  <br />size - specifies the number of bytes to copy. Defaults to the full size of the source **Blob**. |
