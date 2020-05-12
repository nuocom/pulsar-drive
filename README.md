 ====  

这是一个 [修改版的goindex](https://github.com/) 

在 [原版goindex](https://github.com/donwa/goindex) 基础上添加了多盘支持、搜索、分页加载等功能。

`index.js` 包含 Workers 所需的代码.


> **安装部署可以参考原版，以下摘自原版 goindex 的部署说明：**


## 安装部署方案1  
1、在本地安装 rclone   
2、按照 https://rclone.org/drive/ 流程进行授权。  
3、执行 rclone config file 查看 rclone.conf 路径。找到root_folder_id和refresh_token记录下来。  
4、下载 https://github.com/donwa/goindex 中的 index.js  并填入 root 和 refresh_token  
5、复制代码 到 CloudFlare 部署。  

## 安装部署方案2  
作者不会记录refresh_token，但为避免纠纷，建议有条件的同学使用方案1进行部署  
1、访问[https://install.gd.workers.dev/](https://install.gd.workers.dev/)  
2、授权认证后，生成部署代码。  
3、复制代码 到 CloudFlare 部署。  

## 文件夹密码：
在google drive 文件中放置 `.password` 文件来设置密码。  
密码文件只能保护该文件不被列举，不能保护该文件夹的子文件夹不被列举。  
也不保护文件夹下文件不被下载。  

程序文件中 `root_pass` 只为根目录密码，优先于 `.password` 文件  

## 程序说明
本程序来源于GitHub大佬开源源码，我Fork下来备份仅供自己学习交流使用！
