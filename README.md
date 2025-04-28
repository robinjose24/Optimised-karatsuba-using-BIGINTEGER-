# Optimized Karatsuba Multiplication (with Benchmarking)
-----------------------------------------------------------------
This project implements an optimized hybrid multiplication algorithm in Java, combining:

Karatsuba Multiplication (for large numbers)

Normal Grade-School Multiplication (for small numbers)

The algorithm dynamically switches between methods based on the size of the input numbers, ensuring faster and more efficient multiplication.

<br>
## Project Structure

karatBig2.java —
Basic implementation that multiplies two big integers using hybrid Karatsuba and measures execution time for a single run.

karatBig2Bench.java —
Extended version that benchmarks both multiplication methods by running them 10 times and calculating the average execution time for better accuracy.

<br>
# Features

**Dynamic Threshold Switching:** Automatically switches between Karatsuba and Normal multiplication when numbers are small enough.

**Execution Time Measurement:** Tracks and displays the time taken by both methods in milliseconds.

**Benchmarking:** Smooths out random fluctuations in timing by running multiple iterations.

**Accurate BigInteger Support:** Works seamlessly for extremely large numbers.

<br>
# 📈 Observations
Execution time was recorded for various input sizes (small to very large numbers).

For smaller inputs, Normal multiplication can sometimes outperform due to less overhead.

For larger inputs, Karatsuba multiplication consistently outperforms the normal method.

(Observation data is added in the below table)...
/=================================================
No.Of Digits	Traditional method	Karatsuba method
/-------------------------------------------------
10	          0.125	              0.233
50	          0.825	              1.047
100	          1.6113	            2.077
200	          2.476	              3.529
300	          3.417	              7.177
400	          7.840	              11.060
500	          7.433	              6.352
1000	        14.118	            12.262
2000	        66.648	            24.953
5000	        399.722	            157.039
6000	        522.017	            136.031
8000	        929.286	            184.928
10000	        1414.662	          336.260
/=================================================

<br>
# 🔮 Future Plans
Build a web-based frontend that:

Lets users input two large numbers.

Performs multiplication using both methods via a Java backend.

Visually compares the execution times in real-time

<br>
# 🛠 How to Run

Compile the Java files:

javac karatBig2.java
javac karatBig2Bench.java
Run:

java karatBig2
or

java karatBig2Bench
/------------------------------------------------------------------
Input two large numbers when prompted.

<br>
# 📋 Requirements
Java 8 or above

(Optional) IDE like IntelliJ IDEA, Eclipse, or VSCode with Java extension.

<br>
# 📜 License
This project is licensed under the MIT License 
