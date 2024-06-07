
**本工具仅供安全测试人员运用于授权测试, 禁止用于未授权测试, 违者责任自负。**

## 简介
该工具使用了ExpDemo-JavaFX项目，保留了核心的数据包请求接口，使用jdk1.8环境开发。目前编写了oa等多个系列，对相关漏洞进行复现和分析，极力避免exp的误报和有效性。

截止到目前为止，已实现了用友、泛微、蓝凌、万户、帆软报表、致远、通达、红帆、金和、金蝶、广联达、华天动力总共12个OA。
全部是命令执行、文件上传类的漏洞，包括前台和后台，未编写log4j、fastjson相关漏洞。

用友已完成：
- 用友NC-BshServlet 远程命令执行
- 用友NC-BshServlet-bypass 远程命令执行
- 用友NC accept 文件上传
- 用友NC uapim 文件上传
- 用友NC mp 文件上传
- 用友NC saveXmlToFileServlet 文件上传
- 用友NC saveImageServlet 文件上传
- 用友U8CRM swfupload 文件上传
- 用友U8CRM getemaildata 文件上传
- 用友GRP-U8 UploadFileData 文件上传
- 用友GRP-U8 U8AppProxy 文件上传
- 用友GRP-U8 services 文件写入
- 用友GRP-U8 servlet 文件上传
- 用友U8 cloud文件上传
- 用友U9 PatchFile 文件写入
- 用友反序列化-1
- 用友反序列化-2
- 用友反序列化-3
- 用友畅捷通T+密码重置 	
- 用友畅捷通T+文件上传-1 	
- 用友畅捷通T+文件上传-2
- 用友畅捷通T+GetStoreWarehouseByStore反序列化
- 用友KSOA ImageUpload 文件上传
- 用友KSOA Attachment 文件写入
- 用友NC Cloud 文件写入 
- 用友NC Cloud 文件上传
- 用友移动管理平台Apk文件上传 	
- 用友移动管理平台Icon文件上传 	
- 用友U8-OA文件上传 	
- 用友UFIDA NC 文件写入
	
泛微已完成:
- 泛微OA KtreeUploadAction 文件上传
- 泛微OA uploaderOperate 文件上传
- 泛微OA weaver.common.Ctrl 文件上传
- 泛微eoffice OfficeServer 文件上传
- 泛微eoffice UploadFile 文件上传
- 泛微eoffice uploadify 文件上传
- 泛微eoffice ajax 文件上传
- 泛微BshServlet 远程命令执行
- 泛微ecology前台sql注入-1
- 泛微ecology前台sql注入-2
- 泛微ecology前台sql注入-3
- 泛微ecology WorkflowServiceXml命令执行
- 泛微ecology FileClient 文件上传
- 泛微ecology后台风格文件上传
- 泛微ecology后台流程命令执行
- 泛微emobile client命令执行
- 泛微emobile messageType命令执行
- 泛微emobile lang2sql文件覆盖

蓝凌已完成:
- 蓝凌OA 任意用户登录
- 蓝凌OA SSRF
- 蓝凌OA SSRF BeanShell 文件上传
- 蓝凌OA SSRF XmlDecoder 文件上传
- 蓝凌OA treexml 命令执行
- 蓝凌OA界面文件上传
- 蓝凌OA主题文件上传
- 蓝凌OA jg_service文件上传
- 蓝凌OA后台模板文件上传
- 蓝凌EIS api文件上传

万户已完成:
- 万户OA用户密码泄露
- 万户OA fileUpload 文件上传
- 万户OA officeserverservlet 文件上传
- 万户OA smartUpload 文件上传
- 万户OA OfficeServer 文件上传
- 万户OA senddocument 文件导入
- 万户OA wpsservlet 文件上传
- 万户OA SOAP 文件写入

帆软已完成:
- 帆软报表任意文件读取
- 帆软报表任意文件读取-bypass
- 帆软报表任意文件覆盖
- 帆软报表未授权命令执行
- 帆软报表channel命令执行-1
- 帆软报表channel命令执行-2
- 帆软报表后台插件文件上传
- 帆软报表后台主题文件上传

致远已完成:
- 致远session泄露processUpload文件上传
- 致远uploadMenuIcon文件上传
- 致远ajax文件上传
- 致远ajax文件上传-bypass
- 致远wpsAssistServlet文件上传
- 致远htmlofficeservlet文件上传
- 致远任意用户密码重置
- 致远audit-admin用户默认密码
- 致远audit-admin用户重置密码
- 致远后台模板文件上传
- 致远后台模板管理器文件上传
- 致远后台表格文件写入
- 致远后台ofd文件解压
- 致远帆软报表文件读取
- 致远帆软报表文件读取-bypass
- 致远帆软报表后台插件文件上传
- 致远帆软报表后台主题文件上传
- 致远M1命令执行

通达已完成:
- 通达任意用户登录-1
- 通达任意用户登录-2
- 通达任意用户登录-3
- 通达任意用户登录-4
- 通达Ispirit文件上传
- 通达ueditor文件上传
- 通达gateway反序列化
- 通达后台附件文件上传

红帆已完成:
- 红帆OA任意文件上传
- 红帆OA任意文件写入

金和已完成:
- 金和OA命令执行
- 金和OA editeprint文件写入
- 金和OA EditMain文件写入 	
- 金和OA saveAsOtherFormatServlet文件上传
- 金和OA OfficeServer文件上传
- 金和OA UploadFileBlock文件上传
- 金和OA jcsUploadServlet文件上传	
- 金和OA UploadFileEditorSave文件上传 	
- 金和OA viewConTemplate 模板注入

金蝶已完成:
- 金蝶云星空反序列化 	
- 金蝶云星空文件上传 	
- 金蝶EAS file文件上传 	
- 金蝶EAS logo文件上传 	
- 金蝶Apusic 文件上传 

广联达已完成:
- 广联达OA GetIMDictionary sql注入
- 广联达OA 任意用户登录
- 广联达OA 用户文件上传
- 广联达OA 后台文件上传

华天动力已完成:
- 华天动力OA ntkoupload 文件上传
- 华天动力OA Servlet文件上传

## 使用说明
直接下载releases版本即可

**使用JDK8启动，命令如下：**

java -javaagent:Exp-Tools-1.2.7-encrypted.jar -jar Exp-Tools-1.2.7-encrypted.jar

![image-20220324174004915](images/Snipaste_2023-03-09_09-19-21.jpg)

## 更新日志

### 2023/1/2

- 新增红帆OA任意文件上传
- 新增华天动力OA任意文件上传

### 2023/2/1

- 新增泛微ecology FileClient 文件上传
- 新增泛微ecology后台流程命令执行
- 默认上传文件修改为json.txt

### 2023/2/28

- 修复通达oa后台附件文件上传一处bug

### 2023/3/1

- 新增YongyouNC反序列化

### 2023/3/17

- 新增Yongyou-U8 AppProxy 文件上传
- 新增用友KSOA Attachment 文件写入
- 新增致远后台模板管理器文件上传
- 修复多个bug

### 2023/4/6

- 新增蓝凌oa后台模板上传
- 新增用友CRM swfupload 文件上传
- 修复cookie 更新
- 优化部分代码
- 修复多个bug

### 2023/4/27
- 新增泛微ecology前台sql注入-2
- 新增红帆OA任意文件写入
- 修复泛微emobile一处bug
- 删除泛微ecology后台皮肤文件上传
- 删除conf文件夹，修改为启动时创建
- 删除cookie提示

### 2023/6/28
- 新增用友畅捷通T+SQL注入
- 新增致远帆软报表文件读取-bypass
- 新增泛微eoffice uploadify上传
- 新增php-framework和java-framework
- 新增nacos任意用户添加
- 新增金蝶云星空反序列化
- 优化部分代码

##  2023/8/8
- 新增用友反序列化-3
- 新增泛微ecology WorkflowServiceXml命令执行
- 新增用友U8 cloud文件上传
- 新增用友NC 文件上传
- 新增帆软报表文件读取-bypass
- 新增帆软报表未授权命令执行
- 新增用友移动管理平台文件上传
- 优化部分代码

## 2023/9/6
- 删除用友畅捷通T+sql注入
- 新增致远M1反序列化
- 新增用友移动管理平台Icon文件上传
- 新增大华、海康、宏景漏洞利用
- 优化部分代码

## 2023/10/11
- 新增蓝凌、用友、万户部分漏洞
- 修复部分漏洞误报
- 优化部分代码

### 2023/11/24
- 新增蓝凌、nacos、用友部分漏洞

### 2023/12/08
- 修复asp上传内容
- 新增部分漏洞

### 2024/02/28
- 新增部分漏洞

### 2024/03/06
- 修改upload方法兼容性
- 增加部分漏洞
- 修复多个漏洞误报
- 修复致远后台表格文件写入漏洞

### 2024/04/07
- 增加部分漏洞

### 2024/04/26
- 增加广联达、畅捷通部分漏洞

### 2024/05/07
- 修复某些漏洞的漏报、误报问题

### 2024/06/01
- 新增部分漏洞

### 2024/06/07
- 修复部分漏洞

## 参考链接
https://github.com/White-hua/Apt_t00ls

https://github.com/xinyu2428/TDOA_RCE

https://github.com/yhy0/ExpDemo-JavaFX

https://github.com/0x727/DropLabTools

https://github.com/xinyu2428/TDOA_RCE

https://github.com/Ghost2097221/YongyouNC-Unserialize-Tools
## 问题建议
目前随着漏洞数量的累加，自己编写、使用的时候发现部分漏洞存在误报、漏报。
请发现bug的师傅及时提交issues或私信我帮助我更好迭代。

## Stargazers over time

[![Stargazers over time](https://starchart.cc/cseroad/Exp-Tools.svg)](https://starchart.cc/cseroad/Exp-Tools)

