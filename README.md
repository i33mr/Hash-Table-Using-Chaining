# Hash-Table-Using-Chaining
This program uses a hash function to decide where to place each element (emails in this case) in the
array. Whenever collision occurs between different elements, they are placed in a
linked list, pointed to by the key. The program also shows the number of collusions occured, inserting and search durations.

In this program, the following hash function is used:

![image](https://user-images.githubusercontent.com/68453742/124392999-00058680-dd01-11eb-97bf-2a5aad11ccb4.png)

where s is an array of characters in an email, P is the prime number 67, m is the
length of the email, and M is the table size.

The number 67 was chosen as our prime number to reduce collisions. Although it is
closer to a power of 2 compared to other prime numbers, experimentally, it produced
far fewer collisions and better distribution with our dataset.

3 sets of randomized emails were used, A, B, and C,with sizes 100,
100000, and 500000, respectively
The format is as follows.
[A-Za-z0-9]{5}\.[A-Za-z0-9]{5}@[A-Za-z]{5}\.(com|net|org)

Set A: 

![image](https://user-images.githubusercontent.com/68453742/124393085-6d191c00-dd01-11eb-8373-03d2edcbefff.png)

Set B: 

![image](https://user-images.githubusercontent.com/68453742/124393104-8b7f1780-dd01-11eb-93ef-91e8d85ac500.png)

Set C:

![image](https://user-images.githubusercontent.com/68453742/124393115-9cc82400-dd01-11eb-97de-284b14be6416.png)

Note: the targeted are randomly chosen from the specified set. 
