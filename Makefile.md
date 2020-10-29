# Makefile

A Makefile describes a series of steps required to compile an application or library from source code.

## Why Developers Use It

TODO

## How To Include It In Your Project

Create a Makefile in your project folder

## How To Use It

    # An example Makefile
   
    app: main.o display.o search.o              # app requires these three objects to exist
        cc -o app main.o display.o search.o     # build ./app using this command
    
    main.o: main.c main.h                       # main.o requires main.c and main.h to exist
        cc -c main.c                            # build main.o using this command
        
    display.o: display.c display.h              # display.o requires display.c and display.h to exist
        cc -c display.c                         # build display.o using this command  


## Sources
[Official make documentation](https://www.gnu.org/software/make/manual/html_node/Makefiles.html#Makefiles)