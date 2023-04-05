# Prompts that GPT-4 got wrong

## What does the following codeblock do

### Code

```python
for i in range(10):
  print(i)
  i = 5
print(i)
```

- Source : **Python Brain Teasers**

## GPT-4 answer

The provided code is a simple Python script that uses a for loop to iterate through a range of numbers from 0 to 9 (10 numbers in total). The loop prints the value of the variable i and then attempts to assign the value 5 to it. After the loop, the value of i is printed again.

However, it's important to note that the assignment i = 5 inside the loop doesn't affect the next value of i in the loop iteration. This is because the for loop in Python internally manages the value of the loop variable i. In each iteration, it will take the next value from the specified range, regardless of any changes made to i inside the loop.

Here is the output of the code:

```text
0
1
2
3
4
5
6
7
8
9
9

```

## Actual Answer

```text
0
1
2
3
4
5
6
7
8
9
5

```

## Correct Explanation

TODO

### Updated on 04-Apr-2023
