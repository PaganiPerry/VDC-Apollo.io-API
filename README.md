# Project Title

A brief description of your project.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

GitHub should allow you to access, in the main branch, an option to "Open in Colab"

Currently, there are about 13000 contacts in the Engineering Contact List---if you want to keep on adding to that specific file, please download the csv file above. You'll need to then upload that file to Google Drive. The name of the file depends on what you decide to do with the code. Read further into the Contributing portion to learn more.


## Usage

Since this is an API, this is being used in conjunction with Apollo.io, thus it'll be important to remember to check in on rate limits. 

## Contributing

In order for this code to work, since you'll be connecting/mounting/sharing to Google Drive, you'll need to update ceratin lines of the code, since you'll now be the "creator/owner" of the code.

![image](https://github.com/user-attachments/assets/f5a1375a-b906-4e3d-89b3-c204e43d5a82)

The reason it is the way it is is because the way I have the following folders and files set up goes as so: 
1. Shared folder called "VDC Engineering Contacts List" in My Drive (when I say my drive, I literally mean what Google Drive refers to as "My Drive" and not my actual Google Drive", so going forward I will make sure to differentiate them in the explanation).
2. Within the VDC Engineering Contacts List folder, I have document (which is just how Colab created it, but it can be opened as a Sheets file) called Test Engineer Contacts List V1.csv

Line 4 is in charge of simply mounting and connecting to your drive, so no real change needed here.

Next, you'll want to think about whether or not you'll want other to be able to access the CSV you're creating/adding to. 




## License

Information about the project's license.
