# XXScrollAndPageView
This is a custom view for auto page turning view. 

> 这个是我自己封装的一个循环滚动视图，里面包含一个demo和封装的类。封装的特点是节省内存，并且可以通过代理来实现点击事件.

## 使用方法：
####1. 基本使用：把创建好的view或其子类放在NSMutableArray 中并赋值给参数imageViewArr,这些就是你要循环滚动显示的视图。
####2. 设置相关属性：shouldAutoShow： 是否自动滚动显示。
####3. 设置代理：在代理方法`- (void)didTapScrollView:(XXScrollAndPageView *)view atIndex:(NSInteger)index` 中可以实现点击某个视图的点击事件。其中index 是从1 开始，即第一张index为1，依此类推。
####4. 其他：滚动时间间隔和滚动动画的持续时间我都用define的方式放在开始，如果有需要可以自己修改。
