# React JS Notes

## Fragments

- Allows grouping of multiple elements without extra DOM nodes.  
- Return multiple elements without a wrapping parent.
 
- **`Syntax`**  
  (i)  <React.Fragment> ..... </React.Fragment>  
  (ii)  <> ..... </>

> App.jsx
  ``` jsx
import React from "react";

function App() {
	return (
		<>
			<h3>Hello this is Abhishek Yadav.</h3>
		</>
	);
}

export default App;
```

## Map Method

-  Render lists from array data.
-  Transform array items into JSX.
-  **`Key Prop`** : Assign unique key for optimized re-renders. `( <div key={item.id}>{item.name}</div> )`


> App.jsx
``` jsx
import "bootstrap/dist/css/bootstrap.min.css";

function App() {
	let footItems = ["Dal", "Green Vegetables", "Roti", "Salad", "Milk", "Ghree"];

	return (
		<>
			<h1>Healthy Foods Items</h1>

			<ul className="list-group">
				{footItems.map((items) => (
					<li key={items} className="list-group-item"> {items} </li>
				))}
			</ul>
		</>
	);
}

export default App;
```























