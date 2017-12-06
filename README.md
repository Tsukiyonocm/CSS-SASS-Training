Advanced CSS and SASS: Take Your CSS to the Next Level
Udemy Class: Jonas Schmedtmann

1. How to use NPM to auto update your SASS file while working This particular string is part of the package.JSON in your project folder, placed in scripts:
"scss": node-sass sass/main.scss -o css/styles.css --watch

Breakdown:

"scss": This is the name of the function you are going to call in npm. This is used in the final command line in order to run the script.

node-sass: This is I think just directing to the npm sass file system.

sass/main.scss: this is the input file you are using. You use this so that NPM knows where it is pulling the SASS data from in order to compile to the output folder.

-o css/styles.css: This is for windows based system, but this tells the command line that the following filepath/name is the output folder/file. For instance, css/styles.css tells NPM to output to the CSS folder and name the file styles.css.

--watch: this tells the compiler to watch the SASS file and automatically compiles it to the output file.

2. After setting up the package.JSON script above, go back into the command line and use this command:

npm run scss

This is fairly self explanatory. NPM is needed so the command line knows you are using the Node command system. run tells the command line you are going to be running a script and scss is the script you are running.


Using NPM to run a live server (automatic updates of all changes to all files):
1. Download the live-server NPM package (if not already done so)
npm install live-server -g

The -g will install the live server globally so that you can use this feature on any projects.

2. On the NPM command line, type in the text: live-server
Thats it, after this everything will be updated in its own window as you save new updates.
