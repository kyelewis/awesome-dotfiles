# editorconfig

EditorConfig is a file which describes coding styles to be used across various IDEs and editors.

## Why Developers Use It

To keep consistent styles across different IDEs and editors- all IDEs and editors have their own configuration file
formats- and it's usually a good idea to keep these folders out of repositories.

Through the use of IDE and editor plugins and native support, the .editorconfig file allows different IDEs to share a common
configuration.

EditorConfig supports many popular IDEs without plugins, including Visual Studio and most of the IntelliJ Suite of IDEs

Plugins exist for VSCode, Notepad++, Sublime Text, Coda, Atom, Textmate, VIM, Emacs and others


## How To Include It In Your Project

Create a .editorconfig file in the root of your project

## How To Use It

    # An example EditorConfig file
   
    [*]         # The below applies to ALL files
    end_of_line = lf                # use line feed character at end of lines
    insert_final_newline = true     # Make sure there is a new line at the end of each document
    
    [*.js]      # The below applies to all .js files
    indent_style = space                # Use spaces (as opposed to tabs) for indents
    indent_size = 2                     # Use 2 spaces per ident level
    trim_trailing_whitespace = true     # Remove whitespace at the end of a line


## Sources
[Official editorconfig documentation](https://editorconfig.org/)