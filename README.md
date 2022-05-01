# Epay
2020.02彩虹易支付原版开源
最新安装
宝塔添加站点
上传源码

安装
•	推荐使用宝塔面板安装，以下教程为宝塔面板安装教程，其他环境请参考自行配置
1、下载源代码,Clone or download->Download ZIP
2、宝塔面板中新建网站，设置：
 + 网站目录->运行目录 设置为public并保存
 + 伪静态 设置为thinkphp并保存
 + 默认文档 设置将index.html放在第一行并保存
3、打开网站目录 config/database.php ，设置好您的mysql账号密码。
4、导入数据库文件（位于根目录）vmq.sql到您的数据库。
5、至此网站搭建完毕，请访问后自行修改配置信息！默认后台账号和密码均为admin
升级说明：请您直接下载新版本覆盖旧版本即可！
调用
•	请部署完成后访问后台，有详细的Api说明











V免签能够免签约收款，但是很多都不支持V免签，对接上易支付就很方便了，很多源码都支持易支付的协议。
准备好一台VPS。搭建好宝塔面板。
上传好源码后
设置伪静态
location / {
 if (!-e $request_filename) {
   rewrite ^/(.[a-zA-Z0-9\-\_]+).html$ /index.php?mod=$1 last;
 }
 rewrite ^/pay/(.*)$ /pay.php?s=$1 last;
}
location ^~ /plugins {
  deny all;
}
location ^~ /includes {
  deny all;
}
 
 
成功安装，如需重新安装，请手动删除install目录下install.lock文件！
上传V免签插件。
 
 
配置好V免签密钥~！
 
创建好商户直接对接即可。
 
源码下载~！
限时免费~！易支付源码，内涵最新监控端
sspanel-metron对接易支付插件 自行去TG群下载
付费代搭建进![进TG群](https://t.me/huashengkeji1)


