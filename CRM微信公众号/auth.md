#登录注册
server=auth

## 发送登录验证码

``` java 
POST /captcha
 ```  
> 请求参数
 <table>
     <tr>
         <th style="width:150px;">属性名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>mobile</td>
         <td>String</td>
         <td>是</td>
         <td>手机号</td>
         <td>-</td>
     </tr>
 </table>    
 
## 发送注册验证码 

``` java 
POST /captcha/register
 ```
   
> 请求参数  
 
     同登录请求  
  

## crm登录
``` java 
POST /crm-login
 ```  
<table>
     <tr>
         <th style="width:150px;">属性名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>mobile</td>
         <td>String</td>
         <td>是</td>
         <td>手机号</td>
         <td>-</td>
     </tr>
     <tr>
         <td>captcha</td>
         <td>String</td>
         <td>是</td>
         <td>验证码</td>
         <td>-</td>
     </tr>
 </table>    
 



## crm注册

``` java 
POST /crm-register
 ``` 
 > 请求参数: 
 <table>
     <tr>
         <th style="width:150px;">参数名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>serverId</td>
         <td>int</td>
         <td>是</td>
         <td>服务器ID</td>
         <td>暂时固定为1</td>
     </tr>
        <tr>
              <td>captcha</td>
              <td>String</td>
              <td>是</td>
              <td>验证码</td>
<td></td>
          </tr>
     <tr>
         <td>client</td>
         <td>object</td>
         <td>是</td>
         <td>客户信息</td>
         <td>见下表</td>
     </tr>
     <tr>
         <td>user</td>
         <td>object</td>
         <td>是</td>
         <td>用户信息</td>
         <td>见下表</td>
     </tr>
     <tr>
         <td>app</td>
         <td>object</td>
         <td>是</td>
         <td>APP信息</td>
         <td>见下表</td>
     </tr>
 </table>
 
 > client客户信息
 
 <table>
     <tr>
         <th style="width:150px;">参数名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>name</td>
         <td>string</td>
         <td>是</td>
         <td>客户名称</td>
         <td>-</td>
     </tr>
     <tr>
         <td>province</td>
         <td>string</td>
         <td>-</td>
         <td>所在省</td>
         <td>-</td>
     </tr>
     <tr>
         <td>city</td>
         <td>string</td>
         <td>-</td>
         <td>所在市</td>
         <td>-</td>
     </tr>
     <tr>
         <td>county</td>
         <td>string</td>
         <td>-</td>
         <td>所在区(县)</td>
         <td>-</td>
     </tr>
     <tr>
         <td>address</td>
         <td>string</td>
         <td>-</td>
         <td>地址</td>
         <td>-</td>
     </tr>
     <tr>
         <td>contact</td>
         <td>string</td>
         <td>-</td>
         <td>联系人</td>
         <td>-</td>
     </tr>
     <tr>
         <td>tel</td>
         <td>string</td>
         <td>-</td>
         <td>联系电话</td>
         <td>-</td>
     </tr>
     <tr>
         <td>remark</td>
         <td>string</td>
         <td>-</td>
         <td>备注</td>
         <td>-</td>
     </tr>
 </table>
 
 > user 用户信息
 
 <table>
     <tr>
         <th style="width:150px;">参数名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>mobile</td>
         <td>string</td>
         <td>是</td>
         <td>手机号</td>
         <td>-</td>
     </tr>
     <tr>
         <td>name</td>
         <td>string</td>
         <td>是</td>
         <td>名称</td>
         <td>-</td>
     </tr>
 </table>
 
 > app APP信息
 
 <table>
     <tr>
         <th style="width:150px;">参数名称</th>
         <th style="width:60px;">类型</th>
         <th style="width:60px;">必填</th>
         <th style="width:200px;">说明</th>
         <th>备注</th>
     </tr>
     <tr>
         <td>setting</td>
         <td>map</td>
         <td>-</td>
         <td>设置项</td>
         <td>见App文档</td>
     </tr>
 </table>