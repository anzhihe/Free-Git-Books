### Bug分支

我们在开发分支上正常开发，这个是master分支上有个bug需要我们紧急修复一下，这个时候就需要用到临时Bug分支，但是我们开发还没有完成，还不能提交，这个时候我们可以把我们的工作环境隐藏起来。

```
git stash
```

![](https://tva1.sinaimg.cn/large/006tNbRwly1ga70g4yjpvj31ys0sw0z2.jpg)

通过命令，可以把当前的工作隐藏起来。修复完bug会回来继续开发。

通过创建hot_fix分支来修改master分支，修复完成后，在提交到master上。

![](https://tva1.sinaimg.cn/large/006tNbRwly1ga70m5qpt7j31yu0ro7b1.jpg)

![](https://tva1.sinaimg.cn/large/006tNbRwly1ga70jajqivj31ja0u0ti9.jpg)

![](https://tva1.sinaimg.cn/large/006tNbRwly1ga70kxn7wdj31xk0u0tfi.jpg)

### 回到开发分支

```
git stash pop  # 恢复隐藏内容并删除
```

![](https://tva1.sinaimg.cn/large/006tNbRwly1ga70ooii77j31mz0u0ah2.jpg)