# GIT sync plugin

[中文](./README_zh_CN.md)

GIT Sync plugin is a plugin developed by `xstarling` for data synchronization between local files and GITHUB and GITEE code repositories.

## Changelog
#### Historical version update
  * please click to view the all document: [Changelog](https://kdocs.cn/l/caGt3BWn9r5G?linkname=ihqHHyiJ56)

#### Current version update
  1. When exporting a markdown file from Siyuan Notes, a title will be added by default.
  2. A new "Refresh Work Tree" button has been added. Manually click it to trigger the refresh of the work tree, avoiding the system restart caused by refreshing the work tree after each synchronization.
  3. The error prompt information and log recording of the synchronization plugin have been optimized.
  4. Fixed the issue where modifying the note format during synchronization would result in empty remote data.
  5. The settings interface has been optimized to be compatible with both cloud disk and git platform synchronization (the specific data synchronization is still under development).

## Feature list
> features list: [click here](https://kdocs.cn/l/caGt3BWn9r5G?linkname=k7VAb4Wx5b)
+ **🚧 Large File synchronization (under development)**
  + 🚀 Combine git warehouse with Baidu web disk and Ali web disk, etc., to realize large file upload synchronization
+ **🚧 Function menu**
  + 🚀 Start Synchronization: Initiate data synchronization between local and remote
  + 🚀 Refresh Worktree: If after synchronization, newly added local files show the issue of "ID not found!", the problem can be resolved by refreshing the worktree.
  + 🚀 Synchronization range:
    + 👉 Workspace: In the workspace, important data is synchronized to the git repository
    + 👉 data directory: In the workspace, data files stored in the 'data' directory are synchronized to the git repository
    + 👉 Note files: Source Han Sans Notes files in the 'data' directory and 'asset' image resource files in the workspace

  + 🚀 Synchronization policy:
    + 👉 Auto-sync: The system 's auto-sync policy enables file comparison synchronization
    + 👉 Manual synchronization: The pop-up box allows users to manually [Cloud override local], [Local override cloud], and check whether to force override or not
    + 👉 Cloud Overwrite Local: Non-mandatory overwrite mode, overwrite local from a remote location, generate conflicting documents if document conflicts (pops up if you check generate conflicting documents option)
    + 👉 Local Overwrite Cloud: Non-mandatory overwrite mode, overwrite from local to remote, generate conflicting documents if document conflicts occur (pops up if you check generate conflicting documents option)

  + 🚀 Note format:
    + 👉 Source Han Notes: Files synchronized to the remote repository are in Source Han format notes (Note files only, other files not supported)
    + 👉markdown: Files synchronized to the remote repository are notes in markdown format (note files only, other files not supported)


  + 🚀 Synchronization mode:
    + 👉 Automatic synchronization: Data is periodically synchronized to the git repository according to the interval set on the setup screen
    + 👉 Manual synchronization: synchronization is performed only once when the system is started. Synchronization is not triggered when the system is shut down
    + 👉 Full manual synchronization: Synchronization is not triggered when the system is started or shut down. You need to manually click the "Start synchronization" button to synchronize
  + 🚀 Synchronization history:
    + 👉 Local commit: After selecting this option, the system will query all commit records in the remote git repository up to the last commit on the local device
    + 👉 Remote commit: After selecting this option, the system will query all commit records of the remote git repository up to now
    + 👉 File search: Users can search for submission records containing the corresponding file by filtered notebook, file ID or path, and time range
    + 👉 Submit node: Hover over the submit node in the submit history in the sidebar and a summary of the submission will be displayed
    + 👉 Submit file: After clicking Submit Node, a list of files for the submitted node will be displayed on the right side of the Sync History panel
    + 👉 file comparison: After clicking [Submit file], the system will open the file comparison panel, and display the file content of the submitted node and the local file content with the same name, so that users can compare the file content differences
    + 👉 Rollback file: Click [⤴︎] in the submission list. The file in the submission history will be downloaded to the local file and overwrite the local file content
    + 👉 Download file: there is a "↓" in the submission file list. After you click it, the file in the submission record will be downloaded to the local, and the pop-up box on the right will prompt you to download the path
+ **🚧 Settings screen**
  + 🚀 User information: including [git repository platform], [git repository address], [git repository name], [git repository branch name], [git platform user name], [Email], the plug-in system can be used only after users fill in the information correctly and completely according to their platform information
  + 🚀 Ignore files: Enter the path or name of the file that does not need to be synchronized. The system automatically ignores related files during synchronization
  + 🚀 token /SSH: Users log in to their github or gitee repositories and generate their own tokens that can be used by the system to remotely access git repositories
  + 🚀 Generate conflict documents when synchronizing conflicts:
  + 🚀 Sync range: see 【 Function menu 】-> 【 Sync Range 】
  + 🚀 Sync mode: see 【 Function menu 】-> 【 Sync Mode 】
  + 🚀 Synchronization interval: The system synchronization interval when the user sets [automatic synchronization]
  + 🚀 Last Submitted SHA value: Displays the hash value of the last submitted record. It cannot be modified
  + 🚀 Last submitted time: Displays the last submitted time on the local PC. It cannot be modified

## Instructions for use

> detailed instructions please click: [GIT synchronization plugin instructions](https://kdocs.cn/l/caGt3BWn9r5G?linkname=ArymAS7rZm)
## Precautions
> [GIT sync plug-in - disclaimer](https://kdocs.cn/l/caGt3BWn9r5G?linkname=hMZxlMSs8z) <br>
The software (hereinafter referred to as "the Software") is developed by an individual and aims to provide users with the function of synchronizing note data. By using the Software, you signify that you have read, understood and agreed to the entire contents of this disclaimer.
+ 💻1. Data security
  + 🚀 As this plug-in is developed by individuals, system testing may be limited, **users are advised to enable the snapshot function of Siyuan Notes or backup data regularly** in case of data loss.
  + 🚀 Users should understand and accept that **The use of this plug-in may involve unforeseen risks**, such as data loss, corruption or synchronization errors. To the extent permitted by applicable law, Users should assess the risks of use on their own.
+ 💻2. Privacy and Permissions
  + 🚀 The software does not actively collect, store or share users' personal information, and all data processing is carried out locally on user devices or in Git code repositories authorized by users.
  + 🚀 Users should properly manage their Git accounts, API tokens, and related credentials and be responsible for their data security and access rights.
+ 💻3. Risk of use
  + 🚀 The user's use of the Software is at its own risk, and the Developer shall not be liable for any direct or indirect losses arising from the use of the Software, including but not limited to data loss, account blocking, equipment damage or third-party liability.
+ 💻4. Others
  + 🚀 other considerations, please see the plugin Settings interface or disclaimer 】 【 in 】 [GIT sync plug-in - disclaimer](https://kdocs.cn/l/caGt3BWn9r5G?linkname=hMZxlMSs8z)

## Project management
1. The features list: [click here](https://kdocs.cn/l/caGt3BWn9r5G?linkname=k7VAb4Wx5b)
2. The directions for use: [click here](https://kdocs.cn/l/caGt3BWn9r5G?linkname=ArymAS7rZm)
3. Disclaimer: [click here](https://kdocs.cn/l/caGt3BWn9r5G?linkname=hMZxlMSs8z)
4. The development progress: [click here](https://kdocs.cn/l/caGt3BWn9r5G?linkname=Emg3LXgDJp)
5. Feedback communication: [👥 siyuan group - the git plug-in feedback (QQ group: 1015180920)](https://kdocs.cn/l/caGt3BWn9r5G?linkname=Ij7mC9wG6q)
6. Common q&a: [FAQ document](https://kdocs.cn/l/cf8qSfWUdi1O)