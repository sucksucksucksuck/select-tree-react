# 基于react封装的 树形结构单选框
![image](https://github.com/sucksucksucksuck/select-tree-react/blob/master/chain.png)

## 使用范例：
* 首先把该组件引入到项目
```javascript
<SelectTree defaultValue={this.state.search.group_id} admin_group={this.state.admin_group} defaultTitle="全部角色"/>
```
#### defaultValue
默认值 => 可以为一个变量

#### admin_group 
数据格式:
```javascript
const admin_group = [{
        "id":2,
        "pid":1,
        "title":"林宅",
        "son":[
            {"id":3,
            "pid":2,
            "title":
            "林大爷",
            "son":[
                {"id":4,
                "pid":3,
                "title":"林爸爸",
                "son":[
                    {"id":9,
                    "pid":4,
                    "title":"儿子",
                    "son":[]
                    },
                    {"id":10,
                    "pid":4,
                    "title":"女儿",
                    "son":[]
                    }]
                }
            ]
        }
    ]
}]
```
#### defaultTitle
单选框第一个选项