* [Problems/](Problems/)
  - [CTCI.md](Problems/CTCI.md)
  - [DP PATTERNS.md](Problems/DP_PATTERNS.md)
  - [GRIND.md](Problems/GRIND.md)
  - [NEETCODE.md](Problems/NEETCODE.md)
  - [PARETO.md](Problems/PARETO.md)


📓 Data Structure & Algorithm Notes
===================================


---


🎭 [Abstract Data Types](https://en.wikipedia.org/wiki/Abstract_data_type) (Interfaces)
------------------------

<details><summary><a href="https://en.wikipedia.org/wiki/Array_(data_type)"><b>Array</b></a> <i>(Abstract Interface)</i></summary>

* _Abstract Data Types_
  - [Associative Array / Map](https://en.wikipedia.org/wiki/Associative_array)
  - [Set](https://en.wikipedia.org/wiki/Set_(abstract_data_type))
* _Concrete Data Types_
  - [Array](#arrays)
  - [Hash Table](https://en.wikipedia.org/wiki/Hash_table)
  - [Linked List](#linked-list)
  - [Search Tree](https://en.wikipedia.org/wiki/Search_tree)
</details>


<details><summary><a href="https://en.wikipedia.org/wiki/Collection_(abstract_data_type)"><b>Collection</b></a></summary></details>


<details><summary><a href="https://en.wikipedia.org/wiki/List_(abstract_data_type)"><b>List</b></a></summary>

* _Concrete Data Structures_
  - [Array](#arrays)
  - [Balanced Tree](https://en.wikipedia.org/wiki/Self-balancing_binary_search_tree)
  - [Dynamic Array](#arrays)
  - [Hashed Array Tree](https://en.wikipedia.org/wiki/Hashed_array_tree)
  - [Linked List](#linked-list)
  - [Random Access List](https://docs.racket-lang.org/ralist/index.html)
</details>


<details><summary><a href="https://en.wikipedia.org/wiki/Queue_(abstract_data_type)"><b>Queue</b></a></summary></details>


<details><summary><a href="https://en.wikipedia.org/wiki/Stack_(abstract_data_type)"><b>Stack</b></a></summary>

* Last in, first out (LIFO)
* Operations
  - `push` (aka. `append`)
  - `pop`
* Useful for tasks divided into sub-tasks
  - Tracking tokens while parsing
* Concrete Implementation
  - [Dynamic Array](#arrays)
  - [Linked List](#linked-list)
</details>


---


🧑‍🏭 [Algorithms](https://en.wikipedia.org/wiki/Algorithm)
---------------

### [Backtracking](https://en.wikipedia.org/wiki/Backtracking)

* Incrementally builds candidate solutions & backtracks/abandons candidate when it's no longer viable.
* Ideal for [constraint satisfaction problems](https://en.wikipedia.org/wiki/Constraint_satisfaction_problem).
  - [Crossword](https://en.wikipedia.org/wiki/Crosswords)
  - [Eight Queens](https://en.wikipedia.org/wiki/Eight_queens_puzzle)
  - [Graph/Map Coloring](https://en.wikipedia.org/wiki/Graph_coloring)
  - [Sudoku](https://en.wikipedia.org/wiki/Sudoku_solving_algorithms)


### [Sorting](https://en.wikipedia.org/wiki/Sorting_algorithm)

- [__Comparison-based__](https://en.wikipedia.org/wiki/Comparison_sort)
  * Determines if "key" is less, equal, or greater than another.
  * Typical sorting algorithm in standard libraries.
  * Most optimal worst-case time complexity: `O(n log n)`
  * [_Heapsort_](https://en.wikipedia.org/wiki/Heapsort)
    - In-place; unstable
    - Slower than quicksort in practice.
    - Time complexity
      * Best: `O(n)` equal keys; `O(n log n)` distinct keys
      * Average / Worst: `O(n log n)`
    - Auxiliary space complexity
      * Worst: `O(1)`
  * [_Quicksort_](https://en.wikipedia.org/wiki/Quicksort)
    - Divide-and-conquer / recursive algorithm; typically unstable.
    - Ideal pivot point is middle value -- for guaranteed `O(n lg n)` for sorted data.
    - Time complexity
      * Best / Average: `O(n * log n)`
      * Worst: `O(n^2)`
    - Auxiliary space complexity
      * Naive: `O(n)`
      * In-place: `O(log n)`


---


📦 [Data Structures](https://en.wikipedia.org/wiki/Data_structure)
--------------------

### [Arrays](https://en.wikipedia.org/wiki/Array_(data_structure))

* An array is a contiguous sequence of the same type.
* A memory buffer is (pre)allocated for all elements.
* Random access of any element (via index).
* Lookup by index: `O(1)` time
* Lookup by value: `O(n)` time
* [__Dynamic Array__](https://en.wikipedia.org/wiki/Dynamic_array)
  - Occasionally resized (copies elements; typically faster than dynamic allocations required by linked list).
  - Typical "array" type for scripting languages (typically with static array(s) utilized internally).
  - Insertion / Deletion: `Amortized O(1)` | `O(n)` time
* [__Static Array__](https://en.wikipedia.org/wiki/Array_(data_structure))
  - Cannot be resized at runtime; must re-allocate buffer & copy.
* [__String__](https://en.wikipedia.org/wiki/String_(computer_science))
  - Typically a read-only array of characters.
* [__Variable-Length Array__](https://en.wikipedia.org/wiki/Variable-length_array)
  - Length determined at runtime.
  - Not growable; generally preferable to use a dynamic array instead because it's growable.


### [Linked List](https://en.wikipedia.org/wiki/Linked_list)

* Each element dynamically allocated (typically slower than occasional copies required by dynamic array).
* Complexities:
  - Lookup: `O(n)` time
  - Insertion / Deletion: `O(1)` time


---


🎨 Design
---------

* Design code before writing:
  - To have a plan & avoid getting stuck.
  - To collaborate on approach for solution.
  - Because jumping straight into coding, on large projects, is a bad idea.


---


🗺️ Other Resources
------------------

* [Example Sorting Implementations](https://neetcode.io/solutions/sort-an-array) - Neetcode
* [Algorithms](https://www.khanacademy.org/computing/computer-science/algorithms) - Kahn Academy (Cormen/Balkcom)
* [VisuAlgo](https://visualgo.net/en) - visualising data structures and algorithms through animation


### 📚 Books

<details><summary>IEEE/ACM Undergraduate CS Course Recommendations</summary>

- [History of Curricular Guidelines](https://cs.union.edu/~hemmendd/History/curric-hist.pdf)
- [Computer Science Curricula 2023](https://ieeecs-media.computer.org/media/education/reports/CS2023.pdf)
</details>
<details><summary><a href="https://mitpress.mit.edu/algorithms">Introduction to Algorithms</a></summary>

- _Third Edition_
  - [CLRS Solutions](https://walkccc.me/CLRS/) - walkccc
</details>
<details><summary><a href="https://web.archive.org/web/20200218054807/http://www.piexposed.com/">Programming Interviews Exposed</a></summary></details>
<details><summary><a href="https://www.crackingthecodinginterview.com/">Cracking the Coding Interview</a></summary>

- [Solutions](https://github.com/careercup/CtCI-6th-Edition) - 6th edition
- [Solutions](https://github.com/careercup/ctci) - 5th edition
- [Behavioral](https://www.crackingthecodinginterview.com/uploads/6/5/2/8/6528028/cracking_the_soft_skills_-_v6.pdf) - prep sheet
- [Coding](https://www.crackingthecodinginterview.com/uploads/6/5/2/8/6528028/cracking_the_coding_skills_-_v6.pdf) - flow chart
- [PM](https://www.crackingthecodinginterview.com/uploads/6/5/2/8/6528028/cracking_the_pm_skills_-_v6.pdf) - interview questions
</details>
<details><summary><a href="https://bctci.co">Beyond Cracking the Coding Interview</a></summary>
  
- [Boosters](https://drive.google.com/file/d/16C9gz9waj0A9XmVlaOgbDgEQZkATuRNY/preview)
- [Question Landscape](https://drive.google.com/file/d/1Bu4cHzbY0uZg2TcPjdvy_hhNF7_HOlZJ/preview)
- [Catalog of DSA Topics](https://bctci.co/topics-image)
- [Interview Checklist](https://drive.google.com/file/d/1Q9Uc-1UdvyaqbkTGSaZ3-aVEYX5ImZMl/preview)
- [Post Mortem Exmple Log](https://drive.google.com/file/d/1LG-aUqjEbTVddkjeuCHMtROlm9BMIhDb/preview)
- [Post-Mortem](https://docs.google.com/spreadsheets/d/1phKTGfnQtuElTQ4BQSBfa1H5QO1-Ip9j8NRVZkR_FTk)
- [\[Python\] Interview Cheat Sheet](https://docs.google.com/document/d/1LtXh1oew6pZ9D4s5mw_33jzA2UwBfnv9jWh1bkSRTCc)
- [Nine Free Chapters](https://drive.google.com/drive/folders/1AdUu4jh6DGwmCxfgnDQEMWWyo6_whPHJ)
- [Set & Map Implementations](https://docs.google.com/document/d/e/2PACX-1vRWfoJWWNp49cIZxDCZPkvQ2o8WOImKWLkimF7lhnsY-CmT1kREPP0duEKmnXyf-rPG1B0QGsxmcITy/pub)
- [Monotonic Stacks & Queues](https://docs.google.com/document/d/e/2PACX-1vT29T3Tfvdkd-IGI2HCIgtAbWwYZ76pHCSlTkuyHiCvRqU5BD6S6_MJWcZl0Rgw1C2uhMykFFkNLHDu/pub)
- [Union-Find](https://docs.google.com/document/d/e/2PACX-1vRwYsi-g1CKIDpbfhB5Xm9Lp1-OL1ooVI5i3kR4yFMX2ME14ODGZva9dabMM8Pe-Tduj4on8V8TGviZ/pub)
- [All problems, solutions & test cases](https://bctci.co/all-problems)
</details>


### <img src="https://user-images.githubusercontent.com/7102064/160022421-ed9425eb-6a6b-4849-a090-5a27542b60c3.png" width="24px" /> Videos

- [Algorithms 1](https://youtube.com/playlist?list=PLXFMmlk03Dt7Q0xr1PIAriY5623cKiH7V) - Stanford
- [Algorithms 2](https://youtube.com/playlist?list=PLXFMmlk03Dt5EMI2s2WQBsLsZl7A5HEK6) - Stanford

* BINARY TREES
  - [Binary tree traversal - breadth-first and depth-first strategies](https://youtu.be/9RHO6jU--GU) - mycodeschool
* HASH TABLES
  - [Design Hashmap](https://youtu.be/cNWsgbKwwoU) - Neetcode
  - [Intro to Hash Tables and Dictionaries](https://youtu.be/sfWyugl4JWA) - CS Dojo
* HEAPS
  - [Heaps in 3 minutes — Intro](https://youtu.be/0wPlzMU-k00) - Michael Sambol
* LOGARITHMS
  - [Logarithms... How?](https://youtu.be/Zw5t6BTQYRU) - NancyPi
    - <code>log<sub>2</sub>(n) => 2<sup>x</sup> = n</code>
  - [Log base2 using calculator](https://youtu.be/dG2x5nM50ps)
    - <code>log<sub>2</sub>(n) = ln(n) / ln(2)</code>
* QUICKSORT
  - [Complete Quicksort Overview](https://youtu.be/0SkOjNaO1XY) - CS Dojo
  - [Quicksort algorithm](https://youtu.be/COk73cpQbFQ) - mycodeschool
