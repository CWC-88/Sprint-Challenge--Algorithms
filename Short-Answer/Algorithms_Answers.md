#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)

 a = 0
    while (a < n * n * n):
      a = a + n * n

      while a is less than n cubed 
      a is equal to a plus n squared

runtime will grow at a slower rate the more that n grows thus O(logn)



b)

sum = 0    ====> O(1)
    for i in range(n):   ===> O(n)
      j = 1     ====>  O(1)
      while j < n:     =====>O(1)
        j *= 2         =====>O(1)
        sum += 1       =====>O(1)

biggest term = O(n)



c)


def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)


      O(n) 

      as n bunnies grows you add 2 even though -1

      thus runtime increases at same rate


## Exercise II


Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.


assuming floors are integers only

1. take buiding and divide in half
2. toss egg off top of half building 
3. if break divide half building by half
4. if break repeat until no break
5. if no break take a half of building and divide in half and add to existing building and toss egg if break repeat step 4 and 5 until a value between break and no break is achieved 


