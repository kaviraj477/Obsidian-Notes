[[Selenium]]
1. Classname obj = new Classname ();
2. Scanner sc = new Scanner (System.in);
3. CONSTRUCTOR:
     AccessModifier Classname () { }
     Eg. public Classname () { }

4. ARRAY:
    `i)Datatype var [] = new Datatype [size];  --> *DYNAMIC ARRAY*
   `ii)Datatype [] var = {v,a,l,u,e,s}; --> *STATIC ARRAY*

5.  STRING:
     **i) Concat:**  *it wont't overwrite, rather it joins in a new varaible*
         `String var1 = "tiger";
         `` String s1 = var1.concat("muthuvel Pandian");
         
     **ii) Append: *it overwrites the value*
         `StringBuffer var2 = new StringBuffer ("tiger");`
         `var2.append("ferocious");`

`

6. LIST:
     `List<DataType> listName = new ArrayList<>();` {{Datatype-- wrapper class}}
	    List variable = new ArrayList();
	    List variable = new LinkedList();
	    List variable = new VectorList();

      
7. SET:
    Set variable = new HashSet();
    `Set<Integer> variable = new HashSet<>();`

8. MAP:
    Map<key,value> variable = new HashMap<key,value>()

9. ROBOT CLASS:
	Robot var = new Robot();

10. ACTIONS:
	Actions a = new Actions(driver);

11. DROPDOWN:
	Select s = new Select (var);

12. IMPLICIT WAITS:
	driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);

13. EXPLICIT WAITS:
	 i) WEBDRIVER WAIT :
		 WebDriverWait wait = new WebDriverWait(driver, 60);
	    wait.until(ExpectedConditions.visibilityOf(text));

	 ii) FLUENT WAITS = Wait fwait = new FluentWait(driver).
		withTimeout(Duration.ofSeconds(30))
		.pollingEvery(Duration.ofSeconds(5))
		.ignoring(NoSuchElementException.class);

		 fwait.until(ExpectedConditions.elementToBeClickable(userName));

14. FILE :  ("refer Pack: exceptionHandling-->FileHandling ")
	 File var =  new File (path:\\filename.type)
	 boolean B1 = var.mkdir();    //For creating a single folder:--->path name end with folder name
	 boolean B2 = var.mkdirs();  //For creating multiple folder: -->end with folder inside folder.... names
	 boolean B3 = var.createNewFile(); //For creating files:-->for this path name should end with file format(.pdf etc)

15. JAVASCRIPT EXECUTOR:
	  `JavascriptExecutor js = (JavascriptExecutor)driver;`

16. DROP DOWN:
	`Select s = new Select(var);`

17. Broken link:
	 HttpURLConnection var =  (HttpURLConnection) (new URL(link var name).openConnection());

18. Junit Testing:
     `@RunWith(Suite.class)
     `@SuiteClasses ({Class1name.class, class2name.class}) 

     + ***Keywords:***   `@BeforeClass, @Test, @AfterClass
19. POM:
   + *create an argument based constructor , whose values are passed from another class and then initialize it.
   
	   + `public classname1 (WebElement drivername){
	     `pagefactory.initElements(drivername, this);
	       }`
	+ `` classname1 obj = new classname1(drivername1); >> this argument is pased to POM lass
	     `drivername1 = new ChromeDriver(); >> argument value is asignes here
	     
	 + *P.S: drivername and drivername1 can be same or different*









