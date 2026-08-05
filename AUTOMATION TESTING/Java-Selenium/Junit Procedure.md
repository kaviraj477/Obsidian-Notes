JUNIT:
1. New project --> maven project -->  create a simple.... --> next 
2. group ID --> group id and artifact id -- Junit 
3. open pom.xml --> type <dependency> & </dependency>
4. mvnrepository website --> junit --> 2nd code --> copy paste inbetween <dependency> and </dependency> --> remove scope test line
5. add other dependencies from other pom.xml such as 
   i) selenium
   ii) webdriver manager
6. enter various method and their actions
7. add @Test before methods 
      @Ignore -- it ignores the method/test mentioned below it

8. Assertion -  1.Hard assert 
             2. soft assert

9. hard assert- import from Junit--> Assert.assertTrue(condition)
     i) `condition = elementName.isDisplayed (or) isEmpty etc....
*             if the condition is true, the following code will run in the method if not it won't run
       ii) `Assert.assertTrue(false); --> it manually fails the following codes
      iii) `Assert.assertEquals(_, _) -->(Expected value, Actual Value)

10. create another class with Junit methods
     we can run both these class using 
     `@RunWith(Suite.class)
     `@SuiteClasses ({JunitDemo.class, JunitLogin.class})
     `public class TestRunnerDemo { }
 








