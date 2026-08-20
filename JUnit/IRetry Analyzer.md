1. Create a class
2. *implements* `IRetryAnalyzer`
3. hover and select -- *add unimplemented methods
4. If the return type is true, it performs the retry function again and again. So we must set condition to stop the retry at certain limit.
5. If the return type is false, the retry function won't execute.
6. Open implemnent class: 
     `@Test (retryAnalyzer = classname.class)`
     - we add this syntax above the method we know that would fail anyway
7. Open feature file --> run as TestNGsuite
