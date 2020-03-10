# Color Contrast API

## Installation 
The Color Contrast API is really simple. First you need to include color-checker.js which is about 4KB in size. Download the source file [here](https://colorcontrast.dev/api/color-checker.js)
```
<script src="color-checker.js" charset="utf-8"></script>
```

## Global Function
This file exposes a single global function, which takes two hex codes from the url or takes two hex codes from a function. This returns a data for you to use.
```
// URL
www.example.com/?f=000000&b=ffffff

// Function
checkColors("ffffff", "000000");
```

## Retrieve Data
The data is sent via an array to the front end and you can retrieve it like this.
```
colorData.contrast
```

## Available Data
Here's a list of all the data you can retrieve to the frontend.

|Name|Description|
|---|---|
|Foreground|Returns foreground HEX code|
|Background|Returns background HEX code|
|Contrast|Returns true contrast ratio|
|Rounded Contrast|Returns rounded contrast ratio|
|AA Headline|Returns true or false if ratio is greater than 3|
|AAA Headline|Returns true or false if ratio is greater than 4.5|
|AA Text|Returns true or false if ratio is greater than 4.5|
|AAA Text|Returns true or false if ratio is greater than 7|
|AA Component|Returns true or false if ratio is greater than 3|
|Foreground Luma|Returns foreground luma value used to get contrast ratio|
|Background Luma|Returns background luma value used to get contrast ratio|

## Demo
Check out the Color Contrast Checker [Demo](https://colorcontrast.dev/) to see what you could build.

---

# Roadmap
- Transparent foreground colors
- Detailed information on color contrast guidelines
- Suggested color if the color fails

---

#Contribute
Feel free to contribute to the color contrast checker!
