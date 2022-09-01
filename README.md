# easyEvenOdd.py
Programs that determine if an integer is even or odd are a bit of a meme in programming. So I decided I would create the definitively worst, 
least efficient even / odd calculator possible. In fact it is so terrible I cannot actually write this program because this single function,
capable of determining if any integer in the Python programming language is even or odd, would likely exceed 9.22e9 gigabytes of storage! 
So instead I have included a program that will write this program for you below. Returns 
`True` if the given integer is even and `False` otherwise.

RUN IF YOU DARE!!!

```python
# Largest integer possible in python
BIG_INT =  9223372036854775807

with open('easyEvenOdd.py', 'w') as handle:
    handle.write('def isEven(num):\n')
    handle.write('\tnum=abs(num)\n')
    for i in range(BIG_INT):
        if i % 2 == 0:
            handle.write(
                f'\tif num == {i}: return True'
            )
        else:
            handle.write(
                f'\tif num == {i}: return False'
            )
        handle.write('\n')
```
