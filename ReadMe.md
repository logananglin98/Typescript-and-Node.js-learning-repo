# Typescript and Node.js Learning Repo

This repo is my way of learning TypeScript and how to integrate it with Node.js for building an exe. Using this for a final project in a computer security class. Feel free to use as a reference!

## How to set up Typescript and Node.js

'''
Setting up TypeScript with Node.js in Visual Studio Code on Windows 10 is a straightforward process. Follow these steps to get everything up and running:
Step 1: Install Node.js and npm

First, make sure you have Node.js and npm (Node Package Manager) installed.

    Download Node.js:
        Go to the official Node.js website and download the latest LTS version.

    Install Node.js:
        Run the installer and follow the instructions. It should install both node and npm globally.

    Verify Installation:
        Open a new terminal (Command Prompt or PowerShell) and run the following commands:

        bash

        node -v
        npm -v

        This should output the installed versions of Node.js and npm.

Step 2: Install TypeScript Globally

Next, you need to install TypeScript globally on your system using npm.

    Open your terminal and run:

    bash

npm install -g typescript

This will install TypeScript globally so you can use the tsc (TypeScript Compiler) command anywhere.

Verify TypeScript installation:

bash

    tsc -v

    This should output the installed version of TypeScript.

Step 3: Set Up Your Project

Now, create a directory for your Node.js project and set it up.

    Create Project Folder: Open a terminal and navigate to where you want your project. Create a new directory:

    bash

mkdir my-node-ts-project
cd my-node-ts-project

Initialize a Node.js Project: Inside your project folder, run the following to create a package.json:

bash

npm init -y

Install TypeScript as a Development Dependency: It’s a good idea to install TypeScript locally to your project as well:

bash

npm install --save-dev typescript

Install Type Definitions for Node.js (Optional but recommended): This helps TypeScript understand Node.js globals like require, process, etc.

bash

    npm install --save-dev @types/node

Step 4: Set Up TypeScript Configuration

Now, you need a TypeScript configuration file to specify how TypeScript should compile your code.

    Generate tsconfig.json: Run the following command to create a default tsconfig.json file:

    bash

    npx tsc --init

    This will create a tsconfig.json file in your project with default settings. You can adjust the settings, but the basic options should work for most projects.

Step 5: Write Your TypeScript Code

Create a file named index.ts in your project directory.

typescript

// index.ts
console.log("Hello, TypeScript with Node.js!");

Step 6: Compile TypeScript

To compile your TypeScript code into JavaScript, run the following command:

bash

npx tsc

This will compile your index.ts file into an index.js file in the same directory (by default).
Step 7: Run the JavaScript Code

You can now run your compiled JavaScript file with Node.js:

bash

node index.js

You should see:

csharp

Hello, TypeScript with Node.js!

Step 8: Set Up VSCode for TypeScript Development

    Install VSCode if you haven’t already from Visual Studio Code website.

    Open your Project Folder in VSCode:
        Open VSCode and use File > Open Folder to select your project folder.

    Install Recommended Extensions:
        ESLint (for linting TypeScript)
        Prettier (for automatic code formatting)
        TypeScript (for TypeScript syntax support, this should be enabled by default)

    Configure VSCode to Use Local TypeScript Version:
        By default, VSCode may use the global version of TypeScript. To ensure it uses the local version (from node_modules), press Ctrl+Shift+P in VSCode and search for "TypeScript: Select TypeScript Version." Then choose "Use Workspace Version."

Step 9: Watch for TypeScript Changes (Optional)

If you want TypeScript to automatically compile your code whenever you change a .ts file, you can use the --watch flag.

Run this in your terminal:

bash

npx tsc --watch

This will keep TypeScript compiling your code in the background as you make changes.
Summary of Commands

Here’s a quick summary of the key commands you'll use:

    Install Node.js: Download Node.js
    Install TypeScript globally:

    bash

npm install -g typescript

Set up the project:

bash

mkdir my-node-ts-project
cd my-node-ts-project
npm init -y
npm install --save-dev typescript @types/node
npx tsc --init

Compile TypeScript:

bash

npx tsc

Run JavaScript with Node.js:

bash

    node index.js

This should get you up and running with TypeScript in Node.js using VSCode on Windows 10! Let me know if you need further assistance or run into any issues.
'''

## Resources

Setting up TypeScript to integrate with Node.js: https://medium.com/@daveahern/creating-a-node-executable-with-typescript-8cfb6b599fc9  
Running TypeScript in GitHub: https://code.visualstudio.com/docs/typescript/typescript-compiling

