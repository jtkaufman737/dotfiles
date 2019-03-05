# idea one: 
 
## topology as FK with...whatever we want to call it...documentation model? ie 

```json
{ 
   name: ...
   organization...
   documentation: [
     { 
        id: ... ,
        title: ... ,
        body: ...
     }
   ],
   nodes: [
    ...
   ],
   ....
}
```
- documentation as foreign key
- disadvantages: If we ever envisioned having multiple types of documentation per topology, I could see an object of objects 
being more useful 

# idea two 

## close variation of one, easier to deal with if we ever envisioned having multiple documentation models for some reason...

```json 
{  
  ... // all else the same as prior example
  documentation: { 
    identifierOne: { ...}
    identifierTwo: { ...}
  }
  ...
}
```

