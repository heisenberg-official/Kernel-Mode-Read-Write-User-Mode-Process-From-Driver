# Read And Write User Mode Process ViA Kernel Mode (RING-0)
###### This project uses a kernel mode driver in co-operation with a user mode program to establish a method of reading / writing virtual memory from a regular win32 program without having to use regular WinAPI Functions. This happens by using a driver to execute the reading / writing of the memory itself from a lower level. This means the user mode program does not have to open any handles to csgo or use ReadProcessMemory or WriteProcessMemory nor any functions that has to deal with process handles.