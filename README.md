# UNIAPP_WEB
面试题：
一：简答题
1、css中position有几种定位方式,有什么作用？
5种 static,fixed,absoluted,relative, sticky
Static（静态）:HTML 元素默认情况下的定位方式为静态。静态定位的元素不受 top、bottom、left 和 right 属性的影响。position: static的元素不会以任何特殊方式定位，它始终根据页面的正常流进行定位。
Relative（相对）：元素相对于其正常位置进行定位。设置相对定位的元素的 top、right、bottom 和 left 属性将导致其偏离其正常位置进行调整。不会对其余内容进行调整来适应元素留下的任何空间。
Fixed：元素是相对于视口定位的，也就是说即使滚动页面，它也始终位于同一位置。 top、right、bottom 和 left 属性用于定位此元素。
Absolute（绝对）：元素相对于最近的定位祖先元素进行定位。如果绝对定位的元素没有祖先，它将使用文档主体（body），并随页面滚动一起移动。
Sticky（粘性）：元素根据用户的滚动位置进行定位。粘性元素根据滚动位置先是相对（relative）然后是固定（fixed）。起先它会被相对定位，直到在视口中遇到给定的偏移位置为止，然后将其“粘贴”在适当的位置，即使滚动也不变。
2.JavaScript中有几种类型，哪些值会被隐式转换为false
有8种类型，Number、String、Boolean、undefined、object、Null，Symbol，bigINT
以下几个字符串会被隐式转换为false：undefined
null
false
0
NaN
""或’’（空字符串，不能有空格）

3.vue生命周期有哪几个阶段,prop,data初始化在哪两个生命周期之间？
有4大阶段：1、初始化阶段，包含beforeCreate（创建前）和created（创建后）两个小阶段；2、挂载阶段，包含beforeMount（载入前）和mounted（载入后）两个小阶段；3、更新阶段，包含beforeUpdate（更新前）和updated（更新后）两个小阶段；4、销毁阶段，beforeDestroy（销毁前）和destroyed（销毁后）两个小阶段。
Prop，data初始化在created和beforeMount之间。

 4.vuex有哪几种属性,怎么使用,哪些场景使用它

1：State：定义了应用程序的状态，就是我们要管理的数据。存放应用程序的状态（数据），所有组件共享。它是Vue实例的data属性的替代品，但是通过它存储和管理的状态，可以在整个应用程序中实现全局共享，即不同的组件可以通过定义的getter和setter访问同一状态数据。

2:Getters：用于获取State中的状态，主要用于对state进行逻辑上的组合和应用，类似于Vue组件中的计算属性。

3.Mutations：用于修改state中的数据，是唯一可以修改state的地方。mutations接收state作为第一个参数，接收payload作为第二个参数。用于修改State中的状态，只能同步执行。Mutation必须是同步函数，因为它们不能处理异步行为，异步行为应该放在Action中处理。

4.Actions：用于异步操作和提交mutations，在actions中可以进行任何异步操作，最后再提交到mutations中同步修改state。actions接收context作为第一个参数，其中包含了state、getters和commit等属性。可以包含任意异步操作（例如从服务器获取数据），可以用Mutation通过提交（commit）来修改State。

5.Modules：用于将store分割成模块，每个模块都拥有自己的state、mutation、action、getters和子模块，以便提高应用程序的可维护性。将State、Getter、Mutation、Action模块化，便于组件化和模块化开发。


二，选择题
1.B 2.A 3.C 
4.当我在工作中没有思路时，会用准确的prompt来引导chatGPT回答我的问题，给予我思路，而不是直接把整个代码丢进去，只有好的问题，它才能回答我好的答案。
