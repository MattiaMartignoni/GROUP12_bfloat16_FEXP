# GROUP12_bfloat16_FEXP
16 bit floating point exponential unit based on taylor series approximation

BFloat16_FEXP is the final project with fixed number of bits and approximation

BFloat16_FEXP_mod are the sources and project with package and top module that can be modified by decommenting some parts in order to work with different
number of bits and taylor approximation

specifically:

in exponential_top lines from 455 to 478 can be modified for the three cases n mul = n tay, n mul = n tay + 1, n mul = n tay + 2 and n mul <= n tay + 3
we didn't considered the case of n tay > n mul

in exponential_pkg_scrap 65 80 and 85 can be modified respectively the number of bit of multiplication, taylor and the level of taylor approximation
lines from 240 to 398 can be modified to change multiplication bits
lines from 501 to 1056 can be modified to change taylor bits

in the sources file folder there's also a plts.py python file to be added inthe same folder where data_file and wrong_data_file are stored if using
exponential_tb3 or exponential_tb3 to see the error graphic 
