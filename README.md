# Synchronous FIFO memory

Understanding of buffer is such that when data come at the receiving module at a fast rate but are processed slowly or irregularly by the another module, intermediate storage, also known as buffering, is always required.
It is a kind of junction between two same clocked module so that the smooth transfer of data can happen between them.
FIFO is a special type of buffer. 
<br>
The name "FIFO" stands for First In First Out. Here we are going to form a circular FIFO and discuss its operations.
<br>
The write pointer contains the memory address of the incoming data.The read pointer contains the address of the first data word in the FIFO that has to be read out. Reseting will lead to same address for read and write pointer that too at the starting memory location. Writer pointer will move to next memory address after successful write operation and read pointer will also move to next memory address after successful read operation. "Full" will happen when write pointer will gradually reach to read pointer memory location and "Empty" will happen when read pointer will reach to the write pointer location after successful read operations.
<br>
<br>
NOTE: <br>
(1) Never write into full FIFO <bR>
(2) Never read from empty FIFO

# Asynchronous FIFO memory
It is a kind of junction between two same clocked module so that the smooth transfer of data can happen between them. The read and write operation of data will happen
at different clock frequencies here.
