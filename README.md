# How to install NPM package browser-sync using Terminal on Mac
How to browser-sync while saving the changes made in your project's files, using the Terminal command line, without refreshing your browser manually. 

## Getting Started

### Creating the project's files via Terminal

1. Create a folder on your desktop:

``` $ mkdir <folderName> ```

2. Access the folder through the command line (Terminal):

``` $ cd <folderName> ```

3. Create your index.html file:

``` $ touch <fileName> ```

Once you have your project folder with corresponding files in it, follow these steps:

### Steps
4. To create package.json file (it's optional to fill all questions):

``` $ npm init ```

5. Install browser-sync package:

``` $ npm i browser-sync ```

6. If browser-sync was installed the following command will display the current version of the package:

``` browser-sync --version ```

7. Enter the following command to launch your browser (the browser will auto-refresh and display the changes you have made and saved):

``` $ browser-sync start --server --files "*.*" ```

8. If you have files in subfolders, enter the following command to display changes made in subfolders files as well:

``` $ browser-sync -w ```

8. In case, you have your index.html in a sub-folder:

``` browser-sync start --server "build" -w ``` * where "build" is the sub-folder that contain index.html
