# VimStock
基于vim命令行的炒股插件

![Alt text](https://github.com/guofh/VimStock/blob/master/VimStock.png)
  
敲代码看盘两不误，窗口随意调整。
  
![Alt text](https://github.com/guofh/VimStock/blob/master/VimStock2.png)

## 安装事项

1. 需要添加vim对python2的支持
2. 需要安装的python包:requests,pandas
3. .VimStock内放置的是一些功能需要的配置文件，如自选股功能。需要将.VimStock目录复制到用户根目录中。

## VimStock的使用命令

1. #### **:Vallstock [关键字] [正倒序] [页码]**  
    
    说明：Vimstock命令为显示所有股票最新信息，并按照[关键字]进行排序。[关键字]有涨跌幅(zdf)，涨速(zs)等。关键字变量为表头的中文首字母缩写，如市盈率为  syl。排序1为正序，0为倒序。例：`Vallstock zdf 1 1` 为显示所有股票按涨跌幅由高向低排序，显示第一页内容。`Vallstock zs 0 2` 为显示所有股票按涨速由低向高排序，显示第二页内容。
    
2. #### **:Vggzjl [关键字] [正倒序] [页码]**  
    
    说明：Vggzjl命令为显示所有股票资金流信息，并按照[关键字]进行排序。[关键字]中比Vallstock增加了包括大单净量，流入，流出，净额等资金流信息。关键字变量为表头的中文首字母缩写。排序1为正序，0为倒序。例：`Vggzjl lrzj 1 1` 为显示所有股票按流入资金排序，显示第一页内容。
    
3. #### **:Vgnzjl [关键字] [正倒序] [页码]**  
    
    说明：Vgnzjl命令为显示概念板块信息包括资金流信息，并按照[关键字]进行排序。[关键字]关键字变量为表头的中文首字母缩写。排序1为正序，0为倒序。例：`Vgnzjl je 1 1` 为显示所有概念板块按净流入资金排序，显示第一页内容。
    
4. #### **:Vhyzjl [关键字] [正倒序] [页码]**  
    
    说明：Vhyzjl命令为显示行业板块信息包括资金流信息，并按照[关键字]进行排序。[关键字]关键字变量为表头的中文首字母缩写。排序1为正序，0为倒序。例：`Vhyzjl zdf 1 1` 为显示所有行业板块按涨跌幅排序，显示第一页内容。
    
4. #### **:Vr**  
    
    说明：Vr命令为刷新当前行情。如果当前开了多个窗口，则所有窗口信息全部刷新为最新的行情。
    
5. #### **:Vrun**  
    
    说明：Vrun命令VimStock默认的一种窗口显示。默认为四个窗口，第一窗口显示涨速排名，第二窗口显示概念板块涨跌幅，第三窗口显示行业板块涨跌幅，第四窗口显示所有股票信息按涨幅排序。用户也可以根据平时自己的习惯设置自己的界面信息。
     
6. #### **:Vgo**
    
    说明：Vgo命令为显示板块内所有股票，当光标放在相应板块上并敲:Vgo，则显示该板块内的所有股票。

7. #### **:Vmystock**
    
    说明：Vmystock命令为显示自选股信息，自选股配置文件在用户根目录下的.VimStock.mystock中，可以选择手动修改文件也可以通过命令添加、删除自选股列表。

8. #### **:Vadd [股票代码]**
    
    说明：Vadd命令为添加自选股到自选股列表中，[股票代码]为六位数字。例：Vadd 000002 代表添加000002到自选股列表中，通过Vmystock查看自选股信息。

9. #### **:Vdel [股票代码]**
    
    说明：Vdel命令为从自选股列表中删除自选股，[股票代码]为六位数字。例：Vdel 000002 代表将000002从自选股列表中删除，通过Vmystock查看自选股信息。


## 快捷键使用

vimrc文件中定义了一些常用的快捷键，如查看涨幅榜，涨速榜，板块，个股等常用的看盘功能。可以将vimrc中的内容复制到本地的.vimrc配置文件中。也可以根据自己平时的使用习惯自行进行配置。

## 联系方式

微博：@一口大黑郭

微信：g635852898

邮箱：heiguo88@gmail.com
  

