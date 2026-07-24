1. Classname obj = new Classname ();
2. Scanner sc = new Scanner (System.in);
3. CONSTRUCTOR:
     AccessModifier Classname () { }
     Eg. public Classname () { }

4. ARRAY:
    i)Datatype var [] = new Datatype [size];
   ii)Datatype [] var = {v,a,l,u,e,s};

5. LIST:
     `List<DataType> listName = new ArrayList<>();` 
	    List variable = new ArrayList();
	    List variable = new LinkedList();
	    List variable = new VectorList();

      
6. SET:
    Set variable = new HashSet();
    `Set<Integer> variable = new HashSet<>();`

7. MAP:
    Map<key,value> variable = new HashMap<key,value>()

8. ROBOT CLASS:
	Robot var = new Robot();

9. ACTIONS:
	Actions a = new Actions(driver);

10. DROPDOWN:
	Select s = new Select (var);

11. IMPLICIT WAITS:
	driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);

12. EXPLICIT WAITS:
	 i) WEBDRIVER WAIT :
		 WebDriverWait wait = new WebDriverWait(driver, 60);
	    wait.until(ExpectedConditions.visibilityOf(text));

	 ii) FLUENT WAITS = Wait fwait = new FluentWait(driver).
		withTimeout(Duration.ofSeconds(30))
		.pollingEvery(Duration.ofSeconds(5))
		.ignoring(NoSuchElementException.class);

		 fwait.until(ExpectedConditions.elementToBeClickable(userName));

13. FILE :  ("refer Pack: exceptionHandling-->FileHandling ")
	 File var =  new File (path:\\filename.type)
	 boolean B1 = var.mkdir();    //For creating a single folder:--->path name end with folder name
	 boolean B2 = var.mkdirs();  //For creating multiple folder: -->end with folder inside folder.... names
	 boolean B3 = var.createNewFile(); //For creating files:-->for this path name should end with file format(.pdf etc)

14. JAVASCRIPT EXECUTOR:
	  `JavascriptExecutor js = (JavascriptExecutor)driver;`

15. DROP DOWN:
	`Select s = new Select(var);`

16. Broken link:
	 HttpURLConnection var =  (HttpURLConnection) (new URL(link var name).openConnection());








