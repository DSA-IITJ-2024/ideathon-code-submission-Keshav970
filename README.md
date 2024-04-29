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
```cpp
#include <iostream>
#include "fsais.h"

int main() {
    std::string text = "banana";
    auto suffix_array = fsais(text);
    for (auto idx : suffix_array) {
        std::cout << idx << " ";
    }
    std::cout << std::endl;
    return 0;
}

#include <iostream>
#include "bwt.h"

int main() {
    std::string text = "banana";
    auto result = bwt(text);
    std::cout << "Transformed String: " << result.first << std::endl;
    std::cout << "Index: " << result.second << std::endl;
    return 0;
}


