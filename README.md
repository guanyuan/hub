# hub
for personal usage
=========================================================
http://le0zh.github.io/2016/06/21/eslint+in+react+babel+webpack/
使用airbnb，包含react和jsx规则
{
  parser: "babel-eslint",  //检查es6代码
  "extends": "airbnb",
  "rules": {  //对规则进行微调
    "no-unused-vars": 0,
    "max-len": [1, 120, 2, {ignoreComments: true}],
    "prop-types": [2]
  }
}

调整airbnb规范
eslint: react/prefer-es6-class  使用class extends component方式创建组件
eslint: react/jsx-pascal-case  组件名使用驼峰规则
eslint: jsx-quotes  jsx的属性，使用双引号
eslint: react/wrap-multilines  用括号包裹多行 JSX 标签。 

持久化登录信息
copiedUser.fullName = encodeURIComponent(copiedUser.fullName || '');
$localStorage.currentUser = btoa(JSON.stringify(copiedUser));


========================================
在ES6里，可以统一使用static成员来实现

//ES6
class Video extends React.Component {
    static defaultProps = {
        autoPlay: false,
        maxLoops: 10,
    };  // 注意这里有分号
    static propTypes = {
        autoPlay: React.PropTypes.bool.isRequired,
        maxLoops: React.PropTypes.number.isRequired,
        posterFrameSrc: React.PropTypes.string.isRequired,
        videoSrc: React.PropTypes.string.isRequired,
    };  // 注意这里有分号
    render() {
        return (
            <View />
        );
    } // 注意这里既没有分号也没有逗号
}
========================================
replace jquery ajax: https://github.com/mzabriskie/axios
keyboard event: http://blog.garstasio.com/you-dont-need-jquery/events/#keyboard-events
onKeyDown(e) {
        if (!this.state.focus) {
            return;
        }

        /** Tab */
        if (e.keyCode === 9) {
            return this.onBlur();
        }

        /** Arrow Down */
        if (e.keyCode === 40) {
            this.handleArrowDown();
        }

        /** Arrow Up */
        if (e.keyCode === 38) {
            this.handleArrowUp();
        }
    }
    
    
    onKeyPress(e) {
        if (!this.state.options || this.state.options.length < 1) {
            return;
        }

        /** Enter */
        if (e.keyCode === 13) {
            return this.handleEnter();
        }
    }





http://qiutc.me/post/%E8%B0%88%E8%B0%88-react-router.html

https://github.com/reactjs/react-router/blob/master/docs/guides/RouteConfiguration.md
路由readme

https://web-design-weekly.com/2015/01/29/opinionated-guide-react-js-best-practices-conventions/

1、将productRow 和 productList写在同一个文件中
2、Conditional JSX  提取一个变量进行渲染
3、声明prototypes
propTypes: {
        arrayProp: React.PropTypes.array,
        boolProp: React.PropTypes.bool,
        funcProp: React.PropTypes.func,
        numProp: React.PropTypes.number,
        objProp: React.PropTypes.object,
        stringProp: React.PropTypes.string,
    }


4、focus到输入框： this.refs.theInput.focus();


===== LICENSE BEGIN =====
===== LICENSE END =====

路由跳转： this.props.history.pushState(null,'app');//跳转到Router定义路径为app
11194-31102015
可以用 babel-plugin-add-module-exports 这个插件 然后 require('../common/routes').default 后面default 就不用写了.
00000xgI2JAR"YTpqcRVYdZIrNIFnP
react children的正确使用： https://xieguanglei.github.io/blog/post/react-tips-children.html
http://www.w3ctech.com/topic/1845
CqVrFCZXDkFX5Di6Vno0TLPCKQppCx
1、对loader都设置exclude
2、问林帆要最新的node
5dqTTwzhaQfN9g7vVnpK77uK6xR9FO
weibo： http://weibo.com/u/1879746691?source=blog&is_all=1#_rnd1472137945395

https://leozdgao.me/modern-karma/


https://github.com/lelandrichardson/enzyme-example-mocha
http://airbnb.io/enzyme/docs/guides/mocha.html
