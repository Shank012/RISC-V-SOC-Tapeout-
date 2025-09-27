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

<img width="1857" height="647" alt="image" src="https://github.com/user-attachments/assets/e703d41b-3aae-475f-abf3-d28099a1ca00" />


#### <ins>**Iverilog**</ins>
```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
```

<img width="926" height="692" alt="image" src="https://github.com/user-attachments/assets/65ae1b25-4111-4c9e-8b13-76859f5955d4" />


#### <ins>**gtkwave**</ins>
```bash
$ sudo apt-get update
$ sudo apt install gtkwave
```
<img width="602" height="93" alt="image" src="https://github.com/user-attachments/assets/698e10e2-69a6-4e96-b0b1-30b4d11f2b24" />


