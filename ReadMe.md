Installing IPFS on Le Potato
This guide will show you how to install IPFS on a Le Potato board running Ubuntu.
Prerequisites
Le Potato board
Ubuntu operating system
Internet connection
Installation Steps
Download the IPFS binary for the ARM64 architecture: wget https://dist.ipfs.io/go-ipfs/v0.11.1/go-ipfs_v0.11.1_linux-arm64.tar.gz   
Extract the contents of the downloaded file: tar xvfz go-ipfs_v0.11.1_linux-arm64.tar.gz   
Move the extracted IPFS binary to the /usr/local/bin directory: sudo mv go-ipfs/ipfs /usr/local/bin/ipfs   
Launch IPFS for the first time to generate the configuration files: /usr/local/bin/ipfs init   
Add the IPFS binary path to the PATH environment variable so you can launch IPFS from anywhere: echo "export PATH=$PATH:/usr/local/bin" >> ~/.bashrc   
Source the ~/.bashrc file to apply the changes: source ~/.bashrc   
Launch IPFS: ipfs daemon   
IPFS should now be running on your Le Potato board.
Note: Before launching IPFS from the ipfs command, make sure to add the IPFS binary path to the PATH environment variable by following Step 5 and Step 6.
