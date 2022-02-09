# Jitsi Meet API library

You can use Jitsi Meet API to create Jitsi Meet video conferences with a custom GUI.

## Installation

- [Installation guide](doc/API.md#installation)
- [Checkout the example](doc/example)

## Building the sources

NOTE: you need Node.js >= 12 and npm >= 6

To build the library, just type:
```
npm install
```
To lint:
```
npm run lint
```
and to run unit tests:
```
npm test
```
if you need to rebuild lib-jitsi-meet.min.js

```
npm run postinstall
```

Both linting and units will also be done by a pre-commit hook.

## Update

```
git remote add upstream git@github.com:jitsi/lib-jitsi-meet.git
git remote -v
```

```
git fetch upstream
git merge upstream/master
git push origin master
```

```
npm run build
git add .
git commit -a -m "update"
git push
```

```
npm uninstall lib-jitsi-meet
npm install git+ssh://git@github.com/Y-dentity/lib-jitsi-meet.git --save
```

## Install for a specific version tag

```
npm install git+ssh://git@github.com/Y-dentity/lib-jitsi-meet.git#1312 --save
```