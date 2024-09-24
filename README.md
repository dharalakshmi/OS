Disc Scheduling Simulator – Operating System 

Project Overview
The Disc Scheduling Simulator project is an implementation designed to simulate various disc scheduling algorithms used in operating systems to manage and optimize the order of read/write requests on the disk. Disc scheduling plays a vital role in improving the overall performance of the system by reducing seek time and efficiently managing I/O operations. This project demonstrates how different algorithms prioritize requests, allowing users to visualize their impact on performance.


Disc Scheduling Algorithms: 
This simulator implements the following disc scheduling algorithms:

First Come First Serve (FCFS):
1. Processes disk requests in the order they arrive without any reordering.
2. Simple but may result in long wait times for certain requests.

Shortest Seek Time First (SSTF):
1.Selects the disk request that is closest to the current position of the disk arm, minimizing seek time.
2. More efficient than FCFS but may lead to starvation of distant requests.

SCAN (Elevator Algorithm):
1. Moves the disk arm towards one end of the disk, servicing requests in that direction, then reverses.
2. Provides a fairer approach by continuously scanning through the disk.
   
C-SCAN (Circular SCAN):
1. Similar to SCAN, but after reaching the end, the disk arm jumps back to the beginning without servicing requests on the return trip.
2. Ensures a more uniform wait time for all requests.
   
LOOK:
1. A variation of SCAN, where the disk arm only moves as far as the furthest request, then reverses direction.
2. More efficient by avoiding unnecessary movement beyond the last request.
   
C-LOOK:
1. A variation of C-SCAN, where the arm jumps back to the beginning only after servicing the furthest request.
2. Similar to LOOK but with the circular scanning pattern.


OUTPUT:
![image](https://github.com/user-attachments/assets/c4e690bd-7560-4d51-800d-4c4821d15a64)
FCSF - First Come First Serve
![image](https://github.com/user-attachments/assets/ab0a3b1d-8e77-43e1-9e83-1ce285d45856)
SSTF - Shortest Seek Time First
![image](https://github.com/user-attachments/assets/8957e140-0b1e-4011-a7ae-03a5a3238f98)
SCAN
![image](https://github.com/user-attachments/assets/d77ac393-831c-471a-9558-71598ab69220)
C-SCAN
![image](https://github.com/user-attachments/assets/489908ee-6b3d-4534-932d-b9ab69a20968)
LOOK
![image](https://github.com/user-attachments/assets/77213c25-5979-442a-8e26-bceb35105973)
C-LOOK
![image](https://github.com/user-attachments/assets/5504d5c4-b997-4a9f-a941-42be80347098)

Conclusion
This project provides a deep dive into the inner workings of disk scheduling in operating systems, offering a practical and educational tool for visualizing how different algorithms manage disk I/O operations. The simulator serves as an excellent resource for students and professionals alike to understand the impact of scheduling on system performance.

First directly download python versions like PyCharm and can run this main file to get the output.
