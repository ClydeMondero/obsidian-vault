[[Redux]]

# Data Flow  in Redux
#resource 

## State 
a value in the application that can be change.
## Store
a container that hold's the global state of the application's data, runs the reducer when an action is dispatched and tells the subscriber if the state is updated.
## Action 
a event that describes what happened in the application and causes the state to update.
## Dispatch
tells the store what type of action has happened .
## Reducer
calculates the new state based on the old state and the action.
## Subscriber
an object waits for a state to be updated so that the UI can be updated with the new data.
	
![[Pasted image 20231219212005.png]]

[Reference](https://redux.js.org/tutorials/fundamentals/part-2-concepts-data-flow) 