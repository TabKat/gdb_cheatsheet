# gdb_cheatsheet

gdb -q ./myprogram
-q -- suppress copyright, license... on program start

quit or q -- exit from the program

i - instruction
x - examine

example:
    
    i r $rip

address format:

    o - octal
    x - hexadecimal
    u - decimal
    t - binary

size of element:

    b - bite
    h - half-word
    w - word
    g - giant word

example:

    x/8xb $rip

    
    (gdb)> x/4xb $rip
    0x8048386 <main+16>: 0x7c 0x45 0xfc 0x00
    
    examine register $rip, show 4 binary in hex format

b -- breakpoint

ni -- next instruction