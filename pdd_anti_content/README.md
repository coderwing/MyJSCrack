
# node服务使用
```shell
> node demo_pdd_github.js 
> 应用实例，访问地址为 http://:::8085
```
- 可能会报错，如提示：Error: Cannot find module 'express'，使用命令安装express模块即可：> npm install express
- 然后再执行 > node demo_pdd_github.js 

# 访问
直接在浏览器请求，或者使用python、java等的http的get请求即可，得到结果：
anti_result:"0anAfxnUXOtoY9EVWRla2eaf3bFgXgzj-w-XIMdCMZ0_IyIaDZ_7tE-putUpzKOrwFr90AiV9RZPb-s0i0-W60JqcDd9t0j0w_OW9xDUTGJroO0tyw9AumouBJv10u_0la9CmD6nCk5Sr03yCNCO4ZI40aSS8ZYsbeFh1NK_8WxgHOCM1FiF-1suBuii0xpapoKyD2XgJ9nFPTEr9V0Rw2jd4_8umgesze7bbeO4XgLqG2O8IzSkvgcSPb40Nd9uFBkUtJdOcdaQa4ibf3FAqkFy04SD7ZznlYwItBK7yOzzGUv3cVOZ-9us1ZdazzjZKGgyTxvUce5n9-xwdBcVSwwFWePveZZwNbXY_f6AeLPwi-uw3v-3fk1-3wbW5krhBZpfPSF3dHRqFIUffaF1uTHIOftJkDtl4Q8LHZuw7iq3KOFY7pxElqUoxmMhLgu3SoMoiA6oz2315rgDlFgrAhanDHG2h8tMKWROMr2C8naTC"

--------







# pdd_anti_content（2019-07-11 08:33 测试可成功获取数据）
- js破解之再战pdd（搜索商品列表页anti_content参数破解）（~~不是吧，好像历时一天多就凉了？~~）
- 2019-07-01 测试发现，单个ip若首次使用示例py代码调用为不成功时，此时使用浏览器访问搜索链接则需要登录，此时用户完成登录，后再使用py示例代码调用则正确返回数据。（猜测ip与用户登录态存在某些权重绑定，欢迎大家测试）（测试环境为本机ip，本机chrome浏览器）
- 2019-07-05 测试发现，首先用浏览器成功访问一下pdd的搜索，不管是登录也好，滑块也罢，只要浏览器能成功展示页面，此时使用py代码调用亦可成功。（还是猜测ip存在某些权重绑定，需要验证一下）（测试环境为本机ip，本机chrome浏览器）
- 特殊说明：本人测试同一anti_content有效调用次数为2次，目前ip限制较为严重，但代理不在本文讨论之列，请合理安排策略

## 文件列表

- demo_pdd.py（python调用示例）
- demo_pdd_github.js（nodejs接口示例）

## 介绍

- [js破解之秒破pdd](https://mp.weixin.qq.com/s/kj6RPBPdt8pyoSHzXQm87A)
- [js破解之再战pdd](https://mp.weixin.qq.com/s/jWquj66gZtamX25t6pNHlw)

## 其他

- 公众号：妄为写代码（欢迎有趣的朋友一起交流技术，互相学习）
- 简书专题：[JS破解&&Android逆向](https://www.jianshu.com/c/2b5f41371ebf)
- 个人简书：[花儿谢了6](https://www.jianshu.com/u/a26f80937a28)

## 示例

- 调用示例：[pdd搜索参数anti_content破解(06-26)](https://www.jianshu.com/p/58039dc72de8)

## 说明

- 本源码只作技术交流使用，请勿用以违法用途，由本源码直接或间接产生的法律问题，将由使用者自行承担
