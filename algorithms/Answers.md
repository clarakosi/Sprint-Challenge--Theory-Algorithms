## Analysis of Algorithms

### Exercise I:

    a) O(n)
    b) O(log n)
    c) O(Math.sqrt(n))
    d) O(n log n)
    e) O(n^3)
    f) O(n)
    g) O(n)

### Exercise II:

    a) function max(a) {
    minVal=a[0]
    maxDiff = 0;
    for(let i = 0; i < a.length; i++) {
            minVal = min(minVal, a[i]);
            maxDiff = max(maxDiff, a[i]-minVal);
            return maxDiff
        }
    }


    b) Start at floor n/2 and if the egg is broken keep dividing by 2 until an egg is unbroken. Then add and divide by two the floor of the last broken and unbroken egg and follow format until you get floor f.

    However, if the egg is unbroken at n/2 then move up by adding n/2 and n then dividing by two until an egg is broken. Once an egg is broken add the new floor with the last floor of the unbroken egg and divide by two. Continue until you get to floor f.

### Exercise III:
    a & b) Both would fall under O(n log (n)) since they are both best case scenerios. 