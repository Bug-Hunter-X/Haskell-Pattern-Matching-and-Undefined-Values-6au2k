# Haskell Pattern Matching and Undefined Values

This repository demonstrates a subtle bug in Haskell related to pattern matching and undefined values.  The bug highlights a scenario where unexpected exceptions can arise when pattern matching is applied to undefined values in a list context. 

The `bug.hs` file contains the erroneous code.  The `bugSolution.hs` file presents a corrected version that avoids the exception. 

The core problem is that the standard pattern matching approach doesn't explicitly handle undefined lists leading to runtime crashes.  The solution utilizes a more robust approach that handles such cases gracefully. 