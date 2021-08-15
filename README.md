# 浏览器渲染原理
## 浏览器渲染过程：
1. 根据HTML构建HTML树
2. 根据CSS构建CSS树
3. 将两棵树合并成一颗渲染树
4. layout布局（文档流，盒模型，计算大小和位置）
5. paint绘制（把边框颜色，文字颜色，阴影等画出来）
6. composite合成

## 三种更新方式：
* JS/CSS>样式>布局>绘制>合成
* JS/CSS>样式>绘制>合成
* JS/CSS>样式>合成

# CSS动画的两种做法（transition和animation）
## transition：
* transition:属性名称 过渡时间 时间函数 延迟;
* 属性间用空格隔开；transition:all 1s; 可以为所有样式添加过渡效果
## animation：
1. animation:时长|过渡方式|延迟|次数|方向|填充模式|是否暂停|动画名;
2. 我的代码：
``` CSS
@keyframes xxx{
    0%{
        transform:translate(0,0);
        }
    50%{
        transform:translate(200px,0);
    }
    100%{
        transform:translate(200px,200px);
    }
}
```
# 其他
* [用transition写的跳动的红心](http://js.jirengu.com/jihidecote/1/edit?html,css,output)
* [用animation写的跳动的红心](http://js.jirengu.com/fevajehoje/1/edit?html,css,output)
