#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n), since we increment a by n^2 which needs to happen n times before we hit the conditional


b) O(n log(n)), since we are looping n times and mulitply j by two inside the while loop, which will take log2(n) times before we hit the conditional


c) O(n), function will be recursively called n times.

## Exercise II
Essentialy a basic binary search algorithm with some modifications
The floor we are looking for is not special in itself, but is characterised by being next to a floor which doesn't pass our check, thus we are looking for a pair of floors next to each other, one of which would pass the check and the other one wouldn't.
Runtime complexity is log2(n)
```
def findFloor(n):
    if n<=0:
        return = 0
    if n==1:
        return = 1  // This is just guesswork on my side since the task doesn't specify if the "f" floor is always in the set
    found = false
    start = 0
    end = n
    while not found:
        middle = (start+end)//2     // checking neighboring floors, if lower doesn' check and higher checks, the higher one is our answer
        check middle
        check middle - 1
        if last 2 are different:
            found = true
            return middle
        if egg broke on middle:
            end = middle
        else:
            start = middle
```