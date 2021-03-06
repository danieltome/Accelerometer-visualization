Location
======
A Statistics project to visualize accelerometer data and track a relative path based on compass heading and calculated pedometer data.

##Requirements
You will need...

1. [Node.js](http://nodejs.org/) installed on your computer.
2. A smartphone connected to the same Wi-Fi network as your computer.
3. To know the IP address of your computer.

##Setup

1. Clone this repository so you have a copy on your computer.
2. Launch [server.js](server.js) using Node. On Windows, this may be as easy as double-clicking on the file itself. On Linux and Mac, you may have to open a Terminal, `cd` to the folder containing [server.js](server.js), and run `node server.js`.
3. On your computer, launch your favorite browser (tested on Chrome) and type `localhost:5000` into the address bar.
4. On your phone, launch your favorite browser (tested on Chrome for Mobile) and type your computer's IP followed by `:5000`. For example, `192.168.1.123:5000`.
5. Walk around with the smartphone in your pocket and enjoy the data on the screen of your computer!

Enjoy! I'll leave you to figure out what each graph represents.

Note: to stop the server, click on the terminal window and press `Ctrl+C`, or for Mac users, `Control+C`.

##Issues

- Location tracking assumes with that each movement, you have taken a step of constant length forwards. Walking in place, walking backwards, or even taking steps of different lengths will add error to the calculated path.
- Location tracking also assumes that the phone stays in the same orientation relative to your body. Putting the phone in another pocket or rotating the phone in-place will add more error to the calculated path.
