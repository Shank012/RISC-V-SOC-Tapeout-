# RISC-V Reference SoC Tapeout Program VSD
The repository is about the RISC-V Reference SOC Tapeout program offered by VSD, a collabration with IIT Gandhinagar.


The activities include:
<div class="toc">
  <ul>
    <li><a href="#header-1">Day-1</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-2">Day-2</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-3">Day-3</a></li>
  </ul>
</div>  

<div class="toc">
  <ul>
    <li><a href="#header-4">Acknowledgements</a></li>
  </ul>
</div>  

## <h2 id="header-1">Day-1</h2>

**Day-1 - Introduction to Verilog RTL Design & Synthesis**

To start the lab, clone the workshop repository from GitHub:
```
git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop
cd sky130RTLDesignAndSynthesisWorkshop
```
The follow for generating verilog
```
RTL Design + .lib file → Yosys →  Netlist → write_verilog
```
Invoke Yosys

`yosys
`

Following are the commands to read the library file and verilog file

```
read_liberty -lib ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib

read_verilog good_mux.v

synth -top good_mux

abc -liberty ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib

show

write_verilog -noattr good_mux_netlist.v
```




