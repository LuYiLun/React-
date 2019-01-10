# React-
如果您有不同建议可更改及备注用意哈。


react 类组件模板
```jsx
import React, { Component } from 'react';

import { Tabs } from 'antd';
const TabPane = Tabs.TabPane;// const 声明的组件放在 import 下面

class ComponentName extends React.Component {
  constructor(props){
    super(props);
    this.state = {
    };
  }
  render(){
    return (
     <div></div>
    ) 
  }
}
```
