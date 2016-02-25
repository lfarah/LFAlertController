# LFAlertAction
UIAlertAction extension with handler inside initialization

#### Initialization

##### Create Actions
``` swift
//Creating Actions
let action0 = UIAlertAction(title: "First Action", style: .Default, handler: nil)
let action1 = UIAlertAction(title: "Second Action", style: .Default, handler: nil)
```

##### Initialize UIAlertController
``` swift
//Creating UIAlertController with handler
self.controller = UIAlertController(title: "hey", message: "ho", preferredStyle: .Alert,actions:[action0,action1]) 
{ (action,index) -> () in
      
  //Printing index of Action
  print("\(index) - \(action.title!)")
}
```

##### Show UIAlertController
``` swift
self.controller.show()
```

