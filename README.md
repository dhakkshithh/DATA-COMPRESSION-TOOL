# DATA-COMPRESSION-TOOL

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: DHAKSHITH BAVAN S

*INTERN ID*: CT04DF1802

*DOMAIN*: C PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH

*DESCRIPTION OF TASK 4*: 
               Run-Length Encoding (RLE) is a fundamental data compression algorithm that is especially effective for data sets that contain many repeated characters or patterns. Task 4 involves implementing both compression and decompression using the RLE technique in the C programming language. The goal of this task is to demonstrate how character streams can be efficiently encoded to reduce redundancy and then accurately decoded back to their original form.

In the RLE method, sequences of the same character that occur consecutively are replaced by a single character followed by the number of repetitions. For instance, a string like “aaabbcc” would be compressed to “a3b2c2”. This type of encoding is lossless, meaning the original data can be perfectly reconstructed from the compressed data.

The implementation of this task is divided into two parts: compression and decompression. During compression, the program reads a string character by character. It keeps track of the current character and a count of how many times it has appeared consecutively. Once a different character is encountered, the program appends the current character and its count to the output string. This process is repeated until the entire input string is processed. The result is a compressed version of the original string that takes up less space if there are repeating characters.

For decompression, the program reads the encoded string in pairs: it reads a character and the following digit(s) which represent the number of times the character should appear. For example, reading “a3” tells the program to output “aaa”. The decompression algorithm uses a loop to reconstruct the original string by repeating each character the specified number of times.

This task reinforces several important programming concepts in C such as string manipulation, character processing, loops, and use of standard input/output functions. It also introduces an applied use case for basic data compression, which has real-world applications in file storage, transmission, and image encoding (e.g., in bitmap or TIFF files).

To run the program, the user must first write the C code in a file, for example, rle.c. Using a terminal or command prompt, they can compile the code using a C compiler like GCC with the command gcc rle.c -o rle. After compilation, the executable can be run by typing ./rle (on Linux/macOS) or rle.exe (on Windows). The program then prints the compressed version of a predefined string such as "aaabbbccccdd" and also displays the decompressed result, which should exactly match the original.

Example Output:

Compressed: a3b3c4d2
Decompressed: aaabbbccccdd

This confirms that the compression and decompression are functioning correctly. This task is not only an exercise in coding logic but also a foundational step in understanding how larger-scale data compression technologies work. It’s particularly useful for students and beginners looking to understand both algorithm design and string processing in C.
