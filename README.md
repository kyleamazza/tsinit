# tsinit

The year is 2021. Creating a TypeScript project with sensible default development tools is still a P.I.T.A. So, here's a mind-numbingly simplistic bash script to initialize a bare TypeScript project with eslint, Prettier, nodemon and Jest.

Don't like one of them? Just replace the install with the package(s) that you like, then change the `cat <<EOF> ...` portion of the corresponding configuration file to the default configuration of your choosing. It's just a bash script.

## Prerequisites

This assumes you have Yarn 1.x. If you like npm, go ahead, change the script to use npm; your computer won't explode. If you like Yarn 2.x... bless your soul. npm comes bundled with your Node.js installation, Yarn can be downloaded via npm `npm i -g yarn`.


## Usage
`tsinit <your-project-name>`

No options, no flags, no extra arguments, no help messages. All it does is run Yarn/npm to install a bunch of dev dependencies, and then copy some text into configuration files. Everything is `@latest`.

Add this script somewhere in your `PATH` and make it executable with `sudo chmod +x /path/to/tsinit`.

