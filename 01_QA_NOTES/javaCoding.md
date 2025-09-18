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

  # Java Array Programs (logic)

1. **Copy all elements of one array into another**
    
    * Create new array `b` of same length; loop `for(i) b[i] = a[i]`; (or `System.arraycopy` / `Arrays.copyOf`).
        
2. **Frequency of each element**
    
    * Use a `HashMap<value,count>`; for each element `map.put(x, map.getOrDefault(x,0)+1)`.
        
3. **Left rotate an array**
    
    * For one position: store `temp=a[0]`, shift `a[i]=a[i+1]`, set last `a[n-1]=temp`. For k: repeat k times or use reversal algorithm.
        
4. **Print duplicate elements**
    
    * Use `HashSet` to track seen and another set to collect duplicates; or use frequency map and print keys with count&gt;1.
        
5. **Print elements of an array**
    
    * Loop `for (i=0;i<n;i++) System.out.println(a[i]);`.
        
6. **Print elements in reverse order**
    
    * Loop from `i=n-1` down to `0` and print `a[i]`.
        
7. **Print elements at even positions**
    
    * Decide 0-based or 1-based. For 0-based even indices: `for(i=0;i<n;i+=2) print a[i]`.
        
8. **Print elements at odd positions**
    
    * For 0-based odd indices: `for(i=1;i<n;i+=2) print a[i]`.
        
9. **Print largest element**
    
    * Track `max = a[0]`; loop and update `if(a[i]>max) max=a[i]`.
        
10. **Print smallest element**
    

* Track `min = a[0]`; update `if(a[i]<min) min=a[i]`.
    

11. **Number of elements present**
    

* Use `array.length` (for dynamic lists use `list.size()`).
    

12. **Sum of all items**
    

* Accumulate `sum += a[i]` in a loop (use `long` for large sums).
    

13. **Right rotate elements**
    

* For one position: store `temp=a[n-1]`, shift right, set `a[0]=temp`. For k: repeat or use reversal method.
    

14. **Sort ascending**
    

* Use `Arrays.sort(a)` or implement any sorting algorithm (quick, merge).
    

15. **Sort descending**
    

* Sort ascending then reverse, or use `Arrays.sort` with comparator for objects; or implement sort with `>` comparison.
    

16. **Find 3rd largest number**
    

* Maintain three largest variables while scanning, or sort and pick `a[n-3]` (handle duplicates as needed).
    

17. **Find 2nd largest number**
    

* Track `first` and `second` largest while scanning once.
    

18. **Find largest number**
    

* Same as (9).
    

19. **Find 2nd smallest number**
    

* Maintain two smallest variables while scanning, or sort and take `a[1]` (care with duplicates).
    

20. **Find smallest number**
    

* Same as (10).
    

21. **Remove duplicate elements**
    

* Use `LinkedHashSet` to preserve order: `new ArrayList<>(new LinkedHashSet<>(Arrays.asList(...)))`; or two-pointer on sorted array.
    

22. **Print odd and even numbers from an array**
    

* Loop and check `if (a[i] % 2 == 0) evens.add(a[i]) else odds.add(a[i])`.
    

23. **How to sort an array**
    

* Use built-in `Arrays.sort(a)` for primitives/objects; or implement bubble/selection/quick/merge.
    

---

# Java Matrix Programs (logic)

1. **Java Matrix Programs (general)**
    
    * Represent as `int[][] m = new int[r][c]`. Use nested loops `for(i) for(j)` to traverse.
        
2. **Add two matrices**
    
    * Check same dimensions; `res[i][j] = a[i][j] + b[i][j]`.
        
3. **Multiply two matrices**
    
    * For `res[i][j] = sum over k of a[i][k] * b[k][j]`. Validate `aCols == bRows`.
        
4. **Subtract two matrices**
    
    * `res[i][j] = a[i][j] - b[i][j]`.
        
5. **Determine whether two matrices are equal**
    
    * Same dims and every `a[i][j] == b[i][j]`.
        
6. **Display lower triangular matrix**
    
    * For each `i,j` print `a[i][j]` if `i >= j` else print `0` or skip.
        
7. **Display upper triangular matrix**
    
    * Print `a[i][j]` if `i <= j` else `0`.
        
8. **Frequency of odd & even numbers in matrix**
    
    * Loop all entries, increment odd/even counters using `%2`.
        
9. **Product of two matrices**
    
    * Same as (3) — matrix multiplication.
        
10. **Sum of each row and each column**
    

* For rows: loop `i` sum across j. For columns: loop `j` sum across i.
    

11. **Transpose of a matrix**
    

* `res[j][i] = a[i][j]`. For square matrix can swap in-place.
    

12. **Check if identity matrix**
    

* For square `n`: diagonal `a[i][i]==1` and off-diagonal `a[i][j]==0`.
    

13. **Check if sparse matrix**
    

* Count zeros; if zeros &gt; (rows\*cols)/2 → sparse.
    

14. **Transpose matrix**
    

* Same as (11).
    

---

# Java String Programs (logic)

1. **Count total number of characters in a string**
    
    * Use `str.length()` (counts all characters). For excluding spaces use `str.replace(" ", "").length()`.
        
2. **Count total number of characters in a string 2**
    
    * Possibly counting unique characters: use `Set<Character>` and add all chars.
        
3. **Count punctuation characters in a string**
    
    * Loop chars and check `if (!Character.isLetterOrDigit(c) && !Character.isWhitespace(c)) count++`.
        
4. **Count vowels and consonants**
    
    * Loop chars; if `Character.isLetter(c)` then check `aeiou` vs consonant; maintain counts.
        
5. **Determine whether two strings are anagrams**
    
    * Normalize (lowercase, remove spaces), sort both char arrays and compare, or count char frequencies.
        
6. **Divide a string into N equal parts**
    
    * If `len % n == 0` then chunk size `len/n`; slice substrings of that size.
        
7. **Find all subsets of a string**
    
    * Use bitmask from `0` to `2^n - 1` and include characters where bit is set.
        
8. **Find longest repeating sequence in a string**
    
    * Use suffix array/DP or sliding window; simpler: for each start, extend and track longest adjacent repeats.
        
9. **Find all permutations of a string**
    
    * Use recursion/backtracking swapping chars or use Heap’s algorithm.
        
10. **Remove all white spaces from a string**
    

* `str.replaceAll("\\s+", "")`.
    

11. **Replace lower-case with upper and vice-versa**
    

* Loop chars: if `Character.isUpperCase(c)` convert to `toLowerCase`, else toUpperCase.
    

12. **Replace spaces with specific character**
    

* `str.replace(' ', ch)` or `replaceAll("\\s+", String.valueOf(ch))`.
    

13. **Check if a string is palindrome**
    

* Compare with reversed string, or two-pointer scan `i` and `j`.
    

14. **Check if one string is rotation of another**
    

* If lengths equal and `s2` is substring of `s1+s1` then rotation.
    

15. **Find max and min occurring character**
    

* Count frequency array of size 256 or map, then find char with max/min count (skip zeros for min).
    

16. **Reverse of the string**
    

* Use `new StringBuilder(str).reverse().toString()` or manual loop.
    

17. **Find duplicate characters in a string**
    

* Frequency map, print chars with count&gt;1.
    

18. **Find duplicate words in a string**
    

* Split on whitespace to words, use `HashMap<String,Integer>` to count words and print counts&gt;1.
    

19. **Find frequency of characters**
    

* Use `int[256]` or `Map<Character,Integer>` and count.
    

20. **Find largest and smallest word in a string**
    

* Split into words; track longest and shortest by `length()`.
    

21. **Find most repeated word in a text file**
    

* Read file, split into words, count with map, then find max entry.
    

22. **Find number of words in a text file**
    

* Read file and split on whitespace, count tokens (careful with punctuation).
    

23. **Separate individual characters from a string**
    

* Loop `for (char c : str.toCharArray())` and store/print.
    

24. **Swap two string variables without third variable**
    

* `a = a + b; b = a.substring(0, a.length()-b.length()); a = a.substring(b.length());` (or use char arrays).
    

25. **Print smallest and biggest possible palindrome word in given string**
    

* Interpret: find substrings that are palindromes; pick shortest and longest palindrome substrings.
    

26. **Reverse string word by word**
    

* Split into words, reverse array of words, join with spaces.
    

27. **Reverse string without reverse() function**
    

* Build new string by iterating from `len-1` to `0` and appending characters.
    

---

# Java Searching & Sorting Programs (logic)

1. **Linear Search**
    
    * Loop `for(i) if(a[i]==key) return i;` else -1.
        
2. **Binary Search**
    
    * Array must be sorted. Use low/high pointers, mid = (low+high)/2, compare and adjust.
        
3. **Bubble Sort**
    
    * Repeated passes swapping adjacent out-of-order elements; optimization: stop if no swaps in a pass.
        
4. **Selection Sort**
    
    * For each position i, find min from i..n-1 and swap with i.
        
5. **Insertion Sort**
    
    * Build sorted portion by inserting `a[i]` into correct place in `0..i-1`.
        

---

# Java Conversion Programs (logic)

1. **String → int**: `Integer.parseInt(str)` or `Integer.valueOf(str)`.
    
2. **int → String**: `String.valueOf(i)` or `Integer.toString(i)`.
    
3. **String → long**: `Long.parseLong(str)`.
    
4. **long → String**: `String.valueOf(l)`.
    
5. **String → float**: `Float.parseFloat(str)`.
    
6. **float → String**: `String.valueOf(f)`.
    
7. **String → double**: `Double.parseDouble(str)`.
    
8. **double → String**: `String.valueOf(d)`.
    
9. **String → Date**: use `SimpleDateFormat` (`new SimpleDateFormat(pattern).parse(str)`).
    
10. **Date → String**: `new SimpleDateFormat(pattern).format(date)`.
    
11. **String → char**: `str.charAt(index)` or `str.toCharArray()`.
    
12. **char → String**: `String.valueOf(ch)`.
    
13. **String → Object**: The string is already an `Object`; cast: `Object o = (Object) str`.
    
14. **Object → String**: `String s = obj.toString()` (handle null).
    
15. **int → long**: implicit cast `long l = i;` or `(long)i`.
    
16. **long → int**: cast `int i = (int) l;` (may lose data).
    
17. **int → double**: `double d = i;`.
    
18. **double → int**: `int i = (int) d;` (truncation).
    
19. **char → int**: `int code = (int) ch;`.
    
20. **int → char**: `char c = (char) i;`.
    
21. **String → boolean**: `Boolean.parseBoolean(str)` (`"true"` → true).
    
22. **boolean → String**: `String.valueOf(flag)`.
    
23. **Date → Timestamp**: `new java.sql.Timestamp(date.getTime())`.
    
24. **Timestamp → Date**: `new Date(timestamp.getTime())`.
    
25. **Binary → Decimal**: parse with base `2`: `Integer.parseInt(binStr, 2)`.
    
26. **Decimal → Binary**: `Integer.toBinaryString(n)`.
    
27. **Hex → Decimal**: `Integer.parseInt(hexStr, 16)`.
    
28. **Decimal → Hex**: `Integer.toHexString(n)`.
    
29. **Octal → Decimal**: `Integer.parseInt(octStr, 8)`.
    
30. **Decimal → Octal**: `Integer.toOctalString(n)`.
    

---

# Java Pattern Programs (logic)

1–16) **Various printed patterns (spiral, triangle, diamond, palindromic, etc.)**

* General approach: use nested loops (rows/columns).
    
* Compute number of spaces and characters per row based on pattern formula.
    
* Spiral: maintain `top, bottom, left, right` boundaries and traverse in 4 directions updating boundaries.
    
* For symmetric patterns, use `Math.abs` or two halves approach.
    
* For numeric patterns, compute values per position (e.g., increasing, decreasing, row-based increments).
    

(If you want specific ASCII patterns, give one example and I’ll provide exact loop logic.)

---

# Java Singly Linked List Programs (logic)

1. **Singly linked list Examples**
    
    * Node with `data` and `next`. Perform standard operations.
        
2. **Create and display a singly linked list**
    
    * Build nodes linking `next`; traverse from `head` printing `data`.
        
3. **Create n nodes and count nodes**
    
    * Insert n times; to count traverse and increment counter.
        
4. **Display list in reverse order**
    
    * Recursion: print `printReverse(`[`node.next`](http://node.next)`)` then `print` [`node.data`](http://node.data); or push to stack then pop.
        
5. **Delete node from beginning**
    
    * `head =` [`head.next`](http://head.next).
        
6. **Delete node from middle**
    
    * Traverse to node before target and adjust [`prev.next`](http://prev.next) `=` [`target.next`](http://target.next).
        
7. **Delete node from end**
    
    * Traverse to second-last node and set its `next = null`.
        
8. **Check if list is palindrome**
    
    * Find middle (fast/slow), reverse second half, compare halves, optionally restore.
        
9. **Find max and min value node**
    
    * Traverse and track `max` and `min`.
        
10. **Insert new node at middle**
    

* Find middle index using slow/fast or size/2, insert by pointer adjustments.
    

11. **Insert at beginning**
    

* New node's `next = head`; `head = newNode`.
    

12. **Insert at end**
    

* Traverse to last and [`last.next`](http://last.next) `= newNode`.
    

13. **Remove duplicate elements**
    

* Use `HashSet` to track seen values; adjust links to skip duplicates.
    

14. **Search an element**
    

* Traverse and compare each node's data.
    

---

# Java Circular Linked List Programs (logic)

1. **Create & display a Circular Linked List**
    
    * Last node `next` points to `head`. Traverse with do-while to avoid infinite loop.
        
2. **Create N nodes and count**
    
    * Insert while maintaining circular links; to count, start at head and loop until back to head.
        
3. **Display reverse**
    
    * Harder in single-link circular: collect nodes in stack during traversal, then pop to print.
        
4. **Delete from beginning**
    
    * If single node: `head = null`; else set [last.next](http://last.next) = [head.next](http://head.next) and `head =` [`head.next`](http://head.next).
        
5. **Delete from end**
    
    * Find node before last, set its `next = head`.
        
6. **Delete from middle**
    
    * Traverse to previous node of target and adjust link.
        
7. **Find max and min node**
    
    * Traverse circularly scanning `data`.
        
8. **Insert at beginning**
    
    * Create node, set [node.next](http://node.next) = head, update [last.next](http://last.next) = node, head = node.
        
9. **Insert at end**
    
    * Create node, set [last.next](http://last.next) = node, [node.next](http://node.next) = head.
        
10. **Insert at middle**
    

* Find position using count/2 and insert similarly to singly list.
    

11. **Remove duplicates**
    

* Use set to detect duplicates while traversing and remove by relinking.
    

12. **Search an element**
    

* Traverse until back to head; check each node.
    

13. **Sort circular linked list**
    

* Break circularity, apply sorting (e.g., merge sort on linked list), then re-link circularly.
    

---

# Java Doubly Linked List Programs (logic)

1. **Convert binary tree to doubly linked list**
    
    * In-order traversal linking nodes to previous; use recursion to thread nodes.
        
2. **Create doubly linked list from ternary tree**
    
    * Flatten tree (pre/in/post order) and link nodes with `prev` and `next`.
        
3. **Create n nodes and count**
    
    * Standard insert operations, count by traversing `next`.
        
4. **Display in reverse order**
    
    * Traverse to tail, then follow `prev` pointers printing data.
        
5. **Create and display doubly linked list**
    
    * Insert nodes with `next` and `prev`, then traverse from head.
        
6. **Delete node from beginning**
    
    * `head =` [`head.next`](http://head.next)`; head.prev = null;`
        
7. **Delete node from end**
    
    * Move to tail `tail = tail.prev;` [`tail.next`](http://tail.next) `= null;`
        
8. **Delete node from middle**
    
    * Adjust [`prev.next`](http://prev.next) `= next` and `next.prev = prev`.
        
9. **Find max and min node**
    
    * Traverse and keep track of values.
        
10. **Insert at beginning**
    

* New node's `next = head; head.prev = new; head = new`.
    

11. **Insert at end**
    

* Append after tail, set pointers.
    

12. **Insert at middle**
    

* Locate position then link new node between `prev` and `next`.
    

13. **Remove duplicates**
    

* Use set of values while traversing, unlink duplicates updating both `prev` and `next`.
    

14. **Rotate doubly linked list by N nodes**
    

* Move `head` to [`head.next`](http://head.next) N times or adjust `head` and `tail` pointers appropriately.
    

15. **Search an element**
    

* Traverse either forward or backward and compare.
    

16. **Sort elements**
    

* Use merge sort tailored for linked lists (efficient, O(n log n)).
