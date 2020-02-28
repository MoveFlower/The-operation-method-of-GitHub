# The-operation-method-of-GitHub
Reord the operation method of GitHub
## First
>- Config your fundamental settings such as "your name" and "your email".
>- The instructions are:

    >1.git config --global user.name "your name"
    
    >2.git config --global user.email xxx
## Second
>- Open the GitHub and copy its website,then in the designated place click the right mouse button to open the ==Git Bash==.
>- In the window of the ==Git Bash==,we should clone in the first time.And then copy the documents, which you want to submit to GitHub,to the folder has beencreated just now.
>- The instructions are:

    >1.git clone ==htpp://...==
    
    >2.cd ==the name of the repository==
    
    >3.git add .
    
    >4.git commit -m =="free to write"==
    
    >5.git push -u origin master
## Third
>- **The error:**
error: RPC failed; curl 56 OpenSSL SSL_read: Connection was reset, errno 100
>- **The reason:**
at least one file is too large,==just set the file cap higher==
>- **The solution:**
git config --global http.postBuffer  524288000
