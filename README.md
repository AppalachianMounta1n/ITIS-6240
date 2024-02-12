# About This Repository
This repository is for storing and collaborating on the project files for ITIS 6140 (Applied Cryptography) at UNC Charlotte for Spring 2024.
### Group Members
- [Lily Gross](https://github.com/AppalachianMounta1n)
- [Ryan Braswell](https://github.com/braswellry67)
- [Reed Holz](https://github.com/reedholz)

***
## AES Implementation - Due 2/9/2024
The base file [aesO.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/AES%20Implementation/aesO.c) was provided by the professor, Dr. Yongge Wang. The updated file [aesO-Efficient.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/AES%20Implementation/aesO%20-%20Efficient.c) is the project file where our code is being updated to optimize the performance of the original program.

### Relevant Files
- [aesO.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/AES%20Implementation/aesO.c)
- [aesO-Efficient.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/AES%20Implementation/aesO%20-%20Efficient.c)

### Changes
- The first improvement we made was unrolling as many loops as possible. By doing this, we removed the overhead of storing loop info and only had to run the code for the operations performed. While this is not ideal for code readability, it is able to provide small performance boosts to the runtime if done on a large enough scale.
- The second improvement we made was updating the encryption process to utilize the benefits of a 64-bit processor rather than only functioning at a 32-bit level. This allowed for a more efficient runtime do to having more memory and ability to run concurent processes.

### Resulting Runtime Improvements
- Encryption runtime was improved by a total of 35.36%
- Decryption runtime was improved by a total of 3.45%
- The overal runtime, including encryption and decryption, was improved by 10.01%

***
## SHA Implementation - Due 2/23/2024
The base file [shaO.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/SHA%20Implementation/shaO.c) was provided by the professor, Dr. Yongge Wang. The updated file [shaO-Efficient.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/SHA%20Implementation/shaO-Efficient.c) is the project file where our code is being updated to optimize the performance of the original program.

### Relevant Files
- [shaO.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/SHA%20Implementation/shaO.c)
- [shaO-Efficient.c](https://github.com/AppalachianMounta1n/ITIS-6240-Projects/blob/main/SHA%20Implementation/shaO-Efficient.c)

### Changes
- The loops in processing functions were all unrolled to remove the overhead of running loops. By doing this, the code was made significantly less readable (it went from not quite 500 lines to nearly 3000 lines) but the efficiency was drastically increased. We expected a 1% to 5% runtime increase for each set of 100 runs for SHA1, SHA256, and SHA512, but the end result was closer to a 45% improvement for each just from unrolling loops that ran a fixed set of times.

### Resulting Runtime Improvements
- 

***
## OpenSSL Project - Due 3/22/2024


***
## VPN Project - Due 4/12/2024


***
## Research Paper - Due 4/29/2024