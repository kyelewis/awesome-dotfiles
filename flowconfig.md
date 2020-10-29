# flowconfig

flowconfig is a file which describes a configuration for flow, a static type checker for JavaScript code

## Why Developers Use It

TODO


## How To Include It In Your Project

Create a .flowconfig file in the root of your project

## How To Use It

    # An example flowconfig file
   
    [include]       # Additional Files to include in flow, other than ./
    ../anotherfile.js
    ../anotherFolder/
    
    [ignore]        # Files to ignore in flow, as OCaml Regular Expressions
    .*/dist/.*
    
    [untyped]       # Files to not be type checked
    .*/untypedFiles/.*


## Sources
[Official flowconfig documentation](https://flow.org/en/docs/config/)