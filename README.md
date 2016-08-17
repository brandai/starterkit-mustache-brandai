# starterkit-mustache-brandai

A pattern tree built for the Brand.ai and Pattern Lab integration.

## Installation
You can import the starterkit using one of the following commands:

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

Additional explanation and description on starter kit installations in this link: [https://github.com/pattern-lab/patternlab-node/wiki/Importing-Starterkits](https://github.com/pattern-lab/patternlab-node/wiki/Importing-Starterkits).

## Description

* In this starterkit you fill find patterns visualizing your style data from Brand.ai under BRANDAI menu item.
  Pattners:
    - Colors
    - Fonts
    - Typography
    - Logos
    - Icons
    - Images

* You can use those elements and your style data as standard Pattern lab components and the data as mustache data access flow.
* Note: for font to be rendered correctly you need to include your font directly in pattern lab.

## Synchronizing data
This starter kit contains style-data.json representing [example project](https://brand.ai/acme-demo-new) from Brand.ai.

To sync Pattern Lab with your live styleguide use can use our brandai-cli our replace style-data.json content
directly from your styleguide export app [for example](https://brand.ai/acme-demo-new/style/applications/data-export/json).

#### To use the cli
```
npm install brandai-cli --global
```
Then execute the below command that will dowload the json style data and copy it to the destination folder.
```
brandai json --dest source/_data --organization <organization> -- styleguide --<styleguide>

```

More details can be found in [brandai-cli](https://github.com/brandai/brandai-cli)
