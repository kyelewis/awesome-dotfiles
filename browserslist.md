# browserslist

Browserslist is a configuration format and plugin which lets you choose which browsers your node.js application should support.

## Why Developers Use It

Most large javascript applications run through a bundler, which converts them from multiple files and libraries 
into more compact code.

When writing modern javascript or typescript, the bundler will also often trans-compile (transpile) some code,
because older browsers won't understand it.
 
Polyfills are functions written to convert newer code into code that's compatible with these older browsers.

As the number of polyfills increase, your resulting file becomes larger. These larger files take longer to download
and therefore your website will load more slowly.

In a **browserlist** file, you can choose to support browsers by name, version, relative version, market share and other parameters.

Limiting supported browsers helps reduce the number of necessary polyfills, and therefore makes the bundle smaller, and 
speeds up your website- with the trade-off that people with older browsers may not be able to enjoy full functionality.

## How To Include It In Your Project

You can use browserslist by including any of:

### Include it in **package.json**
Use the browserslist key, each query as a string in an array 

    "browserslist": ["last 2 versions", ">1%"]
    
    
### Create a **.browserslistrc** file or **browserslist** file 
Alternatively, set BROWSERSLIST_CONFIG environment variable to any file you like. Each line of the file is one query.

    last 2 versions
    > 1%

### Set a **BROWSERSLIST** environment variable
Each query is comma separated

    BROWSERSLIST="last 2 versions,>1%"

## How To Use It

The available queries include:

**Global usage statistics**

     > 5%
     > 10% in UK

**Relative versions**

    last 3 versions
    last 2 Firefox versions
    
**Absolute versions**

    ios 7
    ie 7
    
**Date**

    since 2018
    last 5 years

## Sources
[Official browserslist Project Github](https://github.com/browserslist/browserslist)