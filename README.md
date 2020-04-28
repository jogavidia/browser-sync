# browser-sync
How to make your browser sync while making changes in your files on the root folder or sub-folder

## STEPS:
* Create a folder on your desktop ``` $ mkdir <folderName> ```
* Create your index.html file ``` $ touch <fileName> ```
* Access the folder through the command line (Terminal) ``` $ cd <folderName> ```
* Use ``` $ npm init ``` to create package.json file 
* Enter the following command ``` $ npm i browser-sync ``` to install browser-sync package
* Enter the following command to verify if browser-sync was installed: ``` browser-sync --help ```
* Now you need to enter the following command to autorefresh your browser: ``` $ browser-sync start --server --files "*.*" ```
* Here we have an issue, it will refresh only when you save a file that is inside the root folder, we need a new command to refresh when you make a change and save a file inside a sub-folder, so enter: ``` $ browser-sync -w ```
* You are done
