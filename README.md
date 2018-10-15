## npm-commands

Some useful commands of npm (Node Package Manager)

#### package.json file creation
```bash
npm init 
```
#### Default package.json file creation
```bash
npm init --yes
```
#### For installing all the packages listed in the package.json file
```bash
npm i
```
#### Install package
```bash
npm i package-name
```
#### Install specific package version
```bash
npm i package-name@version 
```
#### List of all the dependencies with version
```bash
npm list
```
#### list of only package.json file packages (core packages) with version
```bash
npm list --depth=0
```
#### View registry info for a package
```bash
npm view package-name
```
#### View registry info for specific property for ex -> dependencies
```bash
npm view package-name dependencies          
```
#### View all the versions of that package
```bash
npm view package-name versions       
```
#### The list of all outdated packages version
```bash
npm outdated
```
#### Update packages
Only wanted version will be installed. Major version will not be installed with this command
```bash
npm update
```
#### Install npm-check-updates (ncu) package globally 
```bash
npm i -g npm-check-updates
```
-g (use for installing the package globally)
* After installing ncu, update the outdated packages
```bash
ncu -u  
npm i
```
#### Install dev dependency package
```bash
npm i packagename --save-dev
```
#### Uninstall package
```bash
npm un packagename  
```
### Semantic Versioning (SemVer)

Major.Minor.Patch

* Major -> for breaking the existing API features
* Minor -> for adding new feature updates
* Patch -> bug fixing updates

Caret (^) -> Major.x.x

Tilde (~) -> Major.Minor.x

### Publishing packages to npm registry

#### Create new account
```bash
npm adduser     
```
#### Login 
```bash
npm login  
```
#### Publish the package
```bash
npm publish   
```
#### Updating the published package
For changing version number
```bash
npm version patch
```
or
```bash
npm version minor
```
or
```bash
npm version major
```
then
```bash
npm publish
```

