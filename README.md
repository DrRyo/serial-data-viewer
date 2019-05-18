# COM Grapher
![COM Grapher](https://user-images.githubusercontent.com/9062624/57970046-64491d00-79b7-11e9-8259-6d960aa5ce89.png)
Simple graph viewer communicates with serial(COM port).

## Getting Started

You can easily start with Download this project ZIP

### Prerequisites

* [Node.js](https://nodejs.org/) 10.15.3 or 12.2.0 *(Any version will be okay, but not sure)*
* [MS Build Tools 2015](https://www.microsoft.com/en-US/download/details.aspx?id=48159)

### Build
1. It requires [Node.js](https://nodejs.org/) and [MS Build Tools 2015](https://www.microsoft.com/en-US/download/details.aspx?id=48159)
   * *Any version of Node.js will be okay, but not sure*
   
2. [MS Build Tools 2015](https://www.microsoft.com/en-US/download/details.aspx?id=48159) is required for [node-gyp](https://github.com/nodejs/node-gyp)
   * *If you have **VS 2015** or **VS 2017**, you can skip this step*
   * **Don't use VS 2019! (Compatibility issue with node-gyp)**

3. Install required npm package for build
```bash
npm install
```

4. Rebuild packages, additionally rebuild serialport with *--update-binary* option.
```bash
npm rebuild
npm rebuild serialport --update-binary
```
   or, you can just run command below
```bash
npm run rebuild
```

5. Rebuild electron
```bash
./node_modules/.bin/electron-rebuild
```

6. *(Windows only)* To build executable, run this command. This will create **dist** folder with installer and portable.
```bash
npm install -g electron-builder
electron-builder install-app-deps
npm run build:win
```

## Authors

* **Ryo** - *Whole work*

## License

This project is licensed under the MIT License - see the LICENSE file for details

## Credits
Icons made by [Smashicons](https://www.flaticon.com/authors/smashicons) from [www.flaticon.com](https://www.flaticon.com/) is licensed by [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/)

## Acknowledgments

* Just lab work :)
