# aemmultisync
A tool to allow `aemsync`-ing multiple directories at once.

## Usage
Sync two directories to one target:

`ams -t http://admin:admin@example.gov:4503 -w ~/dev/aem/frontend,~/dev/aemdam`

You can also have multiple targets, in case you need to sync multiple directories to author and publish. Simply comma separate each address, and each directory to watch:

`ams -t http://admin:admin@example.gov:4502,http://admin:admin@example.gov:4503 -w ~/dir1/sub/folder,~/dir2`

## Roadmap
Add exclusion and custom packmgr url support

Profile based configuration: configure a json object with targets, directories, exclude filters, etc. and deploy that config from the cli

## Contributing
Fork & clone the repo, make your changes, and submit a pull request..

## Credits
This package relies on [aemsync@1.1.1](https://github.com/gavoja/aemsync).
