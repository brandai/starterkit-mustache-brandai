# starterkit-mustache-brandai

A pattern tree built for the Brand.ai and Pattern Lab integration.

## Installation
You can import the StarterKit using one of the following commands:

#### PHP

``` bash
php core/console --starterkit --install brandai/starterkit-mustache-brandai
```

#### Node


``` bash
npm install brandai/starterkit-mustache-brandai
gulp patternlab:loadstarterkit --kit=starterkit-mustache-brandai
```
Note: use --clean=true if you want Brand.ai patterns to replace your current patterns, otherwise keep it false.

You can learn more about Pattern Lab StarterKit installations in the Pattern Lab wiki:  [https://github.com/pattern-lab/patternlab-node/wiki/Importing-Starterkits](https://github.com/pattern-lab/patternlab-node/wiki/Importing-Starterkits).

## Description

* In this StarterKit you'll find patterns that display your style data from Brand.ai under BRANDAI menu item.
  Pattners:
    - Colors
    - Fonts
    - Typography
    - Logos
    - Icons
    - Images

* You can use these elements and your style data as standard Pattern Lab components, and the data as mustache data access flow.
* Note: for a font to be rendered correctly, include your font directly in Pattern Lab.

## Synchronizing data
This starter kit contains style-data.json representing an [example project](https://brand.ai/acme-demo-new) from Brand.ai.

To have Pattern Lab use data from your design library, replace the default style-data.json with the style-data.json that's available for your design library. You can find the latter by visiting the data export app on Brand.ai. [See an example data export page](https://brand.ai/acme-demo-new/style/applications/data-export/json).

You can download the style-data.json file and copy it to your source folder. Alternatively, you can automate this process by running a brandai-cli command. This makes it easy to update Pattern Lab as your design library changes.

Here's how you'd do it. 

#### To use the cli
```
npm install brandai-cli --global
```
Then execute the below command that will download the JSON style data from Brand.ai and copy it to the destination folder.
```
brandai json --dest source/_data --organization <organization> --library --<design library>

```

More details can be found in [brandai-cli](https://github.com/brandai/brandai-cli)
