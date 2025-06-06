

# List all the Tools

### Below are the Tools will be done in 3 months

- Linux
- Git and Github
- AWS & Terraform
- Maven
- Docker
- Kubernates & helm charts(Micro Service)
- Jenkins & gitlab CI
- Sonarqube
- Nexus
- Monitoring Stack ( grafana , Promatheus &ELK)
- Shell Scripting
- Ansible

### You need to have access few sites
- [Github](https://github.com/)
- [AWS Console](https://aws.amazon.com/)
### Chocolatey 
Chocolatey helps us to install all the tools without any harmful effects
- [chocolatey](https://chocolatey.org)
  
Tools we need to install in our laptop
- Visual Studio Code
- Git bash

# Linux
### Basic Commands
- # pwd :
   Present working Directory
  ```
  pwd
  ```
- # cd :
   Change Directory
  command | Role
  --------|------
  cd      |  change directory
  cd ..   | Take you to previous folder
  cd -    | Take you to the previous working folder
  cd .    | current folder
  cd .. /..| two folders back

- # ls :
  list files and folders
  ```
  ls
  ```
  To list all the files and folders info
  ```
  ls -l
  ```
  Orderng particular files and folders
  ```
  ls -ltr
  ```
  To list all hidden files
  ```
  ls -a
  ```
  to list files and folders in each folder
  ```
  ls -R
  ```
  To list line by line
  ```
  ls -1
  ```
- # Basename :
  To print current folder name:
  ```
  basename "$PWD"
  ```
- # env :
  Environment variables
  ```
  env
  ```
- # Export :
  To set environment variable
  ```
  export Variable_name=Value
  ```
  ```
  vi ~/.bashrc
  ```
  ```
  source ~/.bashrc
  ```
- # date
  ```
  date
  ```
  ```
  date +"%d/%m/%y"
  ```
  if you want particularly the name of the day
  ```
  date +"%A"
  ```
- # man :
  ```
  man date
  ```
- # who :
  ```
  who
  ```
  ```
  whoami
  ```
- # uptime :
  ```
  uptime
  ```
- # History :
  ```
  history
  ```
- # cat :
  To display the data 
  ```
  cat filename
  ```
  if you want to display both files data
  ```
  cat file1 file2
  ```
- # touch :
  To create file
  ```
  touch filename
  ```
  To create multiple files at a time
  ```
  touch file1 file2
  ```
  To create files with extensions
  ```
  touch file1.txt file2.json
  ```
- # vi :
  To edit data in file
  ```
  vi filename
  ```
  * press i = Insert mode
  * Enter data
  * press Esc
  * give :wq! = to save and exit
- # cp :
  To copy data from one file to another file
  ```
  cp sourcefile destinationfile
  ```
  To copy a directory
  ```
  cp -r  sourcefoldername destination
  ```
- # mkdir :
  To create empty directory
  ```
  mkdir foldername
  ```
  To create Multiple directories at a time
  ```
  mkdir folder1 folder2
  ```
  To create folder inside another folder
  ```
  mkdir -P folder1/folder2/folder3
  ```
- # rm :
  To remove files.
  ```
  rm filename
  ```
  To remove directory
  ```
  rm -r foldername
  ```
- # rmdir  :
  To remove Empty directory
  ```
  rmdir foldername
  ```
- # echo :
  To display a message line
  ```
  echo " Hello chandana "
  ```
- # mv :
  To Rename files or foldernames
  ```
  mv filename newfilename
  ```
  To move file into directory
  ```
  mv filename Directory
  ```
  To move a file into folder inside another folder
  ```
  mv filename folder1/folder2/folder3
  ```
  To move a folder into another folder
  ```
  mv sourcefolder Destinationfolder
  ```
- # wc :
  It will print no.of lines , words , characters
  ```
  wc  filename
  ```
  To print number of lines count
  ```
  wc -l filename
  ```
  To print characters count
  ```
  wc -c filename
  ```
  Both lines and characters count
  ```
  wc -lc filename
  ```
- # rev :
  To print in a reverse way
  ```
  rev filename
  ```
- # pipe symbol '|' :
   To pass the output of one command to input of another command
  ```
  ls -l | wc -l
  ```
  ```
  ls -1 | wc -lc
  ```
- # cut :
  To extract specific columns,characters or fields from a text
  ```
  cut -d : -f1 /etc/passwd
  ```
  Using pipe symbol
  ```
  cat /etc/passwd | cut -d : -f1
  ```
  ```
  pwd | cut -d / -f6
  ```
- # > : Output Redirection :
  ```
  ls -l > output.txt
  ```
- # >> : Append Redirection :
  ```
  pwd >> output.txt
  ```
- # 2>&1 : Error Redirection
  ```
  command 2>&1 | tee filename.txt
  ```
- # tee :
  when you want to log the output of a command while still seeing it on terminal
  ```
  ls | tee log1.txt
  ```
  useful options
   * -a : append to the file instead of overwriting it
   * -i : ignore interrupts
  ```
  ls -l | tee -a log1.txt
  ```
  if you run a wrong command and expect the output to be captured using tee
  ```
  wrongcommand 2>&1 | tee -a log1.txt
  ```
  now
  ```
  cat log1.txt
  ```
### Lets try to install any tool
```
tree
```
its not there so we have to install it
Before installing anything we have to do below
```
apt-get update
```
```
sudo apt-get update
```
now we have to install 
```
apt-get install tree -y
```
```
sudo apt-get install tree -y
```
Now, its installed successfully

- # tree :
  To show files and folders in a tree structure
  ```
  tree
  ```
### In some machines Git wont be available,
### So , if the git is not installed ,do below steps
* got to visual studio code
* git clone repositoryURL
```
sudo apt-get update -y
```
*
```
sudo apt-get install git -y
```
- # Head :
  it will print first few lines
  ```
  head filename
  ```
  to print first 20 lines
  ```
  head -20 filename
  ```
- # tail :
   it will print last few lines
   ```
   tail filename
   ```
   To print last 15 lines
   ```
   tail -15 filename
   ```
  # to print only 8th line using head and tail together:
  ```
  head -n 8 filename | tail -n 1
  ```
  * first 8 lines --> head -n 8
  * from that , only the last line ( which is the 8th)--> tail -n 1
# nginx
### its an application
### if you want to install anything in my machine what we will do
 * apt-get install nginx -y
```
sudo apt-get install nginx -y
```
* nginx is installed in linux machine
* we can access that particular application in web browser.
# nginx log file path in ubuntu
 * Access logs:
   ```
   cat /var/log/nginx/access.log
   ```
 * Error logs:
   ```
   /var/log/nginx/error.log
   ```
### if you want to see continuous log files generated
```
tail -f /var/log/nginx/access.log
```
* if you want to see particularly 10th line in log file
  ```
  head -10 logfile | tail -1
  ```
* if you want to print only last line in logfile
  ```
  tail -1 logfile
  ```



    
  
  
  

