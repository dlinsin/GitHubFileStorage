GitHubFileStorage
=================

A Mac OSX service using the wiki of a GitHub project as a replacement for the GitHub Download Area. 
It creates a link which can be pasted from your Clipboard.

##  Requirements

You need CLI Push&Pull access without a password prompt to the wiki of the GitHub project you want to upload the files to. 
In case you don't know how to set it up, check out https://help.github.com/articles/ssh-key-setup.

The repository you want to store files in needs a wiki setup. Just click the wiki link of your 
repository once.

The service needs [Growl](http://growl.info/) to be installed in order to deliver some progress information.

Your user's Downloads folder is used as a temporary storage, so the service needs read/write access to it.

## Installation

Download the service [here](https://github.com/dlinsin/GitHubFileStorage/wiki/files/GitHubFileStorage-1.0.zip) and unzip it. 
Double-click `GitHubFileStorage.workflow` and select installation as a service when Automator prompts you.

## How to upload files

Select on or multiple files and right-click to bring up the context menu. Select GitHubFileStorage

![](https://github.com/dlinsin/GitHubFileStorage/wiki/files/context_menu_screen.png)

The service will prompt you for the name of the repository, including the organization or username. 
For this repository it would be _dlinsin/GitHubFileStorage_:

![](https://github.com/dlinsin/GitHubFileStorage/wiki/files/repository_name_screen.png)

Once the upload was successful, the URLs will be copied to the clipboard and can be pasted anywhere.

Each step is confirmed by a Growl notification, the final notification is posted multiple times in 
case you uploaded multiple files:

![](https://github.com/dlinsin/GitHubFileStorage/wiki/files/final_growl_screen.png)

## Issues and Feature Requests

Please report issues via GitHub's [issue tracker](https://github.com/dlinsin/GitHubFileStorage/issues).

## License

GitHubFileStorage is licensed under the Apache 2 License.
