DSA Coding Interview
====================

_Think out loud the entire time -- even when stuck!_


1. __*PROBLEM CLARIFICATION*__
   * Read the question out loud, then restate it in your own words
   * Rapidly offer up concise examples _(as little as possible; as much as necessary)_:
     - Expected cases
     - Edge cases
     - Error cases / expect valid data ?
   * Discover all constraints & make concise note of them:
     - Input(s) & Output(s):
       - Minimums & Maximums (structure size, element size, negative values, empty)
       - Pre/sorted ? (ascending or descending?)
       - Duplicates ?
       - Types (null, unicode, floating-point, etc)
       - Format (mutable array, immutable string, map, linked list, tree)
2. __*HIGH-LEVEL APPROACH*__
   * Avoid any form of pseudocode
   * Propose high-level solution(s):
     - Determine naive / brute force time & space complexity
     - Work toward an optimal solution (would interviewer prefer better space efficiency or better time?)
     - State time & space complexities
   * Diagram an optimal approach:
     - Step through a small but sufficient example
     - Document essential high-level / abstract steps with (indented) bullet-points:
       - Can act as comments above code blocks
       - Can assist in naming helper functions
   * Get buy-in from interviewer
4. __*CODING IMPLEMENTATION*__
   * Ask permission before writing _any_ code
   * Get agreement on primary interface (parameter order)
   * Implement the agreed upon solution:
     - Import / include all external dependencies
     - Write clean code:
       - Comment above code blocks, especially for later reviewers
       - Meaningful naming (not too short, not too long)
       - Consistent indention / whitespace
       - Create appropriate helper functions:
         - Break down into smaller sub-problems
         - Derive names from high-level bullet points
         - Keeps code DRY
   * Mention line numbers when jumping around
   * Stuck?
     - Revisit high-level (drawing board) solution
     - Refactor for readability:
       - Improve naming
       - Consider helper methods
     - Comment above blocks or any difficult to comprehend code
     - Do a quick dry run (with a very small example)
   * Test code:
     - Don't say "done" until absolutely sure code is error free & runs properly
     - Fix bugs on the fly
     - Dry run _at least_ one example:
       - Test actual implementation, line by line
       - Track state in comments
     - Consider expected, edge & error cases:
       - Mention what else you'd test for, even if you can't do it now
