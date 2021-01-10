
**MVVM (Model View View Model) (Core procedure and steps)**

* Bind viewModel outputs to the views.
    * Mechanism for binding views to output values 
        * Key value observing - mechanism for using key paths to observe a property and get notifications when that property changes.
        * Functional Reactive Programming - A paradigm for processing events and data as streams. Apples Combine Framework is its approach to FRP.
        * Delegation - Using delegate methods to pass notifications when values changes.
        * Boxing - Using property observers to notify observers that a value has changed.
        
* ViewModel should only permit the UIKit.UIImage type, no other UIKit type should be permitted inside the ViewModel.
  A general rule of thumb is to never import UIKit in your view models.
*
