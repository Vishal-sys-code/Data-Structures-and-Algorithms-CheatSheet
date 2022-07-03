# BIT MANIPULATION

Sign Bit <br>
0 -> Positive, 1 -> Negative

## **AND**

```
0 & 0 -> 0
0 & 1 -> 0
1 & 1 -> 1
```

## **OR**

```
0 | 0 -> 0
0 | 1 -> 1
1 | 1 -> 1
```

## **XOR**

```
0 ^ 0 -> 0
0 ^ 1 -> 1
1 ^ 1 -> 0
```

## **INVERT**

```
~ 0 -> 1
~ 1 -> 0
```

<hr>

## **Shifting**
```
- Left Shift
0001 << 0010 (Multiply by 2)
- Right Shift
0010 >> 0001 (Division by 2)
```
<hr>

* Count 1's of n, Remove last bit
n = n & (n-1);

* Extract last bit
n&-n or n&­~(n-1) or n^(n&­(n-1))

* n ^ n -> 0
* n ^ 0 -> n

<hr>