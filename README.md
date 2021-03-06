# Braille Dot

Homework for Interviewing [Young Webmaster Camp 16 (YWC#16)](https://ywc16.ywc.in.th)

This project uses English Braille data from [zeroclickinfo-goodies](https://github.com/duckduckgo/zeroclickinfo-goodies/blob/master/share/goodie/cheat_sheets/json/english-braille.json).<br>

Try it online at [BrailleDot](https://brailledot.herokuapp.com).

## Available Scripts

In the root directory, you can run:

### `npm run dev`

Runs both client and sever side in developer mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view the client side in the browser.<br>
Open [http://localhost:5000](http://localhost:5000) to view the server side in the browser.

### `npm run client`

Runs only client side in developer mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view the client side in the browser.


### `npm run server`

Runs only server side in developer mode.<br>
Open [http://localhost:5000](http://localhost:5000) to view the server side in the browser.

## Braille Dot API

### /api/braille/list

This API to list all Braille alphabet and numbers.

```javascript
[
  { 
    character: "a",
    braille: "100000"   // ⠁
  },
  { 
    character: "b",
    braille: "110000"   // ⠃
  },
  { 
    character: "c",
    braille: "100100"   // ⠉
  },
  ...,
  { 
    character: "z",
    braille: "101011"   // ⠵
  },
  { 
    character: "0",
    braille: "010110"   // ⠚
  },
  ...,
  { 
    character: "9",
    braille: "010100"   // ⠊
  }
]
```

### /api/braille/word/random

This API to random a word in length 1 to 5 and get its Braille.<br>

For example:

```javascript
{
  word: "home",
  brailles: [
    "110010",   // h: ⠓
    "101010",   // o: ⠕	
    "101100",   // m: ⠍
    "100010"    // e: ⠑
  ]
}
```
