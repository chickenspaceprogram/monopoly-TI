Note: This project is still in active development, so it is not exactly user-friendly. Apologies in advance for any inconvenience.

monopoly-TI v.0.2.0 (beta)
readme.txt

COMPATIBILITY:

monopoly-TI is written in TI-BASIC, a language intended for Texas Instruments graphing calculators. However, due to the large matrices used in this application, it is incompatible with the TI-84+ CE, since this calculator limits matrix size to a maximum of 400 elements.

This program should work on any other calculator model in the 83/84+ family, however, it does need somewhere north of 20000 bytes of free RAM to run properly. (The program itself is around 2000 bytes when stored. It only uses the extra memory when actively running.) I recommend archiving or deleting anything stored in RAM before running this program.

DESCRIPTION:

monopoly-TI is a program that uses a Markov Chain to find the probabilities of landing on each space in the board game Monopoly.

Please notify me of any bugs or errors you encounter by creating an issue in this project's GitHub repository!

INCLUDED FILES:

monopoly-TI/
|- dev/
| |- docs.txt
| |- fastrref-docs.txt
| |- MONOPOLY.8xg
|- readme.txt (you are here)

HOW TO USE:

To use this program, simply download MONOPOLY.8xg and send it to your calculator. Then, unpack it using the UNGROUP menu (located at [2nd][+][8]).

Then, run these programs in the following order:

prgmMONOGEN   (runtime: 35s)
prgmFASTRREF  (runtime: 2min)
prgmGETPROBS  (runtime: 1s)

Total runtime (TI-84+): ~2.5min

These times are approximate, runtime can vary depending on a number of factors. If you have a TI-83/83+, expect your runtimes to be roughly 2.5 times longer (~45min total) due to the slower clock speed on those calculators.

For this application to work, the following subprograms must also be present on your calculator (they are included in MONOPOLY.8xg):

prgmCHANCE
prgmCOMCHEST
prgmLEAVJAIL
prgmSENDJAIL

ACKNOWLEDGEMENTS:

Thanks to Kerm Martian for developing SourceCoder 3 (cemetech.com/sc), which made finding errors and debugging this mess far easier.

POSSIBLE FUTURE ADDITIONS:

Additions are listed here in the order they will likely be implemented in, however I make no promises as to when, whether, and in what order they will be added.

- Optimize and neaten some of the code (especially in the main body and subroutines of prgmMONOGEN. 
- Add proper progress indicators to all parts of the program
- Combine subprograms together to reduce the number of subprograms
