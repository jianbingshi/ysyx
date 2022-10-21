all:*.cpp *.v
	$(call git_commit, "sim RTL") # DO NOT REMOVE THIS LINE!!!
	@verilator -Wall *.v *.cpp --cc --trace --exe --build
	@./obj_dir/V*
sim:*.vcd
	@gtkwave *.vcd



