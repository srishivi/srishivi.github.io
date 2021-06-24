https://www.youtube.com/watch?v=DLX62G4lc44&t=17274s

<h1> React JS </h1>

1. Node module package contains all the dependencies to be used in react project like react and react Dom.
2. React Dom helps to render the elements. 
3. ReactDom.render(What to render , Where to render)
   `ReactDOM.render(<h1>Hello World</h1> , document.getElementById('root'))`
4. function name should be in pascal case e.g., FunctionName
5. Any JavaScript which needs to be interpreted in the middle of an element should be wrapped in curly brace.
6. Inline styles are given to jsx elements in the json format. e.g., <h1 style = {{color : "" , backgroundColor :""}}>
   - Everytime we are in js world, we have to follow js conventions. For e.g, backgroundColor in above line.
   - Jsx element expects style to be a js object rather than string hence 1st curly brace, and another because we are switching to js world. 
7. Properties can be passed when we need topass data between one to another component.
   - <NewComponent name ="abc" e-mail ="def@abc.com" />
   - Same data can be extracted as function NewComponent(props){}. Here props is a json. so name can be extracted as props.name which will give the value abc.
   - we can also pass a json object as property . <NewComponent contact = {{name:"abc" email:"def@bc"}}/> which can be extracted as props.contact.name. 
8. We can also apply conditions when applying styles.
   - <h3 style ={{display: !props.question && "none"}} Question : {props.question} </h3>
   - if the props.question is not available then value will not be printed.
9. Refer functional programming in js to know about map, filter, reduce etc methods. These functions operate on an array.
    - `    const productData = ProductData.map(ProductData => <Product key={ProductData.id} product={ProductData}/>) ` 
10. Components can be functional components or class based components.
    - Functional component
      func(){
      return (
         <div> 
         </div>
      ) 
      }
    - Class Component
       class App extends React.component {
         render() {
         return {
             } 
         }
        }
11. <b> State : </b> State is a data that a component maintains. Props can not be changed by the component which is receiving the props whereas the state can be changed. 
   - State can be maintained only by the class component. States are mutable wheras props are not.
   - The initialization of the states are done in constructor of the class (which is extending React.Component).
   - Props are the only way to pass data between compoents.
   - When we change the date through setState method, all the components accessing that state gets updated automatically. 
   - this.state = {isLoggedIn = "false" , todoList = ""} . In this way values are assigned to state property.
12. Function call on the click of button can be done as <button onClick = {this.callTheMethod} >Click me </button>.
13. setState method can be called in two ways. One way is to this.setState({count : 1}) . New version of state is passed as json in the parameter.
    Another way is to create an inline method inside setState. this.setState(prevState = > { return count : prevState.count+1 })
15. Whichever method calls setState method should be bound with the context of the class in the constructor. eg., this.handleClick = this.handleClick.bind(this).

