# mgrm
Multiple Git Repository Management Tool. It's from the idea npm package.json and google repo.
Using this tool needs to write package.json file, it recursively clones all the repositories described in dependencies field. Also it supports sematic version checks based on http://semver.org/
For more details, please reference to https://docs.npmjs.com/files/package.json#dependencies

1. Make sure you have a bin/ directory in your home directory and that it is included in your path:
   ```sh
   $ mkdir ~/bin
   $ PATH=~/bin:$PATH
   ```

2. Download the mgrm tool and ensure that it is executable:
   ```sh
   $ mkdir ~/bin
   $ git clone git@github.com:hsiaoairplane/mgrm.git
   $ cp ./mgrm/mgrm > ~/bin/mgrm
   $ chmod a+x ~/bin/mgrm
   ```

## Package.json format
At dependencies field, write the gitlab URL and the specify branch, tag, commit-ish, or range. For example:
   ```
   {
        "author": "hsiaoairplane"
        "version": "1.0.0".
        "repository": {
            "type": "git",
            "url": "git@github.com:hsiaoairplane/mgrm.git"
        },
        "dependencies": {
            "git@github.com:hsiaoairplane/python.git", "1.0.0",
			"git@github.com:hsiaoairplane/golang.git",  "master"
        }
   }
   ```

    For more details, please reference to https://docs.npmjs.com/files/package.json#dependencies

