<h1>第5章  静态网站、动态网站及IP域名 </h1>

# 1 静态网页、静态网★★★

- 静态网页”指的是每次调用该网页时，其展示内容“固定不变”，当客户通过浏览器向Web服务器请求网页时，Web服务器将纯粹的HTML文档传送给客户浏览器。
- 纯粹的HTML文档全部由标准的HTML代码组成，最多再加上流行的GIF89A格式的动态图片、Flash动画、JavaScript、VBScript和信息滚动等动画效果。
- 静态网页在客户端运行，一般以 .htm、.html、.shtml、.xml等为后缀。

静态网站

- 所有网页都是由“静态网页”组成的网站称为静态网站
- 没有数据库的支持
- 静态网站可能包含动画和滚动信息

# 2 动态网页、动态网★★★

- 并不是网页上有GIF动画图片、Flash动画或滚动文本就称为动态网页，
- 具有交互性、自动更新和因人而异的特点，存取数据库、有代码在服务器端运行并只有访问时才确定内容的网页称为动态网页。
- 动态网页一般是以.asp、.php和.jsp为后缀的网页文件。
- 有动态网页的网站称为动态网站，动态网站并不是所有网页都是动态网页，大多数网站都是以静态网页和动态网页混合而成的。



| 类型   | 含义                                       | 优点                                       | 缺点                                       |
| ---- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| 静态网页 | 网页内容每次调用固定不变, Web服务器将纯粹的HTML文档传送给客户浏览器   | 设计针对性和灵活性强<br>都有一个固定的URL <br>容易被搜索引擎检索 <br>对应独立的磁盘文件<br>网页设计比较简单<br>存取速度比动态网页快 | 更新内容必须重新制作网页，网站制作和维护工作量大交互性较差<br>缺乏对信息数据的管理、检索和维护<br>静态网页信息发布、维护等需要专业人员 |
| 动态网页 | 具有交互性、自动更新和因人而异的特点，存取数据库、有代码在服务器端运行并只有访问时才确定内容的网页称为动态网页。 | 有GIF动画、Flash动画或滚动文本的网页不是动态网页<br>交互性、自动更新、因时因人而变  需要数据库的支持<br>信息发布、维护等不需要专业人员 <br>非常容易检索、统计和管理维护等  <br>可以实现更多的功能，如用户注册、用户登录等等。 | 很难被搜索<br>设计比较复杂 <br>存取速度比静态网页要慢          |

# 3 动态生成静态网站★

- 为了减轻服务器的负担，减少数据库的访问次数，减小使用资源，提高访问网站的速度，
- 为了SEO
- 动态网页静态化


- - 把访问量很大的动态网页(ASP、JSP、PHP等)批量转换成静态网页，保留动态网页的所有显示内容和格式，

**静态化方法**

- 专门的动态网页转为静态网页的工具软件
- 使用HttpWebRequest请求客户端的方式


- - 获取返回资源，生成[静态页面](http://baike.baidu.com/view/3293095.htm)。一般这样只需要获取网页内容即可，其它资源可放置在服务器上，自动加载。(注：此方法缺点明显，需要大量更改匹配URL，建议慎用)


- 使用现成的[插件](http://baike.baidu.com/view/18979.htm)


- - ISAPI_Rewrite、IIS Rewrite、[Apache](http://baike.baidu.com/subview/28283/5418752.htm) HTTP服务器的[mod_rewrite](http://baike.baidu.com/view/5016366.htm)等，
  - 基于[正则表达式](http://baike.baidu.com/view/94238.htm)解析器开发的重写引擎。


- 利用模板技术


- - 将模板中特殊代码的值替换为从[表单](http://baike.baidu.com/view/296684.htm)或是数据库字段中接受过来的值 生成[HTML文件](http://baike.baidu.com/view/394827.htm)；


- 创建FSO对象


- - ASP中，FSO的意思是File System Object 
    - 将所需的内容动态创建到文件中生成[HTML](http://baike.baidu.com/view/692.htm)页面；


- 使用Server.Transfer转换技术

  - [ASP.NET](http://www.baidu.com/link?url=1eZqLAcgUAc6mohbD9B-zshMpBQUBSAH3eoBw7w--ql5VCgSXrT-OwZhtwXSFUg-zQ79RUhSXS_laLW53rBZXK) 

  - 跨页传递信息

  - 把执行流程从当前的ASPX文件转到同一服务器上的另一个ASPX页面

    ​

    ​


# 4 Web应用程序★

- 一些功能相对独立或完整的动态网页集合称为Web应用程序，


- - 例如计数器、留言本、论坛、聊天室、新闻发布系统和咨询调查系统等都是常见的Web应用程序
  - SPA   single-page application 


- Web应用程序需要在服务器端进行相关处理之后，然后将处理后的信息传递到客户端的浏览器? 

# 5 域名系统DNS

- Internet网上这种层次型名字管理机制叫域名系统。
- 每个域名只对应一个唯一的IP地址。
- 域名表示方法如下所示：


- - 四级域名·三级域名·二级域名·一级域名(顶级域名)


- 域名的解析过程


- - Internet网上的主机之间是通过IP地址来进行通信的 
  - 域名服务器（DNS SERVER )
  - Internet网上，IP地址用于网络间的寻址，即网络之间的数据通信通过IP地址来完成，实现点对点通讯，
  - 而同一物理网络中的数据通信则是通过主机的物理地址（也叫MAC地址）来完成的，局域网通过广播方式进行通信。 
  - 网络层的ARP地址解析协议 
    ![](https://ww1.sinaimg.cn/large/006tNc79jw1fbf3gdmq3sj309r07x3ys.jpg)

    ![](https://ww1.sinaimg.cn/large/006tNc79jw1fbf3kefq1kj303907vglj.jpg)