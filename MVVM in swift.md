
**MVVM (Model View View Model) (Core steps)**

* Bind viewModel outputs to the views.
    * Mechanism for binding views to output values 
        * Key value observing - mechanism for using key paths to observe a property and get notifications when that property changes.
        * Functional Reactive Programming - A paradigm for processing events and data as streams. Apples Combine Framework is its approach to FRP.
        * Delegation - Using delegate methods to pass notifications when values changes.
        * Boxing - Using property observers to notify observers that a value has changed.
        
* ViewModel should only permit the UIKit.UIImage type, no other UIKit type should be permitted inside the ViewModel.
  A general rule of thumb is to never import UIKit in your view models.
* In MVVM, the view controller is only responsible for views. The view model is always responsible for formatting data from service and model types to present in the views.
* One of MVVM’s big advantages is how much easier it makes creating automated tests.
* Benifits of refactoring MVC to MVVM :-
   * ViewController will become much simpler.
   * ViewController no longer depends on model types and only focussed on view.
   * ViewController only interacts with viewModel by sending inputs and binding to its        outputs.
   * ViewModel Separates the business logic from the low level view logic.
   * It’s simple to add a new feature with minimal modification to the ViewController.
   * Testable: The ViewModel is relatively easy to test.
   
However, there are some trade-offs to MVVM that you should consider:

* Extra type: MVVM introduces an extra view model type to the structure of the app.
* Binding mechanism: It requires some means of data binding, in this case the Box type.
* Boilerplate: You need some extra boilerplate to implement MVVM.
* Memory: You must be conscious of memory management and memory retain cycles when introducing the view model into the mix.
