1.STATIC METHOD:
    i) Same class :
     methodName();
     
    ii) Diff. Class :
     OriginalClassname var = OrginalClassName.methodName();

2.STATIC + RETURN METHOD:
     methodname(arg.value);
  
 
3.NON-STATIC METHOD & RETURN METHOD:
     i)Normal:
        Classname obj = new Classname();
        obj.methodname();
      ii) Return:
        obj.methodname(arg.value);

3.VARIABLE:
  i) Instance variable:
     Classname obj = new Classname();
     obj.InstanceVar();
 ii) Static variable:
     classname.instancevar();         //no need to create object

4.CONSTRUCTOR METHOD:
     Classname obj = new Classname();

