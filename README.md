<h1 align="center">
  <br>
  <a href="https://nitoneum.com"><img src="NiTNode.png" alt="nitoneum node" width="250"></a>
  <br>
  supernode setup
  <br>
</h1>
<p align="center">
<a href="https://nitoneum.com/">
  <img alt="Master Node Uptime" title="Master Node Uptime" src="https://img.shields.io/uptimerobot/ratio/7/m788016512-c588ac46f17e954369b914ca">
</a>
<a href="https://github.com/nitoneum/core/blob/main/COPYING">
  <img alt="MIT License" title="MIT License" src="https://img.shields.io/github/license/nitoneum/core">
</a>
<a href="https://github.com/nitoneum/donations#readme">
  <img alt="Make a donation" title="Make a donation" src="https://img.shields.io/badge/%24-donate-orange">
</a>
</p>

https://nitoneum.com/node

## Environment Setup
Make sure that you're running Ubuntu 16

``` shell
sudo curl -s -o install https://nitoneum.com/node/setup.sh && sudo bash install
```

## Node Config
First create the `.nitoneum` folder in your home directory. You can copy and paste the following two lines below to create the folder and configuration file.
``` shell
mkdir -p .nitoneum; cd .nitoneum
touch nitoneum.conf
```
Use your favorite text editor eg. `vi`, `vim` or in this case `nano`.
<p align="center">
<img alt="Node Config" src="nanoconfig.png">
</p> 

``` shell
server=1
daemon=1
rpcuser=RPC_USERNAME
rpcpassword=RPC_PASSWORD
rpcallowip=127.0.0.1
```
Save the file and exit.

## Start Node 
``` shell 
./nitoneumd -server -daemon
```

