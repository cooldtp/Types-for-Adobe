# Use TypeScript for Adobe Products
[<img src="https://i.imgur.com/VMx9MeE.jpg" width="560" height="315" />](http://youtu.be/h-c7A8pQzx8)

## Prerequisites
Install [Node.js](https://nodejs.org/en/download/) and [TypeScript](https://www.typescriptlang.org/#download-links).

## Your first script for eg. Adobe Illustrator
```bash
mkdir test
cd test
npm init -y
npm i pravdomil/types-for-adobe

printf '{"compilerOptions":{"module":"none","noLib":true,"types":["types-for-adobe/illustrator/2015.3"]},"exclude":["node_modules"]}' > tsconfig.json
# change tsconfig.json types value to Adobe product you're targeting

printf 'alert(String(app))' > index.ts
# open index.ts your favourite TypeScript editor and start scripting

tsc -p .
# compile files and run index.js in Adobe Illustrator
```

## Note
Declaration files is generated by https://github.com/pravdomil/extendscript-xml-to-typescript converter.

Definitions was created in summer 2017 by [Pravdomil.com](https://pravdomil.com).
You can [buy a beer for him](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=BCL2X3AFQBAP2&item_name=types-for-adobe%20Beer).
