# PureBasic DLL Icons Templates

A set of templates that allow you to compile DLL filesthat contains icons with PureBasic using .rc files.


## How does it work

When compiling a program, you can choose to use one or more .rc file(s) in the "Resources" tab in the compiler options.

These template allow you to either see how to include one or more icon(s) in your executable or DLL, or how to compile multiple DLLs by using one project and multiple build options.

More informations about "Resource Definition Statements" can be on found on [docs.microsoft.com](https://docs.microsoft.com/en-us/windows/desktop/menurc/resource-definition-statements).<br>
And in the [.rc file](Single/resources.rc) in the "Single" template.


## Templates

### Single Template

When compiling [SingleDLLIcon.pb](Single/SingleDLLIcon.pb), the [.rc file](Single/resources.rc) will point to a couple of icons contained in the "[icons/](Single/icons/)" folder.

The resulting DLL will contain 2 icon groups that are declared using numerical IDs and one that is declared using a unique name.<br>

### Project Template

When compiling [ProjectDLL.pbp](Project/ProjectDLL.pbp), you can either select to build one or all targets.<br>
Each target compiles an empty .pb file named [Empty.pb](Project/Empty.pb) with a different .rc file contained in the "[icons/](Project/icons/)" which then points to icons contained in distinct subfolders.

The resulting DLL will be put in the "[icons/](Project/icons/)" directory.


## Useful Resources

* [Resource Hacker](http://www.angusj.com/resourcehacker/) / [7-Zip](https://www.7-zip.org/)<br>
Allows you to easily see what is inside of DLL, executables, ...


## Credits

The icons used in the templates are the property of Microsoft.<br>
They come from Windows 98 and 10.


## License

[WTFPL](LICENSE)
