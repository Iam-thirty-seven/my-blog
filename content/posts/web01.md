---
title: web01
date: 2026-09-29
category: 介绍            # 分类（每篇一个，可选）
tags: [记录]      # 标签（可多个，可选）
cover: /assets/images/flower-imag.png  # 封面图（可选）
summary: 好记性不如敲一遍,html框架和css的display
draft: false              # true = 草稿，发布时改回 false
---
记录搭建html框架->盒子模型->display
# html框架
![框架](/assets/images/web01/html5.png)
```css
head 放不可见的(meta charset 编码,name = "viewport"(移动专用);
title 网站名称 ,style css样式) link 引用外部 
body放可见的 语义化标签 header(头部) nav(导航栏) main(主体); 
aside(侧边栏) footer(脚部)  section (区块) article (文章);
```
## 盒子模型（Box Model）
![盒子模型](/assets/images/web01/Box-Model.png)
```css
margin 外边距 border 房子的线 ;
padding 内边距(文章与线的边距) content(文章/图片 本身);
```
### css的display属性
![display属性](/assets/images/web01/display.png)
```css
display:none(此元素不会显示),flex(子级元素横向排列),inline(行内显示,无宽高);
block(此元素将显示为块级元素,前后有换行符),grid(二维网格布局);
隐藏用 none;
横排用 flex;
换行用 block;
行内用 inline;
按钮用 inline-block;
网格用 grid;
------------------------------
display:none;
display:flex;[justify-content](主轴对齐)
偏左(默认);                 居中                  偏右
justify-content:flex-start; just-content:center; justify-content:flex-end; 
两端对齐,中间等距               每个元素左右等距                所以间距完全相等
justify-content:space-between; justify-content:space-around; justify-content:space-evenly;
              [align-items](交叉轴对齐)
    拉伸填满(默认)        顶部对齐              垂直居中                底部对齐
align-items:stretch; align-items:flex-start; align-items:center; align-items:flex-end; 
文字基线对齐
align-items:baseline;
------------------------------
/* 1. 完全居中（水平+垂直） */
display: flex;
justify-content: center;
align-items: center;

/* 2. 两端对齐（导航栏） */
display: flex;
justify-content: space-between;
align-items: center;

/* 3. 偏左 + 垂直居中 */
display: flex;
justify-content: flex-start;
align-items: center;

/* 4. 偏右 + 垂直居中 */
display: flex;
justify-content: flex-end;
align-items: center;
```
今天就到这里，再次感谢您的阅读，再见 <a href="https://space.bilibili.com/397385348?spm_id_from=333.1007.0.0" style="display:inline-block; border:2px solid #4a90d9; padding:4px 12px; border-radius:6px; text-decoration:none; color:#4a90d9;">不许点人家了啦~</a>