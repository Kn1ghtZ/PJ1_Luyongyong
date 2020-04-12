我的设计文档
=======
## 姓名：陆勇雍  
## 学号：19302010034
------------------
## Github地址：  https://github.com/Kn1ghtZ
## Github Pages地址：
-------------------
## 项目完成情况： 
### 要求均完成
------------------
## Bonus完成情况和解决方法：
Bonus1：  
完成了bonus1，只使用normal文件夹中的自由版式进行排版。  
当所用图片宽高均大于容器时，可以设置img的width和height为100%，相当于把图片缩小不会失真，也可以把超出的部分通过设置父元素overflow：hidden和img的object-fit:cover，完成图片剪裁。对于宽高中至少有一个小于容器的宽高时，可以设置img的width和height使之铺满整个容器。  
在主页中，图片展示部分的六张图片采用了normal文件夹中的6张320x240的图片，img的父元素div也设置了宽高320x240.  
在浏览页中，图片展示部分考虑到各个图片的宽高不一，故对img的object-fit设置为cover，对其父元素设置宽高和overflow：hidden，完成排版。但是考虑到在较窄的屏幕下图片宽高太大时无法显示完整的问题，使用了媒体查询设置了图片的高宽以适应小屏幕，达到完全显示的效果。  
在我的收藏、我的照片页面中，对img设置了与父元素相同的宽和高。  

Bonus2  
对于主页面，以一个父级作为布局容器，来配合子级元素实现变化效果
在不同屏幕下 通过媒体查询来改变这个布局容器的大小，在改变里面子元素的排列方式和大小，从而实现不同屏幕下，看到不同的页面布局和样式变化。即通过
```
@media screen and (max-width:1200px){
  .hotpicture{
      width: 366px;
  }
```
可以使得当屏幕宽度小于等于1200px时，热门图片展示部分的宽度变为366px，从之前的一行3张图片变为一行1张图片，完成响应式布局。  

对于其余页面，通过对页面中大部分元素的各个数值（如宽高、字体大小、内边距、外边距等）的单位设置为vw（即视宽，1vw等于视口宽度的1%）vh（即视高，1vh等于视口高度的1%），对部分元素（主要是子元素）设置其宽高单位为%，通过等比例放缩，得到在不同⻓宽⽐的设备上时，不失去原有的排版和设计。

经chorme的调试功能，在大部分手机机型上（即移动设备，如iPhone6/7/8，iPhone6/7/8 plus，iPhone X，iPad，iPad pro等）运行时也能尽量保持原有的排版和设计。  

Bonus3  
尽量美观，色彩平和。特别是在背景方面，为了不起到喧宾夺主的反作用，特意选取了条纹型的背景图片，并通过ps改变其主要色调，应用在不同的页面上，使得观感不枯燥。

---------
## 对PJ1和本门课程的意见和建议：  
通过PJ1，我对html和css有了更加牢固的掌握，明显觉得使用html和css越来越熟练,也学会了通过搜索引擎以及查找各个教程解决实际问题。也感谢老师和助教们的辛勤付出。  
对于本门课程，老师对于知识概念的讲解十分全面且细致，也有配套的代码和书籍供我们学习，受益匪浅。有一点小小的建议是如果能进行实战演练或是对目前主流页面上各个元素的分析可能会更能加深学生的理解。