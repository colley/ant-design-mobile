---
order: 2
title: 底部选项卡
---

tabPosition: bottom

````jsx
import { Tabs, WhiteSpace } from 'antd-mobile';
const TabPane = Tabs.TabPane;

function callback(key) {
  console.log(key);
}

let TabExample = React.createClass({
  render() {
    return (
      <div>
        <Tabs defaultActiveKey="1" tabPosition="bottom" onChange={callback}>
          <TabPane tab="选项卡一" key="1">
            <div style={{
              display: 'flex', alignItems: 'center', justifyContent: 'center', height: 100,
            }}>
               选项卡一内容
            </div>
          </TabPane>
          <TabPane tab="选项卡二" key="2">
            <div style={{
              display: 'flex', alignItems: 'center', justifyContent: 'center', height: 100,
            }}>
               选项卡二内容
            </div>
          </TabPane>
          <TabPane tab="选项卡三" key="3">
            <div style={{
              display: 'flex', alignItems: 'center', justifyContent: 'center', height: 100,
            }}>
               选项卡三内容
            </div>
          </TabPane>
        </Tabs>
        <WhiteSpace />
      </div>
    );
  },
});

ReactDOM.render(<TabExample />, mountNode);
````
