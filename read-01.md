# Node Ecosystem, TDD, CI/CD

 - 1. **Why would you want to run JavaScript code outside of a browser?**
       - Running JavaScript without/outside a browser means you are using node.js technology to execute your JavaScript code. This type of usage of javascript typically refers to backend programming where your javascript code will interact with your database and can be used to create RESTful APIs.
 
 
 - 2. **What is the difference between a module and a package?**
       - "Java platform module system" 
         - A module is a named, self-describing collection of code and data. Its code is organized as a set of packages containing types, Java classes and interfaces; its data includes resources and other kinds of static information
         - A Java package is a technique for organizing Java classes into namespaces similar to the modules of Modula, providing modular programming in Java.


 - 3. **What does the node package manager do?**
       - Adapt packages of code for your apps, or incorporate packages as they are.
       - Download standalone tools you can use right away.
       - Run packages without downloading using npx.
       - Share code with any npm user, anywhere.
       - Restrict code to specific developers.
       - Create Orgs (organizations) to coordinate package maintenance, coding, and developers.
       - Form virtual teams by using Orgs.
       - Manage multiple versions of code and code dependencies.
       - Update applications easily when underlying code is updated.
       - Discover multiple ways to solve the same puzzle.
       - Find other developers who are working on similar problems and projects.


 - 4. **Provide code snippets showing 3 different ways to export a function from a node module**
      - module.exports = {
    method: function() {},
    otherMethod: function() {},
};    
      - exports.method = function() {};
exports.otherMethod = function() {};




 
  Vocabulary |  Definition
 ------------|------------------------------------------------------------------------------------------------------------------
  ecosystem  | is a collection of software packages, libraries, and other resources that facilitate development as they integrate                        with each other. 
  Node.js    | is a platform built on Chrome's JavaScript runtime for easily building fast and scalable network applications.
  V8 Engine  | is Google's open source high-performance JavaScript and WebAssembly engine, written in C++. 
  module     | is essentially a reusable piece of JavaScript which exports specific objects, making them available for other modules                    to require in their programs.
  package    | is a directory containing a package.js file, which contains roughly three major sections: a basic description, a                          package definition, and a test definition.
  npm        | Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to                      manage private development as well.
  server     | is a computer program or a device that provides functionality for other programs or devices, called "clients".
  environment| variables are a fundamental part of developing with Node.js, allowing your app to behave differently based on the                        environment you want them to run in. 
  interpreter| is a computer program that directly executes instructions written in a programming or scripting language, without                        requiring them previously to have been compiled into a machine language program.
  compiler   | used to convert a program written in a high-level language into machine code(binary code 0's and 1's) understood by                      computers to create an executable program.
  

## node package manager (npm):
   - **npm consists of three distinct components:**
      - 1. the website:  discover packages, set up profiles, and manage other aspects of your npm experience.
      - 2. the Command Line Interface (CLI): runs from a terminal, and is how most developers interact with npm.
      - 3. the registry: is a large public database of JavaScript software and the meta-information surrounding it.
  



