1.组件通信
    (1) props $emit 解决父子组件层数较少的情况
    (2) $attrs $listeners 解决组件嵌套多层关系
    (3) 中央事件总线 $bus new Vue()
        $on() $emit挂载的同一个实例化对象，解决兄弟组件传值
    (4) vuex 的流程图，脑子要有这个概念
2.声明周期的图示
3.路由的使用
    3.1 引入包(两个全局的组件 router-link to属性 router-view(匹配路由组件的出口))
    3.2 创建实例化VueRouter对象
    3.3 匹配路由规则
    3.4 挂载new Vue()实例化对象中
    给vue实例化对象挂载两个对象 this.$router(它就是VueRouter)
                              this.$route(配置路由信息的对象)
命名路由
    绑定自定义的属性 :to = "{name: '路由的名字'}"
路由的参数
    path: '/suer/:id'
    :to = "{name: 'user', params: {id: 1}}"

    path: '/user'
    :to = "{name: 'user', query: {userId: 1}}"

嵌套路由(应用子的路由时不同的页面结构)
    一个router-view 中嵌套另外一个router-view
