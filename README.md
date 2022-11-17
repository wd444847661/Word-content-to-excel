# Word-content-to-excel
将Word中的目录，根据标题等级，放入到excel中

例子：

![image](https://user-images.githubusercontent.com/59003864/202407070-7f774314-8acc-4a04-8efe-19c097387e75.png)

使用脚本处理完为：

![image](https://user-images.githubusercontent.com/59003864/202407186-657aea50-dae1-4b3c-a2f8-636ca6b23ec6.png)

具体留不留目录的层级的数字，可以将截取str的那块改掉就可以了

同事之前手动整理很大的文档目录，整了一份出来就要好几个小时，找我来帮忙，先是知乎找到了一个人写的VBA，但是用不了，也很久没回复了，就想着用python写一个。

具体使用的方法：
1. 将word中的目录复制，无格式粘贴到excel的A列中
2. 将excel文件和脚本放到一个新的文件夹中（会自动处理py文件夹中所有的excel文件）
3. 运行脚本即可，处理好的excel命名为原excel名+NEW

注意：
1. 如果想再次运行脚本，一定要把处理好的excel先放到其他地方，要不然会报错（因为格式已经更改好了）
2. 如果复制的目录不是从一级目录开始的，比如直接从2.1开始，会自动在第一行添加测试，作为2.1的一级目录
3. python是个人爱好，写的代码肯定不是最优的，能用就可行
