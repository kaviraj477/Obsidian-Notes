+ If we know that a method is going to fail and may throw stale element exception we use "*RetryAnalyzer
+ But if we don't know where the test is going to fail, we use "*IAnnotation transformer" 

1.  Create a class (eg.classname1)
2.  *implements* `IAnnotationTransformer`
3.  hover -->`add unimplemented methods`
4. after implementing we get :
     `public void transform(ITestAnnotation annotation, Class testClass, Constructor testConstructor, Method testMethod)`
	  + `annotation, testClass, testConstructor, testMethod` --> user defined variable `annotation.setRetryAnalyzer(Classname2.class)
	  + Classname2 --> we call the classname where script for retryAnalyzer is written 
5. `String s1 = testmethod.getname();`
   `System.out.println(s1);`
	   + `testmethod` --> Method variable (mentioned in method arguments)
	

**OPEN .XML FILE**
1. Below <suite> type : 
			 `<listeners>`
			`<listener class-name = "packagename.classname1"/>`
			`</listeners>`
  2.  Feature file --> run as TestNGsuite

FAILED CASES REPORT

	1. Open test-ouput (folder) --> testing-failed.xml (file)



