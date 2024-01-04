# Getting Help 

* Class 16 [list algorithms](https://docs.google.com/document/d/1igj3J9fbM-vat0iPu3uc39PXeYIbzXyFGDco9q-5rq0/edit?usp=sharing) and Class 15 [whiteboard examples with answers](https://docs.google.com/document/d/1J2mML1EloTDHoIbXXb4WuJZQw4llKBgwzZd1fy50VJk/edit?usp=sharing)

* Counting common words [video lecture](https://drive.google.com/file/d/10T0cmiSTVVirozTyAPHO77GHfgHb1TL_/view?usp=sharing) and [demo code](https://replit.com/@mcarlberg/Class16ListAListB#README.md) 

* Village neighborhoods [video lecture](https://drive.google.com/file/d/1hpP3ho4Tcepv7hohfCFBbrKln58kfFYv/view?usp=sharing) and [demo code](https://replit.com/@mcarlberg/Class17VillageNeighborhoods#main.py)

* Second largest number [video lecture](https://drive.google.com/file/d/1-G_xx4Sk8P8BpU33jsr856GYYXVZ3HLE/view?usp=sharing) and [demo code](https://replit.com/@mcarlberg/Class17SecondLargest#README.md) 

* W3Schools Tutorials
    * [Accessing items](https://www.w3schools.com/python/python_lists_access.asp) in a list
    * [Looping](https://www.w3schools.com/python/python_lists_loop.asp) through lists
    * List [methods](https://www.w3schools.com/python/python_lists_methods.asp)

* Relevant [flash cards](https://drive.google.com/file/d/1eTtDb2-1MksedrCzar0WTU3Z3zGAxIgz/view?usp=sharing)

* Extended [reading](https://drive.google.com/file/d/1eFgiYFafO4PejvoHHxm1umA8bvmuLliy/view?usp=sharing)

* All [Getting Help material](https://github.com/mattcarlberg/OOP-Sp23-Reference) from previous classes




# Challenge 

Professor Firenze is studying the tides.  He is fervent about determining the difference in water level between high tide and low tide.

He measures the ocean using a somewhat unreliable sensor.  It outputs an integer once per hour for a total of twenty-four measurements each day.  Each measurement is between 1 and 100 (inclusive) with larger numbers meaning a higher water level.  

Professor Firenze will calculate the integer difference in water level between high tide and low tide by subtracting the largest number measured by the sensor and the smallest number measured by the sensor in the day. 

HOWEVER, because the sensor can be unreliable, he uses the following criteria to determine if the data for a day can actually be used:  If the measurements between the low tide reading and high tide reading are **strictly increasing**, then the data for the day is okay.  Otherwise, the data for the day is unreliable.  


# Input 

One line of text with twenty-four space-separated integers.  It is guaranteed that the maximum and minimum value are both unique AND that the minimum occurs before the maximum in the list. 

# Output

The integer difference in water level between high tide and low tide. If the sensor data for the day is not reilable, output `unreliable`.  

# Example Input 1 

If the input is 

```
30 31 29 24 18 20 26 28 31 38 41 48 49 52 55 62 71 79 87 90 94 97 88 91
```

the output should be `79` because 97 is the max at position [21] and 18 is the min at position [4] and `97 - 18 = 79` AND because the sequence from position [4] to position [21] is strictly increasing. 

# Example Input 2

If the input is 

```
20 15 7 14 15 19 20 23 24 24 30 33 39 42 41 51 55 62 50 45 44 44 43 41
```
the output should be `unreliable` because 62 is the max at position [17] and 7 is the min at position [2] BUT because the sequence from position [2] to position [17] is NOT strictly increasing.  (In particular, at positions [8] and [9], the value 24 repeats twice, and at positions [13] and [14], the values decrease from 42 to 41.)  
