[[TestNG]]
1. Add @Test before methods (this executes the code based on ASCII Codes randomn order only)
2. Run as TestNG Test

I. Syntax:
    + `@Test (priority = n) `  n = ...-3,-2,-1,0,1,2,3,...
    + `@Test (enabled = false)`  this ignores the following method
    + `@Test (invocationCount = n)` for executing a method multiple times 
    + `@Test (dependsOnMethod = methodName)` this method ensures the following method proceeds only the given method is executed 
    +  `@BeforeMethod` prioritises the following method before other methods
    +  `@AfterMethod` performs the following method after completion of other methods

II.Assertion => TestNG - both soft and hard assert

SoftAssertion --> does'nt stops execution unlie hard assert, but we can only check failure in console/ log report
    + `public static SoftAssert var;`  (Creating an object)
    + `var.assertTrue(True/false);
    + `var.assertTrue(True/false, "varstatement')`  --> this method displays the statement in console
    + `var.assertAll ();` --> this method is must to execute assertion, it can be added in any method

II. TestNG report
   Project > right click > refresh > New folder created automatically > index.html > open with System Editor (We can't share this report unlike BDD)

III. To run multiple classes
 1. After creating multiple classes > project right click > TestNG > Convert to TestNG > Finish
 2. .xml file created > right click > run as TestNG Suite

IV. .xml file methods (Hierarchical order)
 + `@BeforeSuite` --> execute before starting of the suite
 + `@BeforeTest` --> executes after suite but before test
 + `@Beforeclass`
 + `@BeforeMethod`
 + `Test`
 + `@AfterMethod`
 + `@AfterClass`
 + `@AfterTest` 
 + `@AfterSuite` --> executes after the suite

V. PARAMETERS
 *parameters can be passed inside class. It can be passed inside .xml file*
 *can be written multiple times in an .xml file*

*Syntax inside .xml*
 + `<parameter> name = " 1 " value = " 2 " >`  --> can add no.of name and values
 + `</parameter>`

*Syntax inside Class (before method and @Test)* 
+ `@Parameters ({"1", "2"})` ---> can add any no.of parameters based on .xml name and value
+ `@Test(.........) `
+ `public void method (@Optional ("3") datatype 3, @Optional ("4") datatype 4 ){`
+ `WebElemnt var = driver.find.......`

VI. DATA PROVIDERS

+ `@DataProvider (name = "1" )   
+ `public object [ ] [ ] objName ( ) {  `
+ `return new Object [ ] [ ] {{"2"}}`  2--> goes to 1
+ 
+ `@Test (dataProvider = "1")`    1-->3
+ `public void methodName (Datatype "3")`
+ `element.sendkeys (3)`

VII. MULTIPLE VALUES

  + `@DataProvider (name = "1")`
  + `public object [] [] methodName () {`
  + `return new Object [] [] {{ "2", "3", }};  2,3--> goes to 1
  + 
  + `@Test (dataProvider = "1")`
  + `public void methodName2 (Datatype 4 , Datatype 5){`
  + `element.sendKeys(4 (or) 5);`--> only one we can use

VII. MULTIPLE VALUES 2

+ `@DataProvider (name = "1")`
+ `public object [] [] methodname () {
+ `return new Object [] [] {{ "2","3"}{"4","5"}}; -->can add any no.of values
+ 
+ `@Test (dataProvider = "1")`
+ `public void methodName2 (Datatype 6 , Datatype 7){`
+ `element.sendKeys(6 (or) 7);`--> only one we can use
+ 
   


