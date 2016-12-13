# ygoworld

Manual Yu-Gi-Oh! simulator.

## Prerequisites

<table>
  <tr>
    <td>
      <b>Node.js</b>
    </td>
    <td>
      <b>MongoDB</b>
    </td>
  </tr>
  <tr>
    <td>
      <a href="http://nodejs.org">
        <img src="http://i.imgur.com/p3A0qpY.png" height="50" title="Node.js">
      </a>
    </td>
    <td>
      <a href="http://www.mongodb.org/downloads">
        <img src="http://i.imgur.com/yHTrdiP.jpg" height="50" title="MongoDB">
      </a>
    </td>
  </tr>
</table>

## Getting Started

First, start up MongoDB:

```bash
$ mongod
```

Then, open up another terminal window:

```bash
$ git clone https://github.com/Yugioh-Sims-International/ygoworld.git && cd YGOSiM
$ npm install
$ node lib/server.js
```

## Building

To build YGOWorld, you need to install [Grunt](http://gruntjs.com) globally:

```bash
$ npm install -g grunt-cli
```

Run `grunt build` to concat and minify CSS and JavaScript files.

Run `grunt iteration` to watch CSS and JavaScript files and as you make changes,
it minifies the CSS and JavaScript files.

You can also run `grunt test` to use linters to check if you made any errors
in your code.

## Setting up an Administrator account

Once your server is up, you probably want to make yourself an Administrator (-) on it.

### db.json

To become an Administrator, edit congfig.json.


//{"Chen": 4, "Francexi": 4, "Access": 4}

		0: ' ', //user
		1: '+', //voice -> tournaments and broadcast
		2: '*', //mod   -> ban,mute
		3: '#', //admin -> promote
		4: '-' //owner  -> console


## License

[MIT](LICENSE)
