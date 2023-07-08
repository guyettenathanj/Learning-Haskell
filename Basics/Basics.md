Summary of https://www.youtube.com/watch?v=Vgu82wiiZ90

Haskell is a pure functional language with lazy evaluation. It is declaritive and uses immutable data types.

# Functional Purity: 
Equivalent to mathematical functions. Take in input, and return a result. They cannot manipulate the global state.

# Lazy evaluation
Only evaluates a function when needed.

# Declaritive Programming
Defines the what of the program more than the how.

https://play.haskell.org/saved/c9Yhlzup

# Example 

```Haskell
main :: IO ()
main = do
  putStrLn "Hello, World!"
  putStrLn "Hello, World!"
  let numbers = [10, 11, 12 ]
  let strings = ["x", "y", "z"]
  putStrLn $ "Sum of numbers: " ++ show (muhSum numbers)
  putStrLn $ "First was " ++ show (returnFirst strings)
  putStrLn $ "First was " ++ show (returnFirst numbers)



-- Take in Int list and return an Int
muhSum :: [Int] -> Int

-- Base case: sum of an empty list is 0
muhSum []     = 0         

-- Recursive case: add head element to 
-- the sum of the rest of the list
muhSum (first:rest) = first + muhSum rest



-- Take in list of a, and return a single element of type a
returnFirst :: [a] -> a
returnFirst (first:rest) = first
```
