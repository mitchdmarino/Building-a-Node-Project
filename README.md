# Building a Node Project

## Step-by-step guide on building a Node project from scratch.
___
### Getting set-up 

1. Make sure Node is installed. 
* Go to terminal, and run the command: 
```
node -v
```
    
* If Node is not installed, install by running the command 

```
brew install node
```
    
2. Create a new folder for your node project. 
    * In terminal, 
    
    ```
    mkdir Name_of_Node_Project
    ```

    * Change directories into that folder 

3. Initialize NPM inside the folder by running the command: 

```
npm init
```
    
* Note: There will be a few properties you can enter values for. You can enter values based on your project needs, or just leave them as default by pressing 'return' on each one. To skip this step, substitute the above command with : 
   
    ```
    npm init -y
    ```

4. At this point, a new file called package.json should be created. The values from the previous step will be stored here. It is essentially a settings file, and you can edit it at any time. 

5. Your entry point file will be titled 'index.js', unless specified otherwise in step 3. Create this file by running the command: 

```
touch index.js
```

6. To run the code in your entry point file, run the following command: 

```
node index.js
```

        * TIP: install nodemon NPM and run the command 
        ```nodemon index.js``` 
        to automatically rerun your code every time changes are saved. 

7. Your new Node project is now set up! 

___

### Node Modules 

Modules allow us to export code from a file (module), and import it into other files. Modules are useful for achieving certain goals and can be easily reused and shared. 

1. To create a module, create a file called Module_name.js. Within the file, you can add code to export by coding: 

```
module.exports.KEY=(VALUE)
```

* Now, the module.exports object has a key-value pair.

2. In your index.js file, you can import the module code by typing: 

```
const Module_Name = require('Module_File_Path`)

Module_Name.KEY
^^^ this will call the key we defined in the module. 
```
 * Note: you can define more than one key value pair in each module. 

 3. Node has many Built-In Modules that are super useful. You can use them in the same way as defined in part 2, but don't need to define them in their own file. Look up some built in modules and see what they can do! 

 ___

 ### Node Packages

 Node packages are essentially just third-party modules. 

 * There are hundreds of thousands of such modules out there, available as NPMs. 
* Find the NPM that is useful for you, get familiar with it's functions and syntax, and install it in your project folder! 

    * Note: NPMs can be installed globally (where can be accessed by any project) or locally, only within certain projects. 

On a final note, make sure to include a .gitignore file. Inside the file, enter 'Node_modules'

When uploading to github, we don't need to upload the Node Modules since they can be accessed on the internet already. We can easily reinstall the appropriate packages. 


