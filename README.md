# Pattern Lab Node Gulp Dependency Example

Making Pattern Lab Node a dependency allows you to host your source and public patterns and assets outside of the module, making upgrades easier.

This repository is a reference example of a fully configured parent project that uses [Pattern Lab Node](https://github.com/pattern-lab/patternlab-node) as a dependency. `node_modules` are not included out of sanity, but running `npm install` from this cloned repository will show that it is indeed a dependency along with everything else.

The example `patternlab-config.json` contains a paths object that defined absolute paths (C:/src/plndgulp/) to the installation of this example. **You will have to change this if you expect anything to run here.**

``` json
"paths" : {
  "source" : {
    "root": "C:/src/plndgulp/source/",
    "patterns" : "C:/src/plndgulp/source/_patterns/",
    "data" : "C:/src/plndgulp/source/_data/",
    "styleguide" : "C:/src/plndgulp/node_modules/patternlab-node/core/styleguide/",
    "patternlabFiles" : "C:/src/plndgulp/source/_patternlab-files/",
    "js" : "C:/src/plndgulp/source/js",
    "images" : "C:/src/plndgulp/source/images",
    "fonts" : "C:/src/plndgulp/source/fonts",
    "css" : "C:/src/plndgulp/source/css/"
  },
  "public" : {
    "root" : "C:/src/plndgulp/public/",
    "patterns" : "C:/src/plndgulp/public/patterns/",
    "data" : "C:/src/plndgulp/public/data/",
    "styleguide" : "C:/src/plndgulp/public/styleguide/",
    "js" : "C:/src/plndgulp/public/js",
    "images" : "C:/src/plndgulp/public/images",
    "fonts" : "C:/src/plndgulp/public/fonts",
    "css" : "C:/src/plndgulp/public/css"
  }
},
```

Documentation that attained this state can be found [here](https://github.com/pattern-lab/patternlab-node/wiki/Running-Pattern-Lab-Node-as-an-NPM-Dependency).
