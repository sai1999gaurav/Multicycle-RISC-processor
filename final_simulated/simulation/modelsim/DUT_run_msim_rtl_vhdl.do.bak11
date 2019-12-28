transcript on
if {[file exists rtl_work]} {
	vdel -lib rtl_work -all
}
vlib rtl_work
vmap work rtl_work

vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/DUT.vhdl}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/regfile.vhdl}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/alu.vhdl}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/2to1mux.vhdl}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/final.vhdl}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/fa1bit.vhd}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/mem_implementation.vhd}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/fa8bit.vhd}
vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/fa16bit.vhd}

vcom -93 -work work {/home/gaurav/Desktop/Sem4/EE224/projectdigi/final_simulated/Testbench.vhdl}

vsim -t 1ps -L altera -L lpm -L sgate -L altera_mf -L altera_lnsim -L maxv -L rtl_work -L work -voptargs="+acc"  Testbench

add wave *
view structure
view signals
run -all
