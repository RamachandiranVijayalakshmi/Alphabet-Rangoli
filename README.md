# Alphabet Rangoli
- You are given an integer,N.
- Your task is to print an alphabet rangoli of size N.
- Rangoli is a form of Indian folk art based on creation of patterns.
- The center of the rangoli has the first alphabet letter a, and the boundary has the N alphabet letter (in alphabetical order).
## sample code
```
for i in range(n):
        s = "-".join(chr(ord('a')+n-j-1) for j in range(i+1))
        print((s+s[::-1][1:]).center(n*4-3, '-'))
for i in range(n-1):
        s = "-".join(chr(ord('a')+n-j-1) for j in range(n-i-1))
        print((s+s[::-1][1:]).center(n*4-3, '-'))
```
## Example Output
```
Enter the rows:4
------d------
----d-c-d----
--d-c-b-c-d--
d-c-b-a-b-c-d
--d-c-b-c-d--
----d-c-d----
------d------
```
