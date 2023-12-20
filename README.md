# Case Study: Config-as-a-code

## Instructions

### Cloning the Repository to your device

1. Create an ssh key on your local machine since this is a private repository
   > - **`ssh-keygen`**
   > - copy the contents of id_rsa.pub
2. Add your ssh key on github
   > - Click your profile on the top right corner and navigate to settings
   > - On the left side under access select SSH and GPG keys
   > - Click new SSH key on the top right
   > - Add a title for your SSH key and paste the contents of **id_rsa.pub** under the **Key** input box then save.
3. Clone the project on to your device

   > - Go to this link [Case Study](https://github.com/skynet6969/case-study)
   > - Click the **<> Code** button then select SSH and copy the link.
   > - in your terminal make a directory of your choice **example: "mkdir repos/"** and navigate into it **"cd repos/"**
   > - execute the command **"git clone `<paste the link here>`"**
   >   > - **ls -l** (check if cloned folder exists)
   >   > - navigate into the folder if the clone was successful **"cd case-study-demo/"**
   > - if the terminal displays **"(main)"** that means you are inside the initialized git repository

   `additional note: if you are inside an initialized git repository directory and you have visual studio code installed you can execute the command " code . " to open the project in the vscode application`
