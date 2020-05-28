# java-finally
try-catch-finally-return执行顺序问题
<br>
如果有finally，finally代码块一定会执行
如果有finally，但finally里面没有return,那么会先执行完try/catch里面的语句，然后再执行finally里面的代码，然后try/catch有结果则返回其结果
如果有finally，并且finally里面有return,那么先执行完try/catch里面的语句，然后再执行finally里面的代码，
并且finally里面return的结果会覆盖try/catch的，如果catch中再次抛出异常，会被finally的return吃掉，不抛出异常了，
<br>
作者：小乌龟爸
链接：https://www.jianshu.com/p/8a0b113edc96
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
<br>
