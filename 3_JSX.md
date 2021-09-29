# JSX

- JavaScript XML(JSX) - Extension to the Javascript language Syntax.
- Write XML- like code for elements and components
- JSX tags have a tag name, attributes, and Children.

#### why jsx
 
 - JSX is not a necessity to write React applications.
 - JSX makes your react code simpler and elegant.
 - JSX ultimately transpiles to pure JavaScript which is understood by the browsers.

 ```js
 import React from 'react'

 //Normal JSX

 export const Hello = () => {
     return (
         <div>
         <h1>Hello Prasad</h1>
         </div>
     )
 }


 //With pure Js

export const Hi = () => {
 return React.createElement(
     'div',
     {id:"Hello", className: "dummy"},  //In JS class is reserved keyword so we use className for css Classes
     React.createElement('h1',null,'Hello Prasad')
 )
}

 ```
 `NOTE: Always use JSX instead of pure Javascript because you might have 100 of component which can get difficult to manage`

 ### JSX differences

 - Class -> replaced by className
 - for -> replaced by HTMLFor

 camelCase property naming Convention
  - onclick -> onClick
  - tabindex -> tabIndex

  