## SCSS-To-Json for Pattern Lab-Node

A Pattern Lab-Node wrapper for [Evan Lovely's](https://github.com/EvanLovely) excellent [scsstojson](https://github.com/EvanLovely/scsstojson) module. 

**Runs every time a build occurs.**

## Install

(coming to an NPM registry near you)

(Remember to run `NPM run postinstall` in your Pattern Lab base directory.)

## Usage

Add watch files to `patternlab-config.json` under plugins -> plugin-node-scsstojson -> options -> scssFiles 

example:

```
{
  "src": "source/_patterns/00-atoms/00-global/_color-vars.scss",
  "dest": "source/_patterns/00-atoms/00-global/colors.json",
  "lineStartsWith": "$c-",
  "allowVarValues": false
}, {
  "src": "source/_patterns/00-atoms/00-global/_fonts.scss",
  "dest": "source/_patterns/00-atoms/00-global/fonts.json",
  "lineStartsWith": "$font-",
  "allowVarValues": false
}
```
