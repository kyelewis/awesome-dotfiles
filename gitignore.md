# gitignore

Gitignore is a list of files to not track in a git repository

## Why Developers Use It

While developing projects, there are often files located in your development folders that you don't want to include in repositories. This may be because they are temporary (i.e. yarn.log), specific to you (i.e. .idea or .vscode IDE folders) or sensitive (i.e. .env file with secrets)

## How To Include It In Your Project

Git looks for gitignore settings:

- On the command line in commands such as git ls-files and git read-ree
- In the **.gitignore** file
- In ~/git/ignore
- In .git/info/exclude

## How To Use It

    # An example gitignore file
   
    *.json              # Ignore any .json files
    !thisfile.json      # But, don't ignore this one
    logs/               # Ignore the logs directory or any of its contents
    hello?.txt          # Ignore hello1.txt, hello2.txt, helloA.txt, helloZ.txt, etc...

## Additional Tips

A .gitignore file will prevent files from being added, but if files were already in place before
there were rules for them, they will not be automatically removed. They can be manually removed with git -rm --cached

You can use the [git check-ignore](https://git-scm.com/docs/git-check-ignore) command with a filenmame to check if certain files are ignored

## Sources
[Official gitignore documentation](https://git-scm.com/docs/gitignore)