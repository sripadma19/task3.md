By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![image](https://github.com/sripadma19/task3.md/assets/161410141/72bc10c9-ed86-4105-b36a-91a4a1f5e44e)

**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&

![image](https://github.com/sripadma19/task3.md/assets/161410141/0fcc0f22-eafe-4b9b-bc50-22e096e2c001)

Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)
gcc sum1ton.c
![image](https://github.com/sripadma19/task3.md/assets/161410141/c41e8557-e686-4777-aee4-56b548a8f19f)
Step 5: Check the output by using the command

./a.out
![image](https://github.com/sripadma19/task3.md/assets/161410141/3a05d01d-94ed-4a08-8f80-50be82cee63d)



The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c

![image](https://github.com/sripadma19/task3.md/assets/161410141/55c401a3-b2e4-4752-9ea1-08b284b94b78)

Step 2: Compile the code in riscv using the following command


riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![image](https://github.com/sripadma19/task3.md/assets/161410141/ce48e447-48af-4082-a17f-f51d4b5283a8)

Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.


use the command ls -ltr sum1ton.c

![image](https://github.com/sripadma19/task3.md/assets/161410141/91cba957-86d2-489c-841a-c2a8c91c92c2)

Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution
![image](https://github.com/sripadma19/task3.md/assets/161410141/6e9dff33-6abb-4e88-bb01-aeb5a05b23fe)

![image](https://github.com/sripadma19/task3.md/assets/161410141/6dde7783-c5e6-48f9-bf24-55ee2d1560be)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![image](https://github.com/sripadma19/task3.md/assets/161410141/7de814f8-4271-4403-b8bd-0916c540b5f1)
![image](https://github.com/sripadma19/task3.md/assets/161410141/954cbf06-13f1-4603-a257-487a6d7f5977)








