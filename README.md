# ChatGPT-3.5-AccessToken-Web
本项目基于使用Access Token的方式实现了网页版 ChatGPT的前端，不需要openai的api额度，是用<a href="https://github.com/Yidadaa/ChatGPT-Next-Web" target="_blank" title="ChatGPT-Next-Web">
ChatGPT-Next-Web</a>项目进行修改而得，另外本项目需要的后端服务，需要部署<a href="https://github.com/pengzhile/pandora" target="_blank" title="pandora项目">pandora项目</a>


## Access Token

* 官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
* 也可以访问 [这里](http://ai-20230626.fakeopen.com/auth) 拿 `Access Token`
* `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。


## 部署机器说明
* 在本地或者国内服务器都可以部署，不需要海外服务器

## 如何搭建运行
* 部署的机器安装python3,推荐python3.9 ,至少要python3.7以上版本
* 获取 Access Token
> 部署pandora项目
* 下载pandora项目：git clone https://github.com/pengzhile/pandora.git
* cd pandora
* 新建token.txt文件，把获取到的 Access Token放进去，保存文件
* pip install .
* pandora -s -t token.txt
> 部署本项目
* 下载本项目：git clone https://github.com/xueandyue/ChatGPT-3.5-AccessToken-Web.git
* cd ChatGPT-3.5-AccessToken-Web
* 修改.env.local的CODE，如果为空，则表示不需要密码访问
* yarn install && yarn build && yarn start

>PS：如果不是同一机器上部署pandora项目和本项目，又或者部署pandora项目使用非8008端口，那需要修改本项目用到8008端口的url



## 开源协议

> 反对 996，从我开始。
[Anti 996 License](https://github.com/kattgu7/Anti-996-License/blob/master/LICENSE_CN_EN)


## 其他说明


* 项目是站在其他巨人的肩膀上，感谢！
* 喜欢的可以给颗星
* PHP是世界上最好的编程语言！
