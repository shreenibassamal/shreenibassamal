# 🟢 Java Basic Programs

1. **Fibonacci Series in Java**
    
    * Start with `a=0, b=1`.
        
    * Next term = `a+b`.
        
    * Update: `a=b, b=next`.
        
    * Repeat till required terms.
        
2. **Prime Number Program in Java**
    
    * A number `n` is prime if it’s divisible only by `1` and `n`.
        
    * Check divisibility from `2` to `√n`.
        
    * If divisible → not prime.
        
3. **Palindrome Program in Java**
    
    * Reverse the number/string.
        
    * Compare with original.
        
    * If equal → palindrome.
        
4. **Factorial Program in Java**
    
    * Factorial = product of numbers from `1` to `n`.
        
    * Recursive: `fact(n) = n * fact(n-1)`.
        
    * Iterative: multiply in loop.
        
5. **Armstrong Number in Java**
    
    * Count digits of number.
        
    * Take each digit → raise to power (digits).
        
    * Sum them → compare with number.
        
6. **How to Generate Random Number in Java**
    
    * Use `Math.random()`.
        
    * Or `Random` class: `new Random().nextInt(bound)`.
        
7. **How to Print Pattern in Java**
    
    * Use nested loops.
        
    * Outer loop → rows.
        
    * Inner loop → columns/symbols.
        
8. **How to Compare Two Objects in Java**
    
    * Override `equals()` in class.
        
    * Compare fields inside `equals()`.
        
9. **How to Create Object in Java**
    
    * Using `new` keyword → `ClassName obj = new ClassName();`
        
10. **How to Print ASCII Value in Java**
    

* Convert char to int.
    
* Example: `int ascii = (int) 'A';`.
    

---

# 🟢 Java Number Programs

1. **Reverse a Number**
    
    * Initialize `rev=0`.
        
    * Extract last digit `n%10`.
        
    * `rev = rev*10 + digit`.
        
    * Remove last digit `n/=10`.
        
2. **Convert Number to Word**
    
    * Extract digits.
        
    * Map each digit to word using array (`zero, one…`).
        
    * Print sequentially.
        
3. **Automorphic Number**
    
    * Square the number.
        
    * Check if square ends with number.
        
4. **Peterson Number**
    
    * Sum of factorial of digits = number.
        
5. **Sunny Number**
    
    * If `n+1` is a perfect square → Sunny Number.
        
6. **Tech Number**
    
    * Split number into 2 halves.
        
    * Sum them.
        
    * Square of sum = original number.
        
7. **Fascinating Number**
    
    * Concatenate `n, n*2, n*3`.
        
    * Contains all digits `1–9` exactly once.
        
8. **Keith Number**
    
    * Use digits of number as initial sequence.
        
    * Generate next terms = sum of previous digits.
        
    * If sequence reaches number → Keith.
        
9. **Neon Number**
    
    * Square number.
        
    * Sum digits of square.
        
    * If equals number → Neon.
        
10. **Spy Number**
    

* Sum of digits = Product of digits.
    

11. **ATM Program Java**
    

* Menu-driven (Deposit, Withdraw, Check Balance).
    
* Update balance accordingly.
    

12. **Autobiographical Number**
    

* A number is autobiographical if count of digit `i` = digit at position `i`.
    

13. **Emirp Number**
    

* Prime number whose reverse is also prime.
    

14. **Sphenic Number**
    

* Positive integer = product of 3 distinct prime numbers.
    

15. **Buzz Number**
    

* Ends with 7 OR divisible by 7.
    

16. **Duck Number**
    

* Contains zero(s) but does not start with zero.
    

17. **Evil Number**
    

* Binary representation has even number of `1`s.
    

18. **ISBN Number**
    

* Weighted sum of digits (check digit verification).
    

19. **Krishnamurthy Number**
    

* Same as Strong Number (sum of factorial of digits = number).
    

20. **Bouncy Number**
    

* Digits neither in increasing nor in decreasing order.
    

21. **Mystery Number**
    

* Number that can be expressed as sum of a number and its reverse.
    

22. **Smith Number**
    

* Composite number.
    
* Sum of digits = sum of digits of prime factors.
    

23. **Strontio Number**
    

* Multiply number by 2.
    
* Middle digits are same.
    

24. **Xylem and Phloem Number**
    

* Sum of extreme digits = Sum of middle digits.
    

25. **nth Prime Number**
    

* Generate primes in sequence until nth prime is reached.
    

26. **Alternate Prime Numbers**
    

* Generate primes.
    
* Print only alternate ones.
    

27. **Square Root Without sqrt()**
    

* Use **binary search** or **Newton Raphson method**.
    

28. **Swap Numbers (Bitwise)**
    

* `a = a ^ b; b = a ^ b; a = a ^ b;`
    

29. **GCD of Two Numbers**
    

* Use Euclidean algorithm:
    
* `gcd(a,b) = gcd(b, a % b)`
    

30. **Largest of Three Numbers**
    

* Use if-else OR Math.max().
    

31. **Smallest of Three (Ternary)**
    

* `min = (a < b) ? (a < c ? a : c) : (b < c ? b : c);`
    

32. **Check Positive or Negative**
    

* If `n >= 0` → Positive else Negative.
    

33. **Perfect Square**
    

* Find sqrt (integer).
    
* If `sqrt*sqrt == n` → Perfect Square.
    

34. **Even Numbers 1–100**
    

* Loop from 1–100.
    
* If `i % 2 == 0` → print.
    

35. **Odd Numbers 1–100**
    

* Loop from 1–100.
    
* If `i % 2 != 0` → print.
    

36. **Sum of Natural Numbers**
    

* Formula: `n*(n+1)/2`.
    
* Or use loop to sum.
