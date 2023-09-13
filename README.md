# Text-Editor
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

This is a text editor that can run in a browser or as a Progressive Web Application. Users can save any text inputs in the text editor and it will save into a database when the user clicks out of the application. 

This application can also function offline since the data in the app is stored locally through IndexedDB.

One of the biggest problems I have when building this application is when the app could not find cached images. I realized that the file name of the images do not match the source from the `index.html`. Once I was able to fix it in the `webpack.config.js`, I was able to have app to show the image.

Here's the link to the website: https://cmdnguyen-text-editor-fbc030432d18.herokuapp.com/

## Table of Contents 

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

When you click on the deployed link, you have the option to install it as a Progressive Web Application. When you click on the install button and confirm it, it will be a standalone application that you can use outside of the browser.

## Usage

Once you have opened up the application in the browser, you will see this:

![Text Editor Browser](/assets/Opening-JATE.png)

Here it is as a PWA:

![Text Editor PWA](/assets/JATE-PWA.png)

You will also see that JATE header if you have cleared the site data or have nothing in the database.

In this demo, I added `console.log("Hello World")`:

![Text Editor Demo](/assets/JATE-Demo.png)

You can open ChromeDevTools or inspect the elements in your browser. You will see the console logs showing it pulled data from the database. It may not be exact, but this is what the console should look like:

![Text Editor DevTools](/assets/JATE-DevTools.png)

In the DevTools, go to the Application tab and you'll see Manifest. It will pull up the application's `manifest.json` file to show the user the presentation and the cached image. Here's what it should look like:

![Text Editor Manifest](/assets/JATE-Manifest.png)

You can also check if the application's registered service worker in the Application tab. Here's what it should look like:

![Text Editor Service Worker](/assets/JATE-ServiceWorker.png)

This next image shows you how you can access the IndexedDB storage:

![Text Editor IndexedDB](/assets/JATE-IndexedDB.png)

To access the application offline, click on the Network Tab and change from "No throttling" to "Offline". You can use the application offline and it should still be able to store into the database.

## Credits

Boot Camp Tutor, Alexis Gonzalez

Boot Camp TA, Kevin Long

Fellow Boot Camp Students: Eric Beverly, Jake Lipscomb, Marialda Cabral & Aaron Garcia

ChatGPT

## License

MIT License

Copyright (c) 2023 Catherine Nguyen

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
