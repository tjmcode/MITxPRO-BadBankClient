# MITxPRO-BadBankClient

A 4th refactoring of the Bad Bank App, moving it to the 3-Tier MERN Architecture.
The starting project was MITxPRO-BadBankReact3 made from Create-React-App (CRA).


## Description

This will be used for my MIT xPRO Portfolio.
This Bad Bank project is a refactored version of the Bad Bank 'Fire Hydrant' project I did
in the previous MIT 'Digital Transformation' course in December 2021.
It was bascially rewritten from scratch in React Components, Context, and State.
A 3rd refactoring took all possible Components and commonized and simplified them.

This refactoring moved the entire App to the MERN Client-Server Architecture...

<b>This was the process demo'ed by the MITxPRO Course:</b>

STEP 1: Move files into 'public' folder for serving as static files.</br>
STEP 2: Create new NodeJS App to handle the Server Side in the root folder.</br>
STEP 3: Serve all the static files with ExpressJS.</br>
STEP 4: Create Routes in ExpressJS for all React Components.</br>
STEP 5: Update UI to use new functionality from the Server.</br>
STEP 6: Add a Data Store (MongoDB) to the Backend.</br>
STEP 7: Test entire App with HTTP-SERVER and DOCKER Image.</br>
STEP 8: Host the SITE / APP and make public.</br>

I found I could not simply copy a working CRA into a 'public' folder under an Express Server,
this did not work, the React App never started. (Conflicts between the Server's 'public' folder
and the 'public' folder of the CRA project. I found it did work if I 'compiled' the CRA into a 'build'
folder and served that from my Express Server as a 'static public folder'.

<b>So, my process was:</b>

STEP 1:  Clone the MITxPRO-BadBankReact3 App into MITxPRO-BadBankClient.</br>
STEP 1a: Compile the CRA into a deploable 'build' folder' with 'npm run build'.</br>
STEP 2:  Create a new NodeJS App for the Server side: MITxPRO-BadBankServer.</br>
STEP 2a: Copy the MITxPRO-BadBankClient/build into MITxPRO-BadBankServer/public.</br>
STEP 3:  Serve all the static files with ExpressJS.</br>
STEP 4:  Create Routes in ExpressJS for all React Components.</br>
STEP 5:  Update UI to use new functionality from the Server.</br>
STEP 6:  Add a Data Store (MongoDB) to the Backend.</br>
STEP 7:  Test entire App with HTTP-SERVER and DOCKER Image.</br>
STEP 8:  TBD: Host the SITE / APP and make public.</br>


## Getting Started


### Dependencies

* REACT
* BABEL


### Installing

* Clone this repo

* Use "npm install" to load a simple HTTP Server for the project
```
npm install
```

* Make sure the Bad Bank Server is installed at this point and running on Port:3000

* Use "npm start" command in the project folder to start the React App development environment.
* Accept the option to use a new Port # (3001) because bad Bank Server is on Port 3000.
```
npm start
```

* Navigate your Browser to...
```
localhost:3001
```
* Verify standalone functionality if changes are made.

* Compile the CRA into a 'build' folder for use in MITXPRO-BadBankServer
```
npm run build
```

* Copy everything in the 'build' folder to the  MITXPRO-BadBankServer 'public folder replacing everything already there
```
Copy <development-path>\MITxPRO-BadBankClient\build <development-path>\MITxPRO-BadBankServer\public
```

* Demonstration of app startup...

<p align="left"><img src=".\public\app-startup.png" width="720" title="Server Startup..."></p>

* Example of app u.i...

<p align="left"><img src=".\public\app-ui.png" width="720" title="App U.I..."></p>

* Demonstration of the React Bad Bank... (https://youtu.be/hctvo-EFqe4.mp4)

<video id="demo-video" style="border-style:solid; border-width:2px" src="https://youtu.be/hctvo-EFqe4.mp4" width="1024" allowfullscreen="allowfullscreen" webkitallowfullscreen="webkitallowfullscreen" mozallowfullscreen="mozallowfullscreen" allow="autoplay *" loop autoplay autobuffer controls muted>
Your browser does not support the HTML5 player.
</video>


## Help

This is an unsupported demonstation project.

## Terminology

| Word or Acronym	| Description/Definition                                |
|-------------------|-------------------------------------------------------|
|  NPM	            | Node Package Manager, actually “Node PM”, “Node pkgmakeinst” a system to deploy, install, and maintain NodeJS Apps. (PM was a BASH utility).
|  Template	        | A file used to start others to ensure code and documentation consistency.
|  MERN             | MongoDB, Express, React, Node JS.
|  MongoDB          | A ‘NoSQL’ database designed for Cloud applications, also referred to as a ‘Document Store’.
|  Express          | Express is *not* a database but rather an ‘extensible routing language’ for communication between a Client and a Server.
|  React            | A Web UI development system, a JavaScript library developed by Facebook and made public—and Open Source—since 2013.
|  Node JS          | A development stack that executes from a local file store—on a local Server—instead of from a network of remote servers on the Web.


## Authors

Contributors names and contact info

* Dr. Abel Sanchez (MIT) [@Unknown](https://twitter.com/Unknown)

* Timothy J McGuire [@TimothyMcGuire](https://twitter.com/TimothyMcGuire)


## Version History

* 0.4
    * Refactored into the MongoDB, Express, React, NodeJS (MERN) Architecture.
* 0.3
    * Refactored further by simplifying the Form Component for all functions.
* 0.2
    * Refactored further into a 'create-react-app' framework with Context.
* 0.1
    * Refactored into the MicroCODE [MCODE] style and templates.
    * See [commit change]() or See [release history]()
* 0.0
    * Coded using MicroCODE Templates, following along with Dr. Sanchez' videos.

## Future Development

* 0.5
    * Correct NavBar nor re-rendering on Context changes.


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
