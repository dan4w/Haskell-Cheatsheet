# Haskell-Cheatsheet
To Do: Formatting


Arithmetic

2+15
> 17

2-15
> -13

2+(-15)
> -13

49*100
>4900

5/2
> 2.5

div 5 2
> 2

5 `div` 2
> 2

2+4*3
> 14

Only div 5 2 and 5 `div` 2 act like integer arithmetic in other languages.

Watch out for

5* -3  won't work, must do 5*(-3)

Boolean:
&& and
|| or

True && True
> True

True && False
> False

True || True
> True

True || False
> True

Interesting:
not False
> True

== is equal to

/= is not equal to

5==5 -> true

5/=5 -> false

1==0 -> false

5/=4 -> true



C++ Function calls

someFunction(parameter1, parameter2)


Haskell Function calls

someFunction parameter1 parameter2

Some built in functions

succ - returns the successor

succ 8 => 9


min - returns the lower of the two

min 2 10 => 2


max - returns the larger of the two

max 2 10 => 10


Functions has the highester priority
    ghci> succ 9 + max 5 4 + 1  
    16  
    ghci> (succ 9) + (max 5 4) + 1  
    16  
    
If a function takes 2 parameters we can call it using backticks

div 5 2 becomes 5 `div` 2


Function order doesnt matter, you can call a function that calls another function even if the 2nd function is after the first one.
