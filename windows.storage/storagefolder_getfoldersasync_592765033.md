---
-api-type: winrt method
---
 When you use the **DefaultQuery** option with any folder, the query returns a list of subfolders in the file system.
 When you use an option other than **DefaultQuery** with a library folder, the query returns a list of virtual folders that represent containers for files from the subfolders of the current folder. (Files from the current folder are not included.) The files are grouped into virtual folders based on the specified value from the [CommonFolderQuery](../windows.storage.search/commonfolderquery.md) enumeration. For example, if you specify **GroupByMonth**, the query returns a list of virtual folders such as `July 2014`, `August 2014`, and `September 2014`.