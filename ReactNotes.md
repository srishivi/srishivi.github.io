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
