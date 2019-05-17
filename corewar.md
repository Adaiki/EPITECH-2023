B-CPE-200 corewar

Advanced tests

  02 - ASM - Full header - 5 tests

    01 - magic
    02 - prog_name
    03 - comment
    03 - prog_size
    04 - full header

  03 - ASM, valid bytecode cases - 18 tests

    01 - live
    02 - ld
    03 - st
    04 - add
    05 - sub
    06 - and
    07 - or
    08 - xor
    09 - zjmp
    10 - ldi
    11 - sti
    12 - fork
    13 - lld
    14 - lldi
    15 - lfork
    16 - aff
    17 - labels
    18 - comments

  04 - ASM, invalid cases - 35 tests

    01 - chars after comment
    01 - chars after name
    03 - comment too long
    04 - comment without quote
    05 - double comment def
    06 - double label def
    06 - double name def
    07 - empty name
    09 - empty
    10 - illformed label
    11 - incorrect args add
    12 - incorrect args aff
    13 - incorrect args and
    14 - incorrect args fork
    15 - incorrect args ldi
    16 - incorrect args ld
    17 - incorrect args lfork
    18 - incorrect args live
    19 - incorrect args lldi
    20 - incorrect args lld
    21 - incorrect args or
    22 - incorrect args sti
    23 - incorrect args st
    24 - incorrect args sub
    25 - incorrect args zjmp
    26 - label not declared
    26 - name too long
    27 - name without quotes
    29 - null comment
    30 - null name
    31 - ommited command
    32 - syntax invalid arg
    33 - syntax missing label char
    34 - syntax missing val after direct char
    35 - unknown command

  05 - ASM, real champion - 5 tests
  
    01 - champion 1
    02 - champion 42
    03 - champion octobre
    04 - champion spartiates
    05 - champion try_again

Basic tests

  01 - ASM, header - 3 tests

    01 - magic
    02 - prog_name
    03 - comment
