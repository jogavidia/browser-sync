# How to install NPM package browser-sync using Terminal on Mac
How to make your browser sync while making changes in your project's files without refreshing your browser manually. 

## Creating the project's files via Terminal

1. Create a folder on your desktop ``` $ mkdir <folderName> ```
2. Access the folder through the command line (Terminal) ``` $ cd <folderName> ```
3. Create your index.html file ``` $ touch <fileName> ```

Once you have your project folder with corresponding files in it, follow these steps:

## Steps:
4. Use ``` $ npm init ``` to create package.json file (it's optional to fill all questions).
5. Enter the following command ``` $ npm i browser-sync ``` to install browser-sync package
6. Enter the following command to verify if browser-sync was installed: ``` browser-sync --help ```
7. Now you need to enter the following command to autorefresh your browser: ``` $ browser-sync start --server --files "*.*" ```
8. Here we have an issue, it will refresh only when you save a file that is inside the root folder, we need a new command to refresh when you make a change and save a file inside a sub-folder, so enter: ``` $ browser-sync -w ```
