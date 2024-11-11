# Project Title

A brief description of your project.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

GitHub should allow you to access, in the main branch, an option to "Open in Colab"

Currently, there are about 13000 contacts in the Engineering Contact List---if you want to keep on adding to that specific file, please download the csv file above. You'll need to then upload that file to Google Drive. The name of the file depends on what you decide to do with the code. Read further into the Contributing portion to learn more. This may impact which method you decide to choose later (read more further down).

## Usage With Apollo.io

Since this is an API, this is being used in conjunction with Apollo.io, thus it'll be important to remember to check in on rate limits. 

First, locate to the "settings" icon in the bottom left hand corner and click on it.
![image](https://github.com/user-attachments/assets/86c8af5e-b063-49dc-ae78-3e85282e128f)

Below: Navigate to the "Integrations" tab by either searching API in the search bar or by simply navigating to the integrations tab. 
![image](https://github.com/user-attachments/assets/2e62333e-a019-40df-b353-e66bf5b21459)

Below: Once you're in the integrations tab, navgiate to the API tab and click on it.
![image](https://github.com/user-attachments/assets/59f2b902-f573-4d22-8d47-dc9f43cbc475)

Below: Navigate to the "usage" tab and there you'll be able to track how many calls you have. 
![image](https://github.com/user-attachments/assets/8c218240-f911-4a03-a9d2-495acce6c3ec)




## Usage of Code

Terms: 
1. Cell = Jupyter Notebooks are made up of instances/sequences of cells---these are the multiline input fields where you put your code
2. Calls = also known as an API request---a message sent to a server to request information or a service; there are limits to how many you can make in an alotted time

There are two main ways to start out here and they are listed below. You can decide which approach you would like to use.

However, in order for this code to work, since you'll be connecting/mounting/sharing to Google Drive, you'll need to update ceratin lines of the code, since you'll now be the "creator/owner" of the code. The lines circled in blue are the lines that need to be changed (unless you decide to keep the name, but you will read about that below).

Below: Main Cell (2nd cell) where you can change the postions and the number of pages being queried into the API
![titles_pages_change](https://github.com/user-attachments/assets/155fe6ec-0a08-48f3-bfdc-f70218db6ba1)


Below: Main Cell (2nd cell)
![Main_cell_change](https://github.com/user-attachments/assets/cf7f4832-60db-434e-84d6-090e35f980fe)

Below: where you will be entering in the company (or companies) domain. If you want to add more than one company at once, separate the domains with commas (.com, .com, .com, etc). 
![input_change](https://github.com/user-attachments/assets/eb9a791b-26de-48a2-afb2-8c84e9fb8e41)

Below: 3rd cell
![if_file_exists_change](https://github.com/user-attachments/assets/6a0ffcd3-be0e-4a3b-83f8-8354e01776ed)

Below: 4th cell
![download_df_change](https://github.com/user-attachments/assets/1e55cdf0-9a36-4e6b-b7c3-6ba7805c1c2a)

Below: 5th cell
![graph_change](https://github.com/user-attachments/assets/53af68e5-76a4-425b-8e5a-031b993995dc)




#### OPTION 1 - STARTING FROM SCRATCH (CREATING YOUR OWN NEW CSV FILE IN A NEW OR EXISTING FOLDER):

1. You’ll want to create a folder in Google Drive.

2. Make sure you make any changes to the folder now before you run the code because you’ll need to redo some of it if you end up moving the location of the folder/file in Drive after.

3. Note that you DO NOT need to create the actual CSV file in Drive since it will be initialized once you run the code for the first time.

4. Run the first cell by clicking **Shift + Enter** or by pressing the small grey play button to the left of the cell.

5. Before you go any further, you’ll want to think of what folder, if any, you’ll want the file to be in and you’ll want to think of a name for the file. By default, it’s set to what I had my path and file name as. (`/content/drive/My Drive/VDC Engineering Contacts List/Test Engineer Contact List V1.csv`)
   - a. For example, if you want to create a folder called Apollo Contact Lists and you want the file to be named My First Contact List, your file path might look something like this (but remember to make the folder in your desired drive location beforehand): `/content/drive/My Drive/Apollo Contact List/My First Contact List.csv`

6. Once you figure out the naming conventions and have successfully updated each of the lines of code, the ones circled in blue, run the Main cell.
   - b. In the main cell it will prompt you to connect to drive---allow everything and continue.

7. Once that’s done, you can input a company's website into the input box. If you do not and you click enter, it will default to the VDC Website.

8. Once the Main cell is done, you’ll want to run the next one, which displays a list of companies that you have already added to the DF.


#### OPTION 2 - DOWNLOADING AND USING THE "Test Engineer Contact List v1.csv":

1. **First, start by getting everything set up:**
   - a. Download the CSV to your local disk.
   - b. Upload the CSV to Google Drive.
   - c. Depending on where you decide to put it in Google Drive, *and* if you end up changing the name of the file itself, you may need to change the lines of code that are circled in blue to match your file path.
     - i. If you plan on putting this in a shared folder, make sure that everyone you are working with has their code set up correctly with their respective file path.
   - d. For example, if you decide to change the name of the file to "New Engineering Contact List" and you put it in a file in My Drive called "Engineering Project," the lines of code in blue might look like this:
     - iii. `/content/drive/My Drive/Engineering Project/New Engineering Contact List.csv`
   - e. If you decide to keep it the same, you shouldn’t need to change anything about the code.

2. **Once everything is set up**, start by running the first cell by clicking **Shift + Enter** or by pressing the small grey play button to the left of the cell.

3. **Next, run the next cell**, which is the "Main cell". This is where all the action happens. When you run it, it'll prompt you to connect to Google Drive—you’ll need to allow it access to everything (I know it sounds a little sus but if you don’t the cell won’t run—I’ve tried).

4. Once you click through everything, you'll be able to enter a company website into the input box. Once you've typed in a domain, you can simply click Enter and it'll complete running the cell (mentioned above and highlighted in the yellow circle in the screeshot).

5. It may take a little, especially if you've increased `num_pages` (which is fine) and/or added additional terms to the titles list (which is also fine).

6. Once it's finished running, it'll tell you a bunch of information on how much it found. Considering what it says can be confusing sometimes, it's best and easiest to just check to make sure everything was added. This is done by running the next cell and then going to your drive and the location where you stored the file.

7. Check the file to see if anything has been updated. Sometimes it runs, but not everything is added, such as emails or names. In this case, just continue on and try some other companies and come back to it later.

8. Running the next cell (4th cell) will allow you to download a version of the CSV to your local drive if you decide to.

9. Running the last cell (5th cell) will show you a graph of the most common titles. Note that it'll most likley be "Software Engineer", but it's still nice to see the spread of titles researched.





## Contribution

## License

Information about the project's license.
