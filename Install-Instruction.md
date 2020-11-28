
# Installation steps for GoLang [Linux]

## Step-1 Download the specific tar from this download https://golang.org/dl/
   - Example: 
   ```sh 
   $ wget https://dl.google.com/go/go1.15.5.linux-amd64.tar.gz
   ```
   
## Step-2 Untar the golang binary into /usr/local directory
   - Example: 
   ```sh 
   $ tar -xzvf go1.15.5.linux-amd64.tar.gz 
   $ mv go /usr/local/
   ``` 
   
## Step-3 Setup the environment variables [GOROOT,GOPATH,PATH] for golang
   - GOROOT [It is the variable that will keep where the go binary is installed]
   - GOPATH [It is the variable that will keep where the go-project is going to create]
   - PATH [Linux path variable]
   ### Example:
   ```sh 
   $ export GOROOT=/usr/local/go
   $ export GOPATH=$HOME/Projects
   $ export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
   ``` 
   - you can add this lines to end of .profile file, after updating source the profile please source the profile 
   ```sh
   $ source ~/.profile
   ```
   
 ### Step-4 Create your gopath (where you are going to create your go project)

   ```sh
   $ mkdir -p $HOME/Projects/src
   ```
  
  Note: you must place your golang project inside $GOPATH/src
