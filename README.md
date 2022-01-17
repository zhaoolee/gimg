# gimg
自建Github图床代理


## 开启本项目的目的


我有一个改进Github图床的想法，Gtihub是很好的图床，但无法过墙，我可以租一台香港服务器，或者给国内服务器翻个墙，然后把备案好的域名绑定到服务器，服务器开一个反向代理的服务，比如 https://github.v2fy.com/get_image 如果有一张github图片是https://raw.githubusercontent.com/zhaoolee/EasyTypora/master/README/1610212815891fPTxkEFj.png 那国内获取的规则就是  https://github.v2fy.com/get_image?href=https://raw.githubusercontent.com/zhaoolee/EasyTypora/master/README/1610212815891fPTxkEFj.png


markdown文件里面这样写  ![图片说明](https://github.v2fy.com/get_image?href=https://raw.githubusercontent.com/zhaoolee/EasyTypora/master/README/1610212815891fPTxkEFj.png)


这样服务器可以不存储图片，服务器忘了续费，也可以找到原图存储地址，也可以通过图片url规则溯源找到原图，另外在  https://github.v2fy.com/get_image 加一些跨域请求的限制，也能避免别人白嫖流量
