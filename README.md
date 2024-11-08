# DSP-10C# DSP-LAB-10C

#DIVISION USING DIRECT ADDRESSSING MODE

PROGRAM:

 DIVID .SET 0H 
DIVIS .SET 1H 
QOUT .SET 2H 
REMAIN .SET 3H 
.mmregs 
.text 
START: 
STM #140H,ST0 
RSBX CPL 
RSBX FRCT 
NOP 
NOP 
NOP 
NOP 
LD DIVID,A 
RPT #0FH 
SUBC DIVIS,A 
STL A,QOUT 
STH A,REMAIN 
HLT:   B HLT 

INPUT:

 DATA MEMORY
 A000H 0009 
A001H 0002 

OUTPUT:

 DATA MEMORY
 A002H 0004 
A003H 0001
