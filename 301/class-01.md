## Introduction to React and Components

![React](https://miro.medium.com/max/1400/1*CeuWv9fCjD1uTiTuKytnBQ.png)

### What is a Component?
- A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

### What are the charactistics of a component?

1-**Reusability** − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

2-**Replaceable** − Components may be freely substituted with other similar components.

3-**Not context specific** − Components are designed to operate in different environments and contexts.

4-**Extensible** − A component can be extended from existing components to provide new behavior.

5-**Encapsulated** − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

6-**Independent** − Components are designed to have minimal dependencies on other components.

### What are the advantages of using component based architecture?

1-**Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

2-**Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.

3-**Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

4-**Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

5-**Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.

6-**Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

7-**System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.

8-**Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

![Component](https://www.freecodecamp.org/news/content/images/2020/03/React-components.png)


### What is props short for?
- “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

### How are props used in React?
- **Firstly**, define an attribute and its value(data)
- Then pass it to child component(s) by using Props
- **Finally**, render the Props Data

#### Examle 
     function Welcome(props) {
        return <h1>Hello, {props.name}</h1>;
     }
----
    class Welcome extends React.Component {
        render() {
        return <h1>Hello, {this.props.name}</h1>;
     }
    }
---

### What is the flow of props?
- data with props are being passed in a uni-directional flow. (one way from **parent** to **child**)

![properties](https://dmitripavlutin.com/static/6d14625626a323816b47d301a6319626/05127/cover.png)