1. NESTED CLASS "non-static method":  --> type inside nested class
   `nestedclass obj1  = new nestedclass();
   `parentclass obj2 = obj1.new parentclass();
   `obj2.methodname();` 
                 (OR)
    `parentclass obj = new Nestedclass().new parentclass();
    `obj.methodname();

2. NESTED CLASS "static method":
   `parentclass.methodname();` --> type inside nested class