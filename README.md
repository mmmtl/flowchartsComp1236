# flowchartsComp1236
```mermaid
flowchart TB
    A([Start])
    A-->B[/initialPosition = input initial position
    range = input amount of numbers
    x = input positive integer
    maxSum = input maximum sum output
    /]
    B-->D[squareSum = 0]
    D-->E{Is initialPosition <= range?}
    E-- yes -->F[squareNum = initialValue**2
    oddNum = squareNum % 2
    factorX = x % squareNum
    consNum = initialPosition + 1 ** 2]
    F-->G{is oddNum = 1}
    G--yes-->H[/print squareNum/]
    H-->I{is factorX = 0}
    I--yes-->J[/print squareNum is factor of x/]
    J-->K{is squareSum < maxSum}
    K--yes-->L[squareSum = squareNum + consNum // squareSum = squareNum + initialPosition + 1 ** 2]
    L-->M[/print squareSum/]
    M-->N(End)

```

Pseudocode
set initialValue = input initial value
set range = input range
set x = input positive integer

while initialValue <= range
    let squareNum = initialValue ** 2
    let oddNum = squareNum % 2
    let factor = x % squareNum
    let consNum = (initialValue + 1)**2
     
    if oddNum = 1
        print squareNum
    endif
    
    if initialValue < range
        let sumNum = squareNum + consNum
        print sumNum
    endif

    if factor = 0
        print "Yes, squareNum is a factor x."
    endif
    
    let initialValue = initialValue + 1

endwhile
    

    

