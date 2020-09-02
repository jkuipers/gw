你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# What is `gw`?

`gw` is a `gradle`/`gradlew` wrapper written in `Go`. It's a clone of `gdub`
that works the same way (https://github.com/dougborg/gdub). The reason I
wanted to create this in Go is to be able to run it on OSX, Unix and Windows.

## Building

Since I do not have any binaries yet, you have to build it yourself.

    go build

Run it using the `gw` command:

    ./gw

## Cross-platform build

Using goxc (https://github.com/laher/goxc) to build for all supported
platforms.

Before running the commands you have to build tools for every platform:

    goxc -t

Then, compile binaries for the platforms:

    goxc xc

To clean output folders:

    goxc clean
