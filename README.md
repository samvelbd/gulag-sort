# Welcome to the Gulag Sort Repo :clipboard:

## What is Gulag Sort? :question:

### Introduction

Gulag Sort is an evolution of ![Stalin Sort by Gustavo Depaula](https://github.com/gustavo-depaula/stalin-sort). It remains an efficient sorting algorithm, serving as a systematic method for placing the elements of a random access file or an array in order. Stalin Sort is also know as the best sorting algorithm of all times because of its AMAZING capacity of always ordering an array with an O(n) performance.

### How it works?

Stalin sort iterates through the array, checking if its elements are in order. Any element that isn't in order you pull out, in other words, you send it to Gulag. Stalin sort just removes unwanted elements. Gulag sort acknowledges that those elements can still serve the Motherland, thus keeps them for later use.

### Step-by-step example

1. (1 2 5 3 5 7) -> (**1** 2 5 3 5 7) () Here the algorithm stores the first of element of the array
2. (**1** 2 5 3 5 7) -> (1 **2** 5 3 5 7) () Now it will compare the stored element with the second one, if this is bigger than the stored, it replaces the stored element by this
3. (1 **2** 5 3 5 7) -> (1 2 **5** 3 5 7) () Repeats step 2
4. (1 2 **5** 3 5 7) -> (1 2 **5** 5 7) (3) Since the 4th element is smaller than the 3rd one, the 4th element will be sent to Gulag
5. (1 2 **5** 5 7) -> (1 2 5 **5** 7) (3) Equal elements are preserved
6. **(1 2 5 5 7) (3)** Ordered array + Gulag !

### Pseudocode implementation

Keep in mind that this is pseudocode, and is just an example. We strongly encourage you to code a different approach. 

```
FUNCTION stalinSort(A : list OF sortable items)
    n := length(A)
    bigger := 0
    B SET empty list

    FOR i := 0 TO n NOT inclusive DO
        IF A[i] >= bigger THEN
          bigger := A[i]
          B.push(A[i])
        ELSE
		C.push(A[i])
        END IF
    END FOR

    RETURN B,C
END FUNCTION
```

## Want to help? :raised_hands:

Please check the [CONTRIBUTING.md](./CONTRIBUTING.md)

### Give this Project a Star! :star:

## About

Gulag sort is a serious project. It took the combined efforts of 3 engineers using a single shared neuron to be created.
