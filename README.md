# 前言

随着私家车数量的增加，车位资源变得愈发紧张，为有效利用车位资源，降低车主的停车成本，我们开发了这款“私家车位共享系统”。本项目基于SSM框架，结合微信小程序和Uniapp技术，致力于为用户提供便捷、高效的车位共享服务。

# 内容介绍

私家车位共享系统主要实现了以下功能：

1. 车位所有者可以发布车位空闲时间，设置共享规则，实现车位共享；
2. 车主可以根据自己的需求查询附近空闲车位，并进行预约；
3. 系统提供支付功能，车主可以在预约成功后完成支付；
4. 系统还具备车位管理、订单管理、用户管理等功能，方便管理员进行运营管理。

# 技术介绍

- 语言：Java
- 使用框架：Spring、Spring MVC、MyBatis
- 微信小程序
- 前端技术：JS、Vue、CSS3、Uniapp
- 开发工具：IDEA/Eclipse、Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

# 核心代码

以下为车位预约功能的部分代码：

```java
// 车位预约接口
@RequestMapping(value = "/appointSpace", method = RequestMethod.POST)
public ResponseEntity<?> appointSpace(@RequestBody Appointment appointment) {
    try {
        // 校验参数
        if (appointment.getUserId() == null || appointment.getSpaceId() == null) {
            return ResponseEntity.badRequest().body("参数不完整");
        }
        // 预约车位
        appointmentService.appointSpace(appointment);
        return ResponseEntity.ok("预约成功");
    } catch (Exception e) {
        return ResponseEntity.status(HttpStatus.INTERNAL_SERVER_ERROR).body("服务器异常");
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
![封面图片](https://img12.360buyimg.com/ddimg/jfs/t1/348105/36/2881/259487/68c4d7beFc8a07d7a/f4feda5ac9eb3071.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/340833/1/10029/25355/68c4d796Fdba86bdf/dd91888f9b8d950e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/344673/5/2441/255965/68c4d797Ff2a07def/a0e56e88272cd7bc.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/337096/32/8440/20924/68c4d797F35566cee/245b6106ff138b4c.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/327952/25/18884/28128/68c4d797F4556bc8c/d23d08042265f6d1.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/328489/26/19275/22984/68c4d797Fae2c8f02/a6a3dd0d7f92045b.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/334908/34/12508/67727/68c4d798F8921488c/ea9c16e970c697bf.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/348694/38/2925/69526/68c4d798Fc0e1f500/874b02c64ee037a6.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/339553/35/10269/76985/68c4d799Fbaf2cd85/1b12100cf63812de.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/326111/36/19142/77053/68c4d799F3fd88a71/5f509c91f182a660.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
