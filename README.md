# Suffix Array and Burrows-Wheeler Transform (BWT)

This repository contains implementations of two fundamental string processing algorithms: fSAIS (fast Suffix Array Induced Sorting) and BWT (Burrows-Wheeler Transform).  
## Team Members

- Keshav Khandelwal(B22ES009)
- Manthan Solanki (B22CH016)
- Soham Jadhav (B22ME061)
- Harsh Kumar (B22ES027)

## Algorithms

### 1. fSAIS (fast Suffix Array Induced Sorting)

The fSAIS algorithm efficiently constructs the suffix array of a string in linear time O(n). The resulting suffix array is useful for substring searches, longest common prefix calculation, and for generating the Burrows-Wheeler Transform.

### 2. BWT (Burrows-Wheeler Transform)

The BWT algorithm rearranges a string into a form that is more compressible, grouping similar characters together. It's a key component of many compression methods and facilitates efficient text compression and decompression.

## Usage

To use these algorithms in your project:

1. **fSAIS Algorithm**:
   - Implement the `fsais()` function to generate the suffix array of a given string.
   - Pass a string to `fsais()` to obtain its suffix array.

2. **BWT Algorithm**:
   - Implement the `bwt()` function to perform the Burrows-Wheeler Transform on a string.
   - Pass a string to `bwt()` to obtain its transformed string and index.

## Examples

### Example Usage of fSAIS and BWT

```python
from fsais import fsais

text = "banana"
suffix_array = fsais(text)
print(suffix_array)
'''
from bwt import bwt

text = "banana"
transformed_string, index = bwt(text)
print(transformed_string)
print(index)

