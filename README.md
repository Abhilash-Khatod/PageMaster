# PageMaster
This project implements a memory management engine that handles paging and virtual memory. The system simulates a computer's memory management unit, dealing with both main memory and virtual memory, and executes various commands related to process management and memory operations.

## 🚀 Features
- Memory allocation for processes  
- Paging system implementation  
- Virtual memory management  
- Process execution simulation  
- Memory swapping (swap-in and swap-out operations)  
- Page table management  
- LRU (Least Recently Used) replacement algorithm  

---

## 🛠 Key Components
1. **Memory Initialization**: Sets up main memory and virtual memory based on input parameters.  
2. **Process Management**: Handles loading, running, and killing processes.  
3. **Paging System**: Implements page tables and manages page allocation.  
4. **Virtual Memory Handling**: Manages swapping between main memory and virtual memory.  
5. **Command Interpreter**: Processes user commands for system operation.  

---

## 💻 Supported Commands
- `load <filename1> <filename2> .. <filenameN>` : Load executables into memory  
- `run <pid>` : Execute a program  
- `kill <pid>` : Terminate a program  
- `listpr` : List all processes in memory  
- `pte <pid> <file>` : Print page table entries for a process  
- `pteall <file>` : Print all page table entries  
- `swapout <pid>` : Move a process to virtual memory  
- `swapin <pid>` : Move a process to main memory  
- `print <memloc> <length>` : Print values in physical memory  
- `exit` : Terminate the system  

---

## ⚙️ Implementation Details
- Written in **C/C++**  
- Uses **LRU algorithm** for page replacement  
- Handles both **main memory** and **virtual memory**  
- Simulates process execution with **basic arithmetic operations**

## ▶️ Usage

### Compiling
g++ -o memoryEngine main.cpp Process.cpp MemoryManager.cpp
### Executing
./memoryEngine -M <main_memory_size> -V <virtual_memory_size> -P <page_size> -i <input_file> -o <output_file>



---

g++ -o memoryEngine main.cpp Process.cpp MemoryManager.cpp

#
