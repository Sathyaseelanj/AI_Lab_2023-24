# Ex.No: 9  Logic Programming –  Computer Maintenance Expert System
### DATE : 17.10.2024
### REGISTER NUMBER : 212222060233
### AIM: 
Write a Prolog program to build a computer maintenance expert system.
###  Algorithm:
1. Start the program.
2. Write the rules for each fault in computer.
3. If system have printing problem, missing dots and no uniform printing then system fault on printer head.
4. If system have not printing, missing dots and spread inks then system fault on ribbon
5. If system have not printing, paper jam and out of paper then system fault on paper stuck in printer
6. Similarly define rules for all faults.
7. Define facts for system problems.
8. Find the fault of computer by passing query to system.
     
### Program:
```
fault(printer_head) :-
	problem(not_printing),
	problem(missing_dots),
	problem(nonuniform_printing).
fault(ribbon) :-
	problem(not_printing),
	problem(missing_dots),
	problem(spread_ink).
fault(paper) :-
	problem(not_printing),
	problem(paper_jam),
	problem(out_of_paper).
fault(motherboard) :-
	problem(long_beep),
	problem(short_beep).
fault(hard_disc) :-
	problem(two_short_beeps),
	problem(blank_display).
problem(not_printing).
problem(missing_dots).
problem(spread_ink).
problem(two_short_beeps).
problem(blank_display).
```
### Output:

![ComputerMaintenance_1](https://github.com/user-attachments/assets/1ea9e07d-3ea9-4a82-9384-7e5aa1d6be1c)

![ComputerMaintenance_2](https://github.com/user-attachments/assets/f6d6c430-cbb5-4a6a-8879-6966c9abe356)

![ComputerMaintenance_3](https://github.com/user-attachments/assets/f1de32e9-b2cb-453d-b917-eca78fe7bf76)

![ComputerMaintenance_4](https://github.com/user-attachments/assets/77b5e8cc-c77e-4103-9264-3d0722219b58)

![ComputerMaintenance_5](https://github.com/user-attachments/assets/ab59bee1-5137-4d98-be2b-0cfe889d7081)






### Result:
Thus the simple omputer maintenance expert system was built sucessfully.
