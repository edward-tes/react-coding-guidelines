# React Coding Guidelines

## 编码原则:
 1. 文件命名应该尽量简洁，但需要表达出组件功能
 1. 应该尽量减少嵌套
 1. 减少歧义，减少开发沟通成本
## 命名风格
1. 【强制】文件名统一使用小写，多个单词，使用短横线分隔, 不能以下划线或驼峰命名
 
    > 正例: card | card-item 

    > 反例: cardItem 

1. 【强制】类名首字母大写，大驼峰命名

    > 正例: card/index.js => class Card
    
    > 反例: card/index.js => class SmallCard
    
1. 【强制】样式类名必须小写，并且使用短横线分隔

    > 正例: .card-item{} | .people-name{}
    
    > 反例: .cardItem{} 

1. 【推荐】类名应尽量使用以文件名称相对应的大驼峰命名
 
1. 【推荐】每个React组件，都应该使用一个以组件命名的文件夹包裹，组件入口为index.js, styles.scss 或者 styles.less, styels为统一使用复数形式，子组件也应该参考同样的规则。

    > 正例: card/index.js | card-item/styles.scss
    
    > 反例: card-item/card-item.js | card/card.scss | card/style.scss
    
1. 【推荐】样式表应尽量减少类之间的嵌套

    > 正例： .container{} .container-card{} 
    
    > 反例： .container{.card{}}

1. 【推荐】React组件中如果组件是`pure component`，那应该继承React.PureComponent

1. 【推荐】变量定义优先使用`const`

1. 【推荐】组件尽量保证share，所以共享的组件不需要再单独创建一个share文件夹放置
 
1. 【推荐】组件导入时应尽量使用绝对路径
 
    > 正例: import Card from "components/card"

    > 反例: import Card from "../card"
