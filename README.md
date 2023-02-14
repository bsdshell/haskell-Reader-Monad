# haskell-Reader-Monad

# Why Reader Monad is Hard to understand
```haskell
    newtype Reader r a = Reader{runReader:: r -> a}
```

## I DO NOT understand above code
* Actually it is just a function in Haskell
```haskell
    runReader:: Reader r a -> r -> a
```

## Here is how I try to understand *Reader Monad*
```haskell
    newtype Reader Input Output = Reader{ runReader::Input -> Output}

    runReader :: Reader Input Output -> Input -> Output
```
