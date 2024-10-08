# NKU-CSSE0027-软件安全
## 提供软件安全实验报告Lab1-Lab13，以及课程大作业——论文阅读

### Lab1 IDE反汇编实验

根据第二章示例2-1，在XP环境下进行VC6反汇编调试，熟悉函数调用、栈帧切换、`CALL`和`RET`指令等汇编语言实现，将`call`语句执行过程中的`EIP`变化、`ESP`、`EBP`变化等状态进行记录，解释变化的主要原因。 
 
### Lab2 OLLYDBG软件破解

​1.请在XP VC6生成课本第三章软件破解的案例(DEBUG模式，示例3-1) 。进而，使用OllyDBG进行单步调试，获取`verifyPWD`函数对应`flag==0`的汇编代码，并对这些汇编代码进行解释。

​2.对生成的DEBUG程序进行破解，复现课本上提供的两种破解方法。

### Lab3 堆溢出Dword Shoot攻击实验

以第四章示例4-4代码为准，在VC IDE中进行调试，观察堆管理结构，记录Unlink节点时的双向空闲链表的状态变化，了解堆溢出漏洞下的`Dword Shoot`攻击。
 
### Lab4 格式化字符串漏洞

​以第四章示例4-7代码，完成任意地址的数据获取，观察Release模式和Debug模式的差异，并进行总结。

实验代码如下所示：

```c
#include <stdio.h>
int main(int argc, char *argv[])
{
    char str[200];
    fgets(str,200,stdin);
    printf(str);
    return 0;
}

```

### Lab5 Shellcode编写及编码

复现第五章实验三，并将产生的编码后的shellcode在示例5-1中进行验证，阐述shellcode编码的原理、shellcode提取的思想。

### Lab6 API函数自搜索

复现第五章实验七，基于示例5-11，完成API函数自搜索的实验，将生成的exe程序，复制到windows 10操作系统里验证是否成功。

### Lab7 AFL模糊测试

根据课本$7.4.5$章节，复现$AFL$在$Kali$下的安装、应用，查阅资料理解覆盖引导和文件变异的概念和含义。

### Lab8 程序插桩及Hook实验

复现实验一，基于$WindowsMyPinTool$或在$Kali$中复现$malloctrace$这个$PinTool$，理解$Pin$插桩工具的核心步骤和相关$API$，关注$malloc$和$free$​函数的输入输出信息。

### Lab9 Angr应用实例

根据课本8.4.3章节，复现$sym-write$示例的两种$angr$求解方法，并就如何使用$angr$以及怎么解决一些实际问题做一些探讨。
 
### Lab10 WEB开发实践

复现课本第十章的实验三($10.3.5$节):利用$php$，编写简单的数据库插入、查询和删除操作的示例。基于课本的完整的例子，进一步了解$WEB$开发的细节。

### Lab11 跨站脚本攻击

复现课本第十一章实验三，通过$img$和$script$两类方式实现跨站脚本攻击，撰写实验报告。有能力者可以自己撰写更安全的过滤程序。

### Lab12 SQL盲注

基于$DVWA$里的$SQL$盲注案例，实施手工盲注，参考课本，撰写实验报告。

### Lab13 复现反序列化漏洞

复现$12.2.3$中的反序列化漏洞，并执行其他的系统命令。

### 论文阅读
#### 论文题目
DynSQL: Stateful Fuzzing for Database Management Systems with Complex and Valid SQL Query Generation

提供论文翻译，答辩ppt等内容


