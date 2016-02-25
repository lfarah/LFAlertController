# LFAlertController
UIAlertController Swift extension with handler inside initialization :large_orange_diamond:

## How to install

#### Using the Swift file:
Drag the **LFAlertController.swift** from */Sources* to your project

#### Using CocoaPods:
Not available yet!

## How to Use

##### Create Actions
``` swift
let action0 = UIAlertAction(title: "First Action", style: .Default, handler: nil)
let action1 = UIAlertAction(title: "Second Action", style: .Default, handler: nil)
```

##### Initialize UIAlertController with Handler
``` swift
self.controller = UIAlertController(title: "hey", message: "ho", preferredStyle: .Alert,actions:[action0,action1]) 
{ (action,index) -> () in
      
  //Printing index of Action
  print("\(index) - \(action.title!)")
}
```

##### Initialize UIAlertController without Handler
``` swift
self.controller = UIAlertController(title: "hey", message: "ho", preferredStyle: .Default, actions: [action0,action1])
```

##### Show UIAlertController
``` swift
self.controller.show()
```

