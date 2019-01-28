# React-norm
如果您有不同建议可更改及备注用意哈。


react 类组件模板,有状态组件(一个文件一个有状态组件)
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
  componentDidMount(){} // 组件创建完成后调用
  componentWillReceiveProps(){nextProps,nextState} // 组件的 props 或 state 有更新时调用
  shouldComponentUpdate(nextProps,nextState){return true} // 组件将要更新，可在此函数判断是否重新渲染
  componentWillUnmount(){} // 组件卸载时调用，解绑一些函数或其他
  render(){
    return (
     <div></div>
    ) 
  }
}
ComponentName.PropTypes={};// props 传值类型检测
ComponnetName.defaultProps={};// 当检测类型不是必需时，可写默认 props 
export default Component;
```
react 变量组件模板,无状态组件(可在一个文件上写多个无状态组件)
```jsx
import React from 'react;
const ComponentName = ({...props}) => {
  return (
    <div></div>
  );
}
export { ComponentName };
```
