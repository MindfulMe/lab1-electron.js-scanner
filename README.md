# Lab 1 Electron.js

Just run:
```
npm i
npm start
```
make sure you have python 2 installed and node.js environment setup.

# omr

omr is a simple python2 **o**ptical **m**ark **r**ecognition script. It takes as input an image of an answered answer sheet and outputs which alternatives were marked. Scroll down for an example.

## Usage
```sh
$ python2 omr.py --help
usage: omr.py [-h] --input INPUT [--output OUTPUT] [--show]

optional arguments:
-h, --help       show this help message and exit
--input INPUT    Input image filename
--output OUTPUT  Output image filename
--show           Displays annotated image
```

## Example

```sh
$ python omr.py --input img/answered-sheet-photo.jpg  --output /tmp/results.png --show

Q1: A
Q2: C
Q3: C
Q4: E
Q5: N/A
Q6: N/A
Q7: A
Q8: N/A
Q9: N/A
Q10: N/A
```

In this case, we used the following image as input:

<img src="http://i.imgur.com/JTAgYNF.jpg" alt="Input" style="max-width: 50%;"/>

And got the following output:

<img src="http://i.imgur.com/4n9fKFF.png" alt="Output" style="max-width: 50%;"/>

## Anwer Sheet

The answer sheet is available in the `sheet/` directory.

## Development

### Run unit tests

`test_omr.py` contains unit tests that can be run using:

```bash
$ py.test
======================================================== test session starts =========================================================
platform darwin -- Python 3.6.5, pytest-3.5.1, py-1.5.3, pluggy-0.6.0
rootdir: /Users/user/omr, inifile:
plugins: remotedata-0.2.1, openfiles-0.3.0, doctestplus-0.1.3, arraydiff-0.2
collected 1 item

test_omr.py .                                                                                                                  [100%]

====================================================== 1 passed in 1.61 seconds ======================================================

```


# electron-quick-start

**Clone and run for a quick way to see Electron in action.**

This is a minimal Electron application based on the [Quick Start Guide](https://electronjs.org/docs/tutorial/quick-start) within the Electron documentation.

**Use this app along with the [Electron API Demos](https://electronjs.org/#get-started) app for API code examples to help you get started.**

A basic Electron application needs just these files:

- `package.json` - Points to the app's main file and lists its details and dependencies.
- `main.js` - Starts the app and creates a browser window to render HTML. This is the app's **main process**.
- `index.html` - A web page to render. This is the app's **renderer process**.

You can learn more about each of these components within the [Quick Start Guide](https://electronjs.org/docs/tutorial/quick-start).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/electron/electron-quick-start
# Go into the repository
cd electron-quick-start
# Install dependencies
npm install
# Run the app
npm start
```

Note: If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.

## Resources for Learning Electron

- [electronjs.org/docs](https://electronjs.org/docs) - all of Electron's documentation
- [electronjs.org/community#boilerplates](https://electronjs.org/community#boilerplates) - sample starter apps created by the community
- [electron/electron-quick-start](https://github.com/electron/electron-quick-start) - a very basic starter Electron app
- [electron/simple-samples](https://github.com/electron/simple-samples) - small applications with ideas for taking them further
- [electron/electron-api-demos](https://github.com/electron/electron-api-demos) - an Electron app that teaches you how to use Electron
- [hokein/electron-sample-apps](https://github.com/hokein/electron-sample-apps) - small demo apps for the various Electron APIs

## License

[CC0 1.0 (Public Domain)](LICENSE.md)
