# RISC-V Reference SoC Tapeout Program VSD
The repository is about the RISC-V Reference SOC Tapeout program offered by VSD, a collabration with IIT Gandhinagar.


The activities include:
<div class="toc">
  <ul>
    <li><a href="#header-1">Week-0</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-2">Week-1</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-3">Week-3</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-4">Acknowledgements</a></li>
  </ul>
</div>  

## <h2 id="header-1">Week-0</h2>

**Week-0 - Installing TOOLS**
#### <ins>Instructions for installation of required tools can be found here:</ins>

### **System Requirements**
- 6 GB RAM
- 50 GB HDD
- Ubuntu 20.04 or higher
- 4 vCPU


### **TOOL CHECK**

#### <ins>**Yosys**</ins>
```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
$ git submodule update --init --recursive
$ make 
$ sudo make install
```


#### <ins>**Iverilog**</ins>
```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
```


#### <ins>**gtkwave**</ins>
```bash
$ sudo apt-get update
$ sudo apt install gtkwave
```
