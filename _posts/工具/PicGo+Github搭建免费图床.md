---
style: summer
---
#  图床
## Github repo图床

Github的repo也可以储存东西，最直接的就是程序的版本控制，当然也可以用来当作备份储存，用来储存图片（github官方回复是：该行为不构成abuse，如果把github当图床算滥用，那么那么多人把微博当图床怎么就理所应当捏）。其实github对于国内的响应速度并不快，而且时不时被block，所以用github当图床完全是出于储存个人用途的自创图片，并不能当CDN使用。github自从被微软收购后，我对github的信心大增，代码以前只敢用git管理保存在本地，现在可以放心大胆上传到github了（很多是private，所以不可见），github图床主要就是图个稳定，也并不是想恶意刷github服务器的流量，恶意影响大家的体验。

1.  新建repo，名称任意

2.  打开账户/Settings/Developer settings/Personal access tokens,点击Generate new token

    ![](//upload-images.jianshu.io/upload_images/17029678-88e1807b0a33255e.png?imageMogr2/auto-orient/strip|imageView2/2/w/233/format/webp)

    image

    ![](//upload-images.jianshu.io/upload_images/17029678-7656c08d619ed359.png?imageMogr2/auto-orient/strip|imageView2/2/w/1002/format/webp)

    image

3.  在弹出的产生token页面，Token description随意填写，但是一定要勾选上这几项

    ![](//upload-images.jianshu.io/upload_images/17029678-55b2842f6875b416.png?imageMogr2/auto-orient/strip|imageView2/2/w/784/format/webp)

    image

4.  下载PicGo客户端对应的版本并安装，github地址：[https://github.com/Molunerfinn/PicGo/releases](https://links.jianshu.com/go?to=https%3A%2F%2Fgithub.com%2FMolunerfinn%2FPicGo%2Freleases)

5.  启动PicGo后，打开设置界面，点击

    ![](//upload-images.jianshu.io/upload_images/17029678-3ed6d235f87629c4.png?imageMogr2/auto-orient/strip|imageView2/2/w/800/format/webp)

    image

    在第一栏填入你的github名称/repo名称；在第二栏填入你的分支名称，默认为master；在第三栏填入你刚才申请到的Token；第四栏填入你的repo中的储存路径；最后点击确认，再点击设为默认图床

6.  使用QQ截图Ctrl+Alt+A或者微信的Alt+A截图后，按下Ctrl+Shiht+P快捷键即可自动上传到github对应的repo中，上传完成后，会有提示，自动将对应的图片地址送入剪贴板中，直接Ctrl+V即可粘贴对应的地址出来了~~

## PicGo中使用其他图床

PicGo一共支持多种图床：

![](//upload-images.jianshu.io/upload_images/17029678-8384285fdd2d24ee.png?imageMogr2/auto-orient/strip|imageView2/2/w/390/format/webp)

image

*   其中SM.MS图床是免费且不需要账号的图床，缺点是无法查看历史上传的图片，因此每次使用同一张图片都需要重新上传一张一样的获取新的地址，或者是拷贝之前上传过的地址
*   ~~微博图床，我设置好账号和密码后，并不能正常上传，原因应该是微博限制了必须加上验证码才能登陆，所以微博图床对于这款程序并不太友好，应该说微博图床上传图片都很麻烦，登录过程就很麻烦，如果手动上传，感觉更麻烦，所以还是不推荐用微博图床~~ 经过再次测试后，发现**微博第一次在某台电脑上登陆**时，验证比较复杂，需要输入验证码，还有可能需要验证手机号，所以可以使用浏览器在网页中打开微博，然后登陆自己的微博，登陆成功后，在使用PicGo选择微博图床，进行上传测试，这时就可以正常上传了

    ![](//upload-images.jianshu.io/upload_images/17029678-56786d5429dd4183.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/211/format/webp)

    image

*   腾讯、阿里的对象储存，上面说了，免费都有时间，过了免费时间后，可能需要付费，主要优势就是CDN加速了，超快，当然如果你的博客看的人多了，那么流量也多，费用也贵
*   七牛云和又拍云可以申请免费储存空间，是不错的选择，但是也要小心流量被刷导致扣费、封号，具体可以看看别人的前车之鉴

* * *

![](//upload-images.jianshu.io/upload_images/17029678-4a5223963ae5106a.png?imageMogr2/auto-orient/strip|imageView2/2/w/768/format/webp)

image

*   Imgur也是免费的图床，是国外网站，相对国内速度不太理想，还是SM.MS速度快些

# Github图床缺点

1.  对应储存图片的repo必须是public，如果是pravite，那么图片地址会带有一个随时刷新token，这样虽然repo他人不可见，但是也没法作为图床用
2.  图床每添加一张，那么会提交一次commit，这样会导致你的github动向表部分一片绿。。。。。虽然这样显得你很活跃，但是真正点进去会发现你的代码更新并没有你真正提交commit的频率高。

# 禁止滥用

对于个人MD使用来说，Github是一个相对稳定（微软收购后更加稳定了）、不用付费、可以查看历史、速度还行的图床。但是绝对不适用于大流量的场所，只限于个人小流量使用！！！！！！！！！！！！！！！

作者：FelixCoder
链接：https://www.jianshu.com/p/d51258ef5484
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
