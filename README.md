# React Coding Guidelines

## 编码原则:
 1. 文件命名应该尽量简洁，但需要表达出组件功能
 2. 应该尽量减少嵌套
 3. 减少歧义，减少开发沟通成本
## 命名风格
* 【强制】文件名统一使用小写，多个单词，使用短横线分隔, 不能以下划线或驼峰命名
    正例: card | card-item 
    反例: cardItem

* 【强制】类名首字母大写，大驼峰命名
    正例: card/index.js => class Card
    反例: card/index.js => class SmallCard

* 【强制】样式类名必须小写，并且使用短横线分隔
    正例: .card-item{} | .people-name{}
    反例: .cardItem{} 

* 【推荐】类名应尽量使用以文件名称相对应的大驼峰命名
 
* 【推荐】每个React组件，都应该使用一个以组件命名的文件夹包裹，组件入口为index.js, styles.scss 或者 styles.less, styels为统一使用复数形式，子组件也应该参考同样的规则。
    正例: card/index.js | card-item/styles.scss
    反例: card-item/card-item.js | card/card.scss | card/style.scss
    
5. 【推荐】样式表应尽量减少类之间的嵌套
    正例： .container{} .container-card{} 
    反例： .container{.card{}}



