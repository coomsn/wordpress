去除ftp限制

```
chown -R www /home/wwwroot/wordpress
```

wordpress 抱歉，您无权上传此文件类型。
在网站根目录，编辑 wp-config.php，在 /* That’s all, stop editing! Happy blogging. */ 前面填入代码：
```
define('ALLOW_UNFILTERED_UPLOADS', true);
```
