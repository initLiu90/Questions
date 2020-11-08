# mac Android Device monitor no response

1. 因为 jdk 版本不对---使用 1.8.0_151 及以下的版本解决
2. Android/sdk/tools/lib/monitor-x86_64/plugins/org.eclipse.swt.cocoa.macosx.x86_64_3.100.1.v4236b.jar
   版本太低，更新 jar。
   下载
   http://ftp.yz.yamagata-u.ac.jp/pub/eclipse/eclipse/downloads/drops4/R-4.7.3a-201803300640/swt-4.7.3a-cocoa-macosx-x86_64.zip
   解压后，吧 swt.jar 复制到 Android/sdk/tools/lib/monitor-x86_64/plugins/目录下替换原来的 org.eclipse.swt.cocoa.macosx.x86_64_3.100.1.v4236b.jar

# mac 不能启动 Android Device monitor

因为 Android Device monitor 需要监听 8700 端口，这个端口被 Android studio 占用。
需要 kill android studio 进程

# mac Android Device monitor 启动之后什么也不显示

然后用户目录下的~/.android/monitor-workspace 的目录
