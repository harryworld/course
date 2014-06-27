# Command Line

Some tools to install your environment.

First to install `iTerm 2`, which is an equivalent tool to the default `Terminal` provided by Mac. Why? Because it is more powerful.

## Install Node.js

```
brew install node
```

## Install CoffeeScript

```
npm install -g coffee-script
```

## Install CoffeeLint

```
npm install -g coffeelint
coffeelint <file.coffee>

Why coffeelint uses 80 chars as a line length limit:
http://legacy.python.org/dev/peps/pep-0008/#maximum-line-length

coffeelint --makeconfig > ~/.coffeelint.json

alias clint='coffeelint -f ~/.coffeelint.json'
```

## Install http-server

```
npm install http-server -g
```

### Some Commands

```
cd
mkdir
rm -rf
mv
ls
ls -la
nano

~/Documents/workspace/
```

## Install oh-my-zsh

Handy tools and themes in Command Line, make it more fun.

```
via `curl`

curl -L http://install.ohmyz.sh | sh

via `wget`

wget --no-check-certificate http://install.ohmyz.sh -O - | sh
```

If you are using `wget`, make sure it is installed. For Mac:

```
brew install wget
```

# Success Completion

Student feels comfortable to the Command Line, creating project, files, and git push to a repository. Also, he knows how GitHub helps the open-source community to build powerful tools.

# Resources

- http://nodejs.org/
- https://www.npmjs.org/
- http://shapeshed.com/setting-up-nodejs-and-npm-on-mac-osx/
- https://github.com/joyent/node
- https://github.com/jashkenas/coffeescript
- https://github.com/robbyrussell/oh-my-zsh
- http://ohmyz.sh/
- https://gist.github.com/chasm/9066104
- https://gist.github.com/chasm/9066128