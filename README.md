# HLASM-Instruction-Set-XRef
Based on z390 ZOPCHECK.CPY (courtesy Don Higgins), this is an Excel xref that allows for quick investigation of the IBM ISA via search by mnemonic or opcode.  There are 2,358 mnemonics/opcodes represented here.

For further reference see https://github.com/z390development/z390 (www.Z390.info) - z390 mainframe assembler emulator and run-time engine.

Overview
----------
Within Z390, Don and his team have a great tool called ZOPCHECK - a macro assembler program which runs on the open source z390 Portable Mainframe Assembler and on the IBM mainframe High Level Assembler (HLASM).

ZOPCHECK.CPY is a file that contains the instruction set found in IBM's z/Architecture Principles of Operation (SA22-7832-12). Further, a file called HLASM_Instruction_Set_Summary.TXT is used to gather instruction name and flags.

This Excel tool parses each line in ZOPCHECK.CPY and organizes the data in a way that is easily sorted and searchable. It also references HLASM_Instruction_Set_Summary to get name and flags.

This tool should help software developers to quickly reference mnemonics and opcodes, their operands, etc. Relevant data (columns C through P) can be sorted b/c filters are set for each column.

Future Use
----------
This tool has a VBA code behind it, intended to automate parsing. You can view the code by going to the Developer menu item in Excel and then choosing Visual Basic option. 

If and when the Z390 project updates ZOPCHECK, load the instruction set strings from the copybook in column 2 (starting row 2) and Click the Parse button. If all goes well, Column O shows a Match string.

Enjoy and KMF-Keep Moving Forward!
