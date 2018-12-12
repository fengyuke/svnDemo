# svnDemo
打包部署时候获取svn版本号、时间戳等信息


版本信息获取可以解决项目升级页面缓存的问题，此demo每次打包时候会获取svn的版本信息及时间戳等信息，
打包过程中也会在控制台中显示出来，可以看一下版本信息是否正确。

这里有一点特别的要注意，当此项目仅有你自己操作，你修改好代码提交到SVN此时你本地的版本信息没有加1；
此时打包，版本信息还是上一次的版本信息，

repository = 
path = 
revision = 2315
mixedRevisions = false
committedRevision = 2315
committedDate = 2018-12-12 15:38:22 +0800 (Wed, 12 Dec 2018)
status = 
specialStatus = 

此时要做一次项目的update，则此项目此时已经升级到最新版本，此时打包会获取到最新的版本号

repository = 
path = 
revision = 2316
mixedRevisions = false
committedRevision = 2316
committedDate = 2018-12-12 15:48:22 +0800 (Wed, 12 Dec 2018)
status = 
specialStatus = 


至于后续是否有更好的解决方案，找到后再次更新
