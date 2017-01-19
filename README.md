# GitHubDemo之前也有过一个小小的demo，当然只是小小的啦，但是测试失败了，我也不知道原因是什么，就暂且不去追究吧，今天又花了大概半个小时写了
写了一下这个例子，其实也没有什么，就是想把我的library放到JitPack.io上面去，下次我就好方便的引用了，
哈哈先简单的介绍一下步骤吧，其实也是很简单的

1，第一步就是在你的project下面新建一个library，这个应该不用我多说了吧

2，把你的project项目上传到GitHub上面去，这个也不用多说了吧

3，等等，先别上传，先在你的project下的bulid.gradle中配置


classpath 'com.github.dcendents:android-maven-gradle-plugin:1.3'
具体的版本可是有讲究的，具体参考官网，你的gradle是什么版本的就对应什么版本

再在你的moudle的bulid.gradle中配置apply plugin: 'com.github.dcendents.android-maven'
group='com.github.DavidWeiZhong'//你的grihub地址，不要写错了
然后你就可以上传了
记得改一下版本，把你的版本改为什么v1.0更好看一点，淡然你要是不想改也无伤大雅

4，进入JitPack中配置你的项目url就可以了，接着你就可以很方便的通过
compile 'com.github.DavidWeiZhong:GitHubDemo:v1.0'引用了是不是很开心，是不是很开兴，是不是很开心，是不是很开心，哈哈哈哈
