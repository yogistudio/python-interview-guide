
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [写在前面（扯皮）](#写在前面扯皮)
  - [公司选择](#公司选择)
  - [简历投递](#简历投递)
  - [面试策略](#面试策略)
  - [面试总结](#面试总结)
- [技术部分](#技术部分)
  - [语言特性篇](#语言特性篇)
    - [Python2和Python3的区别](#python2和python3的区别)
    - [闭包](#闭包)
    - [装饰器(面向切面编程AOP)](#装饰器httpsfoofishnetpython-decoratorhtml面向切面编程aop)
    - [协程](#协程httpswwwcnblogscomzhaofp7631851html)
    - [Python垃圾回收机制(GC)](#python垃圾回收机制gchttpsmpweixinqqcoms__bizmzu1nzuzmziynwmid2247483786idx1snd9e490ff84da3140483595399ac9cc95chksmfc3510cecb4299d8230be48a50ac125b7dec379a654b50de0f28d1510879eb82b5ff5b0c1033mpshare1scene1srcidsharer_sharetime1565661971268sharer_shareidd8d88a642b42a12a54cd09298c974b8crd)
    - [全局解释锁 GIL](#全局解释锁-gilhttpswwwlmlphpcomuser6793articleitem349814)
    - [Python的参数传递](#python的参数传递)
    - [Python 深拷贝和浅拷贝](#python-深拷贝和浅拷贝)
    - [鸭子类型](#鸭子类型)
    - [猴子补丁](#猴子补丁)
    - [Python中的作用域](#python中的作用域)
    - [lambda函数](#lambda函数)
    - [Python函数式编程](#python函数式编程)
    - [迭代器和生成器](#迭代器和生成器)
    - [Python自省](#python自省)
    - [Python 面对对象编程](#python-面对对象编程)
      - [封装](#封装)
      - [继承](#继承)
      - [多态](#多态)
      - [类成员](#类成员)
      - [类成员的修饰符](#类成员的修饰符)
      - [类的特殊成员](#类的特殊成员)
    - [Python 中的元编程和反射](#python-中的元编程和反射)
    - [谈谈对 Python 和其他语言的区别](#谈谈对-python-和其他语言的区别)
    - [设计模式](#设计模式)
      - [单例模式](#单例模式)
      - [工厂模式](#工厂模式httpssegmentfaultcoma1190000013053013)
  - [数据结构与算法篇](#数据结构与算法篇)
    - [排序算法](#排序算法)
    - [链表算法](#链表算法httpsmpweixinqqcoms__bizmzuynjqxnjyymgmid2247484830idx1sn9d24fc787da4b49b82ac01c7f8de257bchksmfa0e6a1fcd79e309a2e7f3e09ec9913a55f1c077287c907f13528578b7785831a2effb3104e0scene21wechat_redirect)
    - [栈和队列算法](#栈和队列算法)
    - [二叉树算法](#二叉树算法)
    - [字符串算法](#字符串算法)
    - [哈希算法](#哈希算法)
    - [Backtracking回溯法(又称DFS,递归)全解](#backtracking回溯法又称dfs递归全解httpssegmentfaultcoma1190000006121957)
    - [2018 秋招笔试面经](#2018-秋招笔试面经httpsgithubcomimhuayalgorithm_interview_notes-chinesetreemasterd-笔试面经一面)
  - [操作系统篇](#操作系统篇)
    - [进程与线程区别](#进程与线程区别)
    - [谈谈多线程并发](#谈谈多线程并发)
    - [线程同步方式](#线程同步方式httpsblogcsdnnetebowtangarticledetails29905309)
    - [线程有几种状态](#线程有几种状态)
    - [分页机制](#分页机制)
    - [分页和分段有什么区别（内存管理）](#分页和分段有什么区别内存管理)
    - [什么是虚拟内存？](#什么是虚拟内存)
    - [颠簸(抖动)](#颠簸抖动)
    - [进程调度算法](#进程调度算法)
    - [进程同步机制](#进程同步机制httpsblogcsdnnetwangrunminarticledetails7941592)
    - [进程的状态](#进程的状态)
    - [进程间通信方式](#进程间通信方式)
    - [僵尸进程和孤儿进程](#僵尸进程和孤儿进程httpswwwcnblogscomankerp3271773html3777880)
    - [fork进程时的操作](#fork进程时的操作)
    - [Socket编程](#socket编程)
    - [Linux的五种IO模型](#linux的五种io模型)
    - [IO 多路复用模型](#io-多路复用模型)
      - [select](#select)
      - [poll](#poll)
      - [epoll](#epoll)
      - [select、poll、epoll区别](#select-poll-epoll区别)
    - [谈谈死锁](#谈谈死锁)
      - [死锁的概念](#死锁的概念)
      - [死锁产生的原因](#死锁产生的原因)
      - [死锁产生的四个必要条件](#死锁产生的四个必要条件)
      - [解决死锁的基本方法](#解决死锁的基本方法)
  - [计算机网络篇](#计算机网络篇)
    - [从URL输入到页面展现到底发生什么？](#从url输入到页面展现到底发生什么httpsmpweixinqqcoms__bizmzg5oda5ntm1mwmid2247483803idx1sn460597ae3bd3ec10ad3426b7db605074chksmc066800df711091b2b6e005a922fff4a6a8e4b7930928a1c60fc0ac657c3ea5061cf1b51563dmpshare1scene1srcidrd)
    - [ARP 协议工作原理](#arp-协议工作原理)
    - [TCP 三次握手](#tcp-三次握手)
    - [TCP 四次挥手](#tcp-四次挥手)
    - [TCP 怎样保证可靠性](#tcp-怎样保证可靠性)
    - [TCP的流量控制和拥塞控制](#tcp的流量控制和拥塞控制httpsblogcsdnnetyechaodechuntianarticledetails25429143)
    - [TCP 与 UDP 的区别](#tcp-与-udp-的区别)
    - [HTTP协议](#http协议)
      - [HTTP 和 HTTPS 的区别](#http-和-https-的区别)
      - [URL详解](#url详解)
    - [HTTP 常见方法（GET/PUT）](#http-常见方法getput)
      - [安全性和幂等性](#安全性和幂等性)
      - [GET和POST 区别](#get和post-区别)
    - [常见 HTTP 状态码](#常见-http-状态码)
    - [HTTP 长连接与短连接](#http-长连接与短连接)
      - [长连接](#长连接)
      - [短连接](#短连接)
    - [cookie 和 session 的区别](#cookie-和-session-的区别)
    - [JSON Web Token](#json-web-token)
    - [IP 地址的分类](#ip-地址的分类)
    - [OSI七层参考模型](#osi七层参考模型)
  - [数据库篇](#数据库篇)
    - [MySQL 基础问题](#mysql-基础问题)
    - [MySQL的innodb引擎是如何实现MVCC](#mysql的innodb引擎是如何实现mvcc)
    - [事务](#事务)
    - [如何解决高并发场景下的插入重复](#如何解决高并发场景下的插入重复)
    - [乐观锁和悲观锁](#乐观锁和悲观锁)
    - [InnoDB 和 MyISAM](#innodb-和-myisam)
    - [B树和B+树](#b树和b树)
    - [MySQL 索引](#mysql-索引)
    - [聚集索引和非聚集索引](#聚集索引和非聚集索引)
    - [排查慢查询](#排查慢查询)
    - [内存缓存（Redis和Memcached)](#内存缓存redis和memcached)
    - [Redis的使用](#redis的使用)
- [最佳实践](#最佳实践)
  - [编码规范](#编码规范)
  - [正确的流程开发](#正确的流程开发httpswwwzhihucomquestion300762444answer529335326appzhihuliteutm_sourcezhihusignmtu2mda2nzmzmzyznwutm_mediumsocialutm_oi758575502888824800invite_code7jv2ek)
  - [单元测试](#单元测试)
  - [CI/CD工具篇](#cicd工具篇)
  - [Git 命令应急手册](#git-命令应急手册httpsmpweixinqqcoms__bizmzaxotcxntiwnqmid2457914802idx1sna8d2cb9b626da84d94d8b2ebd9e85c24chksm8cb6a858bbc1214e62feff7028ce6b6e942556e42d5f2edbedb8216a03c0b54fa52ce378256empshare1scene1srcidrd)
  - [Docker 篇](#docker-篇)
- [Web 扩展](#web-扩展)
  - [Web安全篇](#web安全篇)
    - [DDos 攻击](#ddos-攻击)
    - [XSS 攻击](#xss-攻击)
    - [SQL 注入攻击](#sql-注入攻击)
    - [加密](#加密)
  - [Nginx篇](#nginx篇)
  - [Vue篇](#vue篇)
  - [Django篇](#django篇)
    - [WSGI、uwsgi、uWSGI 区别](#wsgi-uwsgi-uwsgi-区别)
  - [正则表达式篇](#正则表达式篇)
- [其他](#其他)

<!-- /code_chunk_output -->

### 写在前面（扯皮）
#### 公司选择
* 写 Python 可供选择的公司本来不多，但中小公司还是很多，但找到小而美的就很少，说说个人心中“小而美”的标准：
  - 团队互补能力强，虽小但是能够cover的业务能力广；
  - 有明锐的嗅觉和创新能力，并且能够专注于某个行业领域或者发展方向；
  - 快或缓，有清晰的发展规划;
  - 他山之石可以攻玉，不重复造轮子。
  - 最后一条，商业模式应该在很小的规模下就能验证。（好像是雷布斯说的，逃）
  - 多抓鱼，长亭科技，待补充。。。
* 大两级的学长说过，找工作很重要，更重要的是找准一个行业，看有哪些公司(采用波特五力模型)在做什么，处于产业链什么位置😃
#### 简历投递
* 岗位对上三条及以上就可以投了，要不要实习都可以尝试一下😂
* 自己设计一张简历投递状态记录表，投递中->笔试->一面->二面->hr面，面试结果，被拒绝/get offer
* 找正确的投递渠道，拉勾上找到前几页满足岗位要求的公司，然后去官网，一般都有加入我们，没有的就不用考虑啦(官网连这些基本都做不到，还招啥人，可以看看一面数据，不光有，连招过的实习生都有展示)，当然还有没来得及建官网的😂，不想放过的话，去V2EX、知乎搜关键字会发现惊喜。
* thank you letter!面试结束后发感谢信！
#### 面试策略
* 项目回答
  - 任何一个公司，任何一个面试，都一定会涉及到你作为一个工程师最最核心的价值和能力，就是你的经验，具体来说就是你做过的项目。这块是面试准备时的重中之重，应该作为最高优先级来对待。有很多同学，做的项目其实挺不错，但是平时疏于总结，面试前也不准备，结果面试时支支吾吾，半天答不上来，白白浪费面试机会。
  - 比如一个非常典型的项目经验的面试考察情景如下：面试官反复的追问项目的各个地方的技术实现细节，就想看看有没有哪个地方是有一定的技术难度的，可以体现出这个候选人的一些项目上的亮点。但是呢，候选人说来说去，总是从业务的角度去说，就说有哪些子系统组成，分别是干什么的，如何交互的，看来看去都是系统业务的东西，就是没看到什么有技术含量的东西在项目里体现出来了。
  - 在面试时，你在阐述项目经验的时候，可以让面试官看到你在里面有更多的技术架构的设计，考虑到了解决更多的技术问题，那么自然你的面试表现就会更好，就更加容易会拿到更好的offer了。
  -  项目的短期突击应该如何进行，才能尽可能的让我们的项目显得更加吸引人。我估计可能更多的同学需要这方面的技巧。自己至少应该反复思考，你目前负责的系统应该引入什么样的技术架构，采用何种技术方案，才能抗住各种冲击。突击准备，你肯定没有大把时间来付诸实践，但是你一定要自己思考，同时百度一下国内大型互联网公司的技术架构，他们使用了哪些高大上的技术，对于某个技术难点采用了什么技术方案。然后在面试的时候，可以对面试官阐述一下你对这个项目一些问题的思考，以及技术方案、架构如何来设计，这样设计可以解决什么技术问题，有没有更好的方案选择。
* 投递顺序
  - 第一阶段练手：当你觉得自己充分的准备好了面试之后，你应该先找几个感觉对自己会有一定技术挑战的公司，但是并不是自己特别意向想要去的公司去投递简历面试一下。在这个阶段，十有八九会暴露出来你很多的问题。对于很多人来说，别看可能是去一些中小型的互联网公司去面试，但是其实里面也有一些技术不错的面试官，只要面试官的技术实力比你强，那么在面试的过程中，一定会问到你一些问题，是你之前没注意以及没准备好的。此时你很可能会发现，刚开始面试的头三四家公司，每家公司聊的都不太顺畅，每家公司总有那么几个问题没回答好，然后都没拿到offer。但是这个阶段的好处是，你发现了自己很多薄弱环节，这个时候你应该尽快通过上网查资料的方式填补好自己对一些薄弱问题的弱项。然后迅速总结，内化为自己的语言，并且能落地到纸上画图实现。这样，下次再问到相同问题的时候，可以回答的更好。基本上按照之前很多同学的情况来说，大概第一个阶段就是持续个三家到五家公司那样子，但是这个期间你会瞬间发现自己很多的问题，然后短时间内通过查阅资料的方式就可以尽快弥补好自己没准备好的一些地方
  - 第二个阶段冲刺：经过了第一个阶段的被虐之后，每个人的面试能力都会加强很多，而且找到了一些面试的感觉，对面试的节奏、对答都有了更好的把控。这个时候第二个阶段，就可以尝试去冲刺一下阿里、美团、滴滴等国内的一些大厂了。在这个阶段里，你需要全力以赴去面试，如果你准备的很充分，经过了第一阶段的打磨提升了面试能力和经验，而且本身的一些学历、过往公司履历相对较好，同时你的一些软素质比如说学习能力、表达能力、沟通能力都比较好，那么在这个阶段相对就会有更大的把握拿到大厂的offer了。但是如果冲刺了一些大厂之后，感觉还是有一定的差距导致没拿到大厂的offer呢？其实这也是很正常的一个现象，因为毕竟大厂的面试官问的问题可能会更难，让你更加难以承受，可能会暴露出来你更多的问题。在面大厂的过程中暴露出来的问题，很多时候就不是准备充分与否的问题了，而是可能暴露出来你的技术能力和知识体系的欠缺，很多东西可能你根本就不会。这对你来说是好事情，因为你通过面试大厂，瞬间会明白自己跟大厂之间的技术差距。这个时候有些技术能力跟大厂欠缺很大的同学一下子会被极大的打击自己的自信心，建议大家暂停一下面试的过程。这时，你完全可以将面大厂过程暴露出来的自己的技术能力的欠缺记录一个清单，然后有针对性的找一些技术资料来对这些不足之处进行学习和准备，尽可能的弥补自己的欠缺。
  - 第三个阶段收尾：假如说你的面试进行到了这个阶段，那么很不好意思，说明几个你最心仪的大厂没能进去。不过也没关系，这个时候如果你针对自己的技术短板进行突击学习之后，相信你的技术能力又会有一个成长和提高。此时你就应该针对你的跳槽进行收尾了，这个时候你可以投递一些中大型互联网公司的职位，同时再加上一些比较好的独角兽企业的职位，或者是一些你感觉技术氛围比较好的中小型互联网公司的职位。从笔者指导过的一些同学来看，你的面试能力积累到这个程度，基本上拿下一些offer是已经没问题了，你面试的时候都会比较游刃有余了。然后接着就可以在收获的几个比较好的offer里选择一个各方面最适合自己的offer。
#### 面试总结
* 总结起来，面试是一场持久战，要软硬兼备。硬性条件：面试官考察候选人的时候主要是从技术广度、技术深度、基础功底、系统设计、项目经验几个角度来进行的，软性条件：表达交流能力和运气。
### 技术部分
* 真正有用的部分，哈哈😄
#### 语言特性篇
* 主要参考：[《流畅的Python》](https://book.douban.com/subject/27028517/)
##### Python2和Python3的区别
##### 闭包
* 闭包指延伸(延伸的意思是seriers在average函数用，但在average_nums中定义的)了作用域的函数，访问定义体之外定义的非全局变量。创建一个闭包必须满足以下几点:
    - 必须有一个内嵌函数
    - 内嵌函数必须引用外部函数中的变量
    - 外部函数的返回值必须是内嵌函数
```python
def average_num():
    series=[]
    def average(num):
        # series自由变量,未在本地作用域绑定
        series.append(num)
        return sum(series)/len(series)
    return average
aver=average_num()
```
* nonlocal 关键字将变量count，total 手动标记为自由变量
```python
def average_num():
    count=0
    total=0
    def average(num):
        nonlocal total,count
        total+=num
        count+=1
        return total/count
    return average
aver=average_num()
print(aver(10))
```
* 顺便提下 global 关键字，Python 默认函数定义体中赋值的变量是局部变量，所以要在函数中使用全局变量，须用global声明。(下面这句去掉global就会报错，`local variable 'b' referenced before assignment`)
```python
b=9
def test(a):
    print(a)
    global b
    print(b)
    b=6
test(3)
```
##### [装饰器](https://foofish.net/python-decorator.html)(面向切面编程AOP)
* 闭包的一个重要应用就是装饰器，函数装饰器在导入模块时立即执行，被装饰的函数只在明确调用时执行。装饰器采用语法糖，使用方便，既可以自定义在装饰器中指定日志级别，也可以使用官方提供的预激协程装饰器等等。
``` python
# 手动实现一个带参数的装饰器
def use_arg(argument):
    def decorate(fun):
        def wrapper(*args,**kwargs):
            print('%s is running'%fun.__name__)
            print('传入的参数 %s'%argument)
            return fun()  
        return wrapper
    return decorate
@use_arg('hahhaa')
def demo():
    pass
demo()
```
##### [协程](https://www.cnblogs.com/zhaof/p/7631851.html)
* 协程调用细节：实际上next()和send()在一定意义上作用是相似的，区别是send()可以传递yield表达式的值进去，而next()不能传递特定的值，只能传递None进去。因此，我们可以看做c.next() 和 c.send(None) 作用是一样的。第一次调用时，请使用next()语句或是send(None)，不能使用send发送一个非None的值，否则会出错的，因为没有Python yield语句来接收这个值。
* send执行的顺序。n1 = yield r这句话是从右往左执行的。当第一次send（None）时，启动生成器，从生成器函数的第一行代码开始执行，直到第一次执行完yield后，跳出生成器函数。这个过程中，n1一直没有定义。运行到send（1）时，进入生成器函数，此时，将yield r看做一个整体，赋值给它并且传回。此时即相当于把1赋值给n1，但是并不执行yield部分。下面继续从yield的下一语句继续执行，然后重新运行到yield语句，执行后，跳出生成器函数。即send和next相比，只是开始多了一次赋值的动作，其他运行流程是相同的。
```python
def consumer():
    r = 'hello'
    while True:
        n1=yield r  #这里的等式右边相当于一个整体，接受回传值
        if not n1:
            return
        print('[CONSUMER] Consuming %s...' % n1)
        r='%d00 OK' % n1
c = consumer()
c.__next__()
n=0
while n<3:
    n=n+1
    r1=c.send(n)
    print('[PRODUCER] Consumer return: %s' % r1)
c.close()
```
* 预激装饰器，使用协程之前必须预激，为了避免忘记，可以在协程上使用一个特殊的装饰器。
```python
from functools import wraps
def corountine(func):
    @wraps(func)                      
    # functools.wraps 则可以将原函数对象的指定属性复制给包装函数对象, 默认有 __module__、__name__、__doc__,或者通过参数选择
    def primer(*args, **kwargs):       # 把被装饰的生成器函数替换成这里的 primer 函数；调用 primer 函数时，返回预激后的生成器
        gen = func(*args, **kwargs)    # 调用被装饰的函数，获取生成器对象。
        next(gen)                      # 预激生成器
        return gen                     # 返回生成器
    return primer
    
@corountine               # 预激装饰器
def coro_average():
    total = 0.0
    count = 0
    average = None
    while 1:
        term = yield average
        total += term
        count += 1
        average = total/count
coro3 = coro_average()
print (coro3.send(5))
print (coro3.send(7))
print (coro3.send(10))
coro3.close()
````
##### [Python垃圾回收机制(GC)](https://mp.weixin.qq.com/s?__biz=MzU1NzUzMzIyNw==&mid=2247483786&idx=1&sn=d9e490ff84da3140483595399ac9cc95&chksm=fc3510cecb4299d8230be48a50ac125b7dec379a654b50de0f28d1510879eb82b5ff5b0c1033&mpshare=1&scene=1&srcid=&sharer_sharetime=1565661971268&sharer_shareid=d8d88a642b42a12a54cd09298c974b8c#rd)
* 引用计数
* 标记-清除机制
* 分代回收
##### [全局解释锁 GIL](https://www.lmlphp.com/user/6793/article/item/349814/)
* GIL是一个防止多线程并发执行机器码的Mutex：cpython解释器的内存管理不是线程安全的，保护多线程情况下对python对象的访问，cpython使用简单的锁机制避免多个线程同时执行字节码。
* 缺陷 ：限制程序的多核执行，同一时间只能有一个线程执行字节码，CPU密集型程序（大量时间花在计算上）难以利用多核优势；但是IO期间会释放GIL，对IO密集型程序(大量时间花在网络传输上，资源调度)影响小。
* 规避影响策略：CPU密集型使用多进程+进程池，IO密集型采用多线程/协程的策略；cython扩展（将python转换为c代码）
*  GIL释放：Python会计算当前已执行的微代码数量，达到一定阈值后强制释放GIL；系统分配的时间片用完释放；IO操作时释放。
* 一个操作如果是一个字节码指令可以完成就是原子的，原子操作是可以保证线程安全的，有了GIL之后仍然要关注线程安全，必要时候需人为加锁。
```python
import threading
lock=threading.Lock()
n=[0]
def demo():
    #with lock:
    n[0]=n[0]+1
threads=[]
for i in range(5000):
    t=threading.Thread(target=demo)
    threads.append(t)
for t in threads:
    t.start()
print(n)
```
* 剖析程序性能：内置profile/cprofile工具，使用pyflame(uber开源)工具分析web应用。
##### Python的参数传递
* args and *kwargs
##### Python 深拷贝和浅拷贝
##### 鸭子类型
##### 猴子补丁
##### Python中的作用域
##### lambda函数
##### Python函数式编程
##### 迭代器和生成器
* 主要参考
    - [Python中的可迭代对象、迭代器和生成器的异同点](https://blog.csdn.net/SL_World/article/details/86507872)
##### Python自省
##### Python 面对对象编程
###### 封装
* 将内容封装到某处
* 从某处调用被封装的内容
```python
class Person:
    def __init__(self,name,age):
        self.name=name
        self.age=age

# 初始化一个实例时调用__init__方法
tim=Person('Tim',18)
# 将Bob,16分布封装到bob的name和age属性中
bob=Person('Bob',16)
```
###### 继承
* 对于面向对象的继承来说，其实就是将多个类共有的方法提取到父类中，子类仅需继承父类而不必一一实现每个方法。Python的类如果继承了多个类，那么其寻找方法的方式（即MRO,method resolution order (方法解析顺序)，在上述查找过程中，一旦找到，则寻找过程立即中断，便不会再继续找了）有两种，可以分别粗略理解为：深度优先和广度优先。具体实现细节可以看这篇[python多重继承C3算法](https://blog.csdn.net/fmblzf/article/details/52512145)
    * 当类是经典类时，多继承情况下，会按照深度优先方式查找，Python 2.x中默认都是经典类，只有显式继承了object才是新式类。
    * 当类是新式类时，多继承情况下，会按照广度优先方式查找Python 3.x中默认都是新式类，不必显式的继承object。
* 继承中super的调用顺序是与MRO-C3的类方法查找顺序一样的，super作用如下：
    - 如果子类继承父类不做初始化，那么会自动继承父类属性。
    - 如果子类继承父类做了初始化，且不调用super初始化父类构造函数，那么子类不会自动继承父类的属性。
    - 如果子类继承父类做了初始化，且调用了super初始化了父类的构造函数，那么子类也会继承父类的属性。
```python
class A:
    def __init__(self):
        print('A')
class B(A):
    def __init__(self):
        print('B')
        super().__init__()
class C(A):
    def __init__(self):
        print('C')
        super().__init__()
class D(B, C):
    def __init__(self):
        print('D')
        super().__init__()
```
###### 多态
* Pyhon不支持多态并且也用不到多态，多态的概念是应用于Java和C#这一类强类型语言中，而Python崇尚“鸭子类型”。
###### 类成员
![leichengyuan.png](https://i.loli.net/2019/08/16/i4GtE972ScAjQhJ.png)
* 字段
	* 静态字段在内存中只保存一份
	* 普通字段在每个实例对象中都要保存一份
	* 应用场景： 通过类创建实例对象时，如果每个实例对象都具有相同的字段，那么就使用静态字段
```python
class Province:
    # 静态字段
    country = 'China' 
    def __init__(self,name):
        # 普通字段
        self.name = name
obj1 =Province('BeiJing')
print(obj1.name)
print(Province.country)
```
* 方法
    - 普通实例方法：由实例对象调用；至少一个self参数；执行普通方法时，自动将调用该方法的实例对象赋值给self；
    - 类方法：由类调用；至少一个cls参数；执行类方法时，自动将调用该方法的类复制给cls；
    - 静态方法：由类调用；无默认参数；
```python
class Foo:
    def __init__(self,name):
        self.name =name
    # 定义普通实例方法,至少一个self参数
    def ord_func(self):
        print(self.name)
    # 定义类方法，至少一个cls参数
    @classmethod
    def class_func(cls):
        print('类方法')
    # 定义静态方法，无默认参数
    @staticmethod
    def static_fun(): 
        print('静态方法')
f = Foo('ord_func')
f.ord_func()
Foo.class_func()
Foo.static_fun()
```
* 属性
    - 定义时，在普通方法的基础上添加@property装饰器，属性仅有一个self参数，调用时无需括号。@property装饰器可以实现其他语言所拥有的getter，setter和deleter的功能（例如实现获取，设置，删除隐藏的属性）；通过@property装饰器可以对属性的取值和赋值加以控制,提高代码的稳定性。
```python
class Goods:
    # 查看属性值 
    @property       
    def price(self):   
        print('@property')
    # 修改、设置属性
    @price.setter                                         
    def price(self, value):       
        print('@price.setter')
    # 删除属性
    @price.deleter   
    def price(self):      
       print('@price.deleter')                             
obj = Goods()
# 自动执行 @property 修饰的 price 方法，并获取方法的返回值 
obj.price
# 自动执行 @price.setter 修饰的 price 方法，并将2000赋值给方法的参数              
obj.price = 2000 
# 自动执行 @price.deleter 修饰的 price 方法  
del obj.price     
```
###### 类成员的修饰符
* _xxx 表示这是一个保护成员（属性或者方法），它不能用from module import * 导入，其他方面和公有一样访问；
* __xxx 这表示这是一个私有成员，它无法直接像公有成员一样随便访问，但可以通过`实例对象名._类名__xxx`这样的方式可以访问；
* __xxx__表示这是一个特殊成员，用来区别其他用户自定义的命名以防冲突，就是例如`__init__()、 __del__()`  这些特殊方法
###### 类的特殊成员
![魔法函数.png](https://i.loli.net/2019/08/16/aeglES6LYfQIz3U.png)
1. __doc __输出类的描述信息
2. __module __输出当前操作对象所在模块
3. __class __输出当前操作对象的类
4. __init __构造方法，通过类创建实例对象时，自动触发执行
5. __del __析构方法，当对象在内存中被释放时，自动触发执行，此方法一般无须定义，因为Python是一门高级语言，程序员在使用时无需关心内存的分配和释放，因为此工作都是交给Python解释器来执行，所以，析构函数的调用是由解释器在进行垃圾回收时自动触发执行的。
6. __call__对象后面加括号，触发执行，构造方法的执行是由创建对象触发的，即：对象 = 类名() ；而对于 __call__ 方法的执行是由对象后加括号触发的，即：对象() 或者 类()()
```python
class Foo:
    def __init__(self):
        pass
    def __call__(self,*args,**kwargs):
        print('__call__')
# 执行 __init__
obj6 = Foo() 
# 执行 __call__
obj6()
```
7. __dict__类或对象中的所有成员
```python
class Province:
    country = 'China'
    def __init__(self, name, count):
        self.name = name
        self.count = count
    def func(self, *args, **kwargs):
        print('func')
# 获取类的成员，即：静态字段、方法、
# 输出：{'__module__': '__main__', 'country': 'China', '__init__': <function Province.__init__ at 0x00000264B20F1E18>, 
# 'func': <function Province.func at 0x00000264B4638D08>, '__dict__': <attribute '__dict__' of 'Province' objects>, 
# '__weakref__': <attribute '__weakref__' of 'Province' objects>, '__doc__': None}
print(Province.__dict__)
# 输出：{'name': 'HeBei', 'count': 1000}
obj1 = Province('HeBei',1000)
print(obj1.__dict__)
obj2 = Province('HeNan', 3)
# 输出：{'name': 'HeNan', 'count': 3}
print(obj2.__dict__)
```
8. __str__如果一个类中定义了__str__方法，那么在打印对象时，默认输出该方法的返回值。
```python
class Foo:
    def __init__(self):
        pass
    def __str__(self):
        return '__str__'
obj=Foo()
print(obj)
```
9. `__getitem__、__setitem__、__delitem__`用于索引操作，如字典。以上分别表示获取、设置、删除数据。
9. `__getslice__、__setslice__、__delslice__`该三个方法用于分片操作，如列表。
10. __iter__用于迭代器，之所以列表、字典、元组可以进行for循环。
11. `__new__和__init__`
`__new__`是一个静态方法，而`__init__`是一个实例方法，`__new__`方法会返回一个创建的实例，而`__init__`什么都不返回，当创建一个新实例时调用`__new__`，初始化一个实例时用`__init__`。
##### Python 中的元编程和反射
##### 谈谈对 Python 和其他语言的区别
##### 设计模式
###### 单例模式
1. 使用new方法
2. 共享属性
3. 装饰器版本
4. import方法
###### [工厂模式](https://segmentfault.com/a/1190000013053013)
#### 数据结构与算法篇
* 主要参考
  - [problem-solving-with-algorithms-and-data-structure-using-python 中文版](https://facert.gitbooks.io/python-data-structure-cn/)
  - 五分钟算法公众号
* 数据结构都有啥，[戳这里](https://mp.weixin.qq.com/s?__biz=MzUyNjQxNjYyMg==&mid=2247485737&idx=1&sn=82fa3f103ef485a8ce28c5e1c5e012ea&chksm=fa0e66a8cd79efbeb88cb175fcc21a71964d975a47d3c87a8335506466937e811a066f8a1889&mpshare=1&scene=1&srcid=&sharer_sharetime=1564711256674&sharer_shareid=d8d88a642b42a12a54cd09298c974b8c#rd)就行
##### 排序算法
* 快排，堆排，归并排序详细原理参考这篇[这或许是东半球分析十大排序算法最好的一篇文章](https://mp.weixin.qq.com/s?__biz=MzUyNjQxNjYyMg==&mid=2247485556&idx=1&sn=344738dd74b211e091f8f3477bdf91ee&chksm=fa0e67f5cd79eee3139d4667f3b94fa9618067efc45a797b69b41105a7f313654d0e86949607&scene=21#wechat_redirect)，下面我将用 Python 快速实现出来。话不多说，Show me code!
* 冒泡排序
```python
def bubble_sort(alist):
    for i in range(len(alist)-1):
        for j in range(len(alist)-1-i):
            if alist[j]>alist[j+1]:
                alist[j],alist[j+1]=alist[j+1],alist[j]
alist=[54,26,93,17,77,31,44,55,20]
bubble_sort(alist)
print(alist)
```
* 选择排序
```python
def select_sort(alist):
    for i in range(len(alist)-1):
        min_index=i
        for j in range(i+1,len(alist)):
            if alist[j]<alist[min_index]:
                min_index=j
        if i!=min_index:
            alist[i],alist[min_index]=alist[min_index],alist[i]
alist=[54,26,93,17,77,31,44,55,20]
select_sort(alist)
print(alist)
```
* 插入排序
```python
def insert_sort(alist):
    for i in range(1,len(alist)):
        for j in range(i,0,-1):
            if alist[j]<alist[j-1]:
                alist[j],alist[j-1]=alist[j-1],alist[j]
            else:
                break
alist=[54,26,93,17,77,31,44,55,20]
insert_sort(alist)
print(alist)
```
* 希尔排序
```python
# 变换步长（增量）的插入排序->(n ~ n^2,不稳定)
def shell_sort(alist):
    gap=len(alist)//2
    while gap>=1:
        for i in range(gap,len(alist)):
            j=i
            while(j-gap)>=0:
                if alist[j]<alist[j-gap]:
                    alist[j],alist[j-gap]=alist[j-gap],alist[j]
                    j-=gap
                else:
                    break
        gap//=2
alist=[54,26,93,17,77,31,44,55,20]
shell_sort(alist)
print(alist)
```
* 归并排序
```python
#分而治之，递归分解/递归合并 （nlogn）
def merge_sort(alist):
    if len(alist)<=1:
        return alist
    mid = len(alist)//2
    left_alist = merge_sort(alist[:mid])
    right_alist = merge_sort(alist[mid:])
    return merge(left_alist,right_alist)
def merge(left_list,right_list):
    result=[]
    j=0
    i=0
    while i<len(left_list) and j < len(right_list):
        if left_list[i]<=right_list[j]:
            result.append(left_list[i])
            i+=1
        else:
            result.append(right_list[j])
            j+=1
    result+=left_list[i:]
    result+=right_list[j:]
    return result
alist=[54,26,93,17,77,31,44,55,20]
print(merge_sort(alist))
```
* 快速排序
```python
# 快速排序使用分而治之来获得与归并排序相同的优点，而不使用额外的存储。
# 有可能列表不能被分成两半。当这种情况发生时，性能降低
def quick_sort(alist, start, end):
    if start>= end:
        return
    #基准
    mark = alist[start]
    left = start
    right = end
    while left < right:
        while left<right  and alist[right]>mark:
            right-=1
        alist[left]=alist[right]
        while left<right and alist[left]<mark:
            left+=1
        alist[right]=alist[left]
    alist[right]=mark
    quick_sort(alist,start,left-1)
    quick_sort(alist,left+1,end)
alist=[54,26,93,17,77,31,44,55,20]
quick_sort(alist,0,len(alist)-1)
print(alist)
```
##### [链表算法](https://mp.weixin.qq.com/s?__biz=MzUyNjQxNjYyMg==&mid=2247484830&idx=1&sn=9d24fc787da4b49b82ac01c7f8de257b&chksm=fa0e6a1fcd79e309a2e7f3e09ec9913a55f1c077287c907f13528578b7785831a2effb3104e0&scene=21#wechat_redirect)
* 输出/删除 单链表倒数第 K 个节点
```python
# leetcode 19：快慢双指针
class Solution:
    def removeNthFromEnd(self, head: ListNode, n: int) -> ListNode:
        second = fist = head
        for i in range(n):  # 第一个指针先走 n 步
            fist = fist.next
 
        if fist == None:  # 如果现在第一个指针已经到头了，那么第一个结点就是要删除的结点。
            return second.next
 
        while fist.next:  # 然后同时走，直到第一个指针走到头
            fist = fist.next
            second = second.next
        second.next = second.next.next  # 删除相应的结点
        return head
```
* 判断链表是否有环
* 使用链表实现大数加法
```python
# leetcode 2
class Solution:
    def addTwoNumbers(self, l1: ListNode, l2: ListNode) -> ListNode:
        flag=0
        root=n=ListNode(0)
        while l1 or l2 or flag:
            v1=v2=0
            if l1:
                v1=l1.val
                l1=l1.next
            if l2:
                v2=l2.val
                l2=l2.next
            flag,val=divmod(v1+v2+flag,10)
            n.next=ListNode(val)
            n=n.next
        return root.next  
```
* 合并K个排序链表
```python
# leetcode 23
class Solution:
    def mergeKLists(self, lists: List[ListNode]) -> ListNode:
        k_heap=[]
        for i in lists:
            while i:
                k_heap.append(i.val)
                i=i.next
        if k_heap==[]:
            return []
        k_heap.sort()
        head=cur=ListNode(0)
        while k_heap:
            cur.next=ListNode(k_heap.pop(0))
            cur=cur.next
        return head.next
```
* 删除链表中节点，要求时间复杂度为O(1)
* 反转链表
* 从尾到头打印链表
* LRU缓存机制
##### 栈和队列算法
* [以下几个算法原理详解](https://mp.weixin.qq.com/s?__biz=MzUyNjQxNjYyMg==&mid=2247484846&idx=2&sn=e508da06e9f7a0b3d00db5415d7ce622&chksm=fa0e6a2fcd79e3397fe8083f9493ae639f47c9448ac2a0026026494d098c47ecc6e08f1f8e28&scene=21#wechat_redirect)
* 有效的括号
```python
# leetcode 20
class Solution:
    def isValid(self, s: str) -> bool:
        chars={'(':')','[':']','{':'}'}
        stack=[]
        for i in s:
            if i in chars:
                stack.append(i)
            else:
                if not stack or chars[stack.pop()]!=i:
                    return False
        return not stack
```
* 用两个栈实现队列
```python
# leetcode 232: 一个栈作为缓存区
class MyQueue:

    def __init__(self):
        """
        Initialize your data structure here.
        """
        self.stack1=[]
        self.stack2=[]
        

    def push(self, x: int) -> None:
        """
        Push element x to the back of queue.
        """
        self.stack1.append(x)
        

    def pop(self) -> int:
        """
        Removes the element from in front of queue and returns that element.
        """
        if len(self.stack2)==0:
            while(self.stack1):
                self.stack2.append(self.stack1.pop())
        return self.stack2.pop()

    def peek(self) -> int:
        """
        Get the front element.
        """
        if len(self.stack2)==0:
            while(self.stack1):
                self.stack2.append(self.stack1.pop())
        return self.stack2[-1]

    def empty(self) -> bool:
        """
        Returns whether the queue is empty.
        """
        return not self.stack1 and not self.stack2
```
* 栈的压入、弹出序列
```python
# leetcode 946:借用一个辅助的栈tmp，遍历压栈顺序
class Solution:
    def validateStackSequences(self, pushed: List[int], popped: List[int]) -> bool:
        tmp=[]
        while pushed:
            tmp.append(pushed.pop(0))
            while tmp and tmp[-1]==popped[0]:
                popped.pop(0)
                tmp.pop()
        return not tmp
```
* 包含 min 函数的栈
```python
# leetcode 155：实际上就是实现最小栈
class MinStack:

    def __init__(self):
        """
        initialize your data structure here.
        """
        self.stack=[]
        self.minstack=[]

    def push(self, x: int) -> None:
        self.stack.append(x)
        if self.minstack:
            self.minstack.append(x)
        else:
            if x<self.minstack[-1]:
                self.minstack.append(x)
            else:
                self.minstack.append(self.minstack[-1])

    def pop(self) -> None:
        self.stack.pop()
        self.minstack.pop()

    def top(self) -> int:
        return self.stack[-1]

    def getMin(self) -> int:
        return self.minstack[-1]
```
##### 二叉树算法
##### 字符串算法
* 最长公共前缀
```python
# leetcode 14
class Solution:
    def longestCommonPrefix(self, strs: List[str]) -> str:
        temp_str=""
        zip_obj = zip(*strs)
        for obj in zip_obj:
            if(len(set(obj)))>1:
                break
            temp_str+=obj[0]
        return temp_str 
```
* 最长回文子串
```python
# leetcode 5
class Solution:
    def longestPalindrome(self, s: str) -> str:
        start=0
        maxstr=0
        for i in range(len(s)):
            if i-maxstr>=1 and s[i-maxstr-1:i+1]==s[i-maxstr-1:i+1][::-1]:
                start = i-maxstr-1
                maxstr+=2
                continue
            if  i-maxstr>=0 and s[i-maxstr:i+1]==s[i-maxstr:i+1][::-1]:
                start = i-maxstr
                maxstr+=1
        return s[start:start+maxstr]
```
* 无重复字符的最长子串
```python
# leetcode 3 ：滑动窗口法
class Solution:
    def lengthOfLongestSubstring(self, s: str) -> int:
        max_str=0
        for i in range(len(s)):
            if len(s[i-max_str:i+1])==len(set(s[i-max_str:i+1])):
                max_str+=1
        return max_str
```
##### 哈希算法
* 两数之和
```python
# leetcode 1
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        #enumerate() 函数用于将一个可遍历的数据对象(如列表、元组或字符串)组合为一个索引序列，同时列出数据和数据下标
        demo_dict = dict((num,i)for i,num in enumerate(nums))
        for i,num in enumerate(nums):
            #get() 方法和 [key] 方法的主要区别在于，[key] 在遇到不存在的 key 时会抛出 KeyError 错
            j=demo_dict.get(target-num)
            if j and i!=j:
                return [i,j]
```
* 三数之和
```python
# leetcode 15
class Solution:
    def threeSum(self, nums: List[int]) -> List[List[int]]:
        nums.sort()
        res = []
        # 排序后遍历
        for t in range(len(nums)- 2):
            # 跳过相同的情况
            if t > 0 and nums[t] == nums[t - 1]:
                    continue
            # i向后判断，j向前判断
            i, j = t + 1, len(nums) - 1
            while i < j:
                _sum = nums[t] + nums[i] + nums[j]
                if _sum == 0:
                    res.append([nums[t], nums[i], nums[j]])
                    i += 1
                    j -= 1
                    # 跳过相同的情况
                    while i < j and nums[i] == nums[i - 1]:
                        i += 1
                    while i < j and nums[j] == nums[j + 1]:
                        j -= 1
                elif _sum < 0:
                    i += 1
                else:
                    j -= 1
        return res
```
* 重复的 DNA 序列
```python
# leetcode 187
class Solution:
    def findRepeatedDnaSequences(self, s: str) -> List[str]:
        res=dict()
        for i in range(len(s)-9):
            res[s[i:i+10]]=res.get(s[i:i+10],0)+1
        return [k for k,v in res.items() if v>=2]
```
* 两个数组的交集 (leetcode 349)
* 两个数组的交集 (leetcode 350)
```python
class Solution:
    def intersect(self, nums1: List[int], nums2: List[int]) -> List[int]:
        res=[]
        num_dict={}
        for num in nums1:
            if num not in num_dict:
                num_dict[num]=1
            else:
                num_dict[num]+=1
        for num in nums2:
            if num in num_dict and num_dict[num]>0:
                num_dict[num]-=1
                res.append(num)
        return res
```
##### [Backtracking回溯法(又称DFS,递归)全解](https://segmentfault.com/a/1190000006121957)
##### [2018 秋招笔试面经](https://github.com/imhuay/Algorithm_Interview_Notes-Chinese/tree/master/D-笔试面经#一面)
#### 操作系统篇
* 主要参考
   - [哈工大李治军老师的OS](https://www.icourse163.org/course/HIT-1002531008)
    - [配套的实验环境](https://www.shiyanlou.com/courses/115)
    - [gitbook和源码](https://github.com/hoverwinter/HIT-OSLab)
    - [Linux内核完全注释](https://book.douban.com/subject/1231236/)
##### 进程与线程区别
* 进程是对运行时程序的封装，是系统进行资源调度和分配的的基本单位，实现了操作系统的并发；线程是进程的子任务，是CPU调度和分派的基本单位，用于保证程序的实时性，实现进程内部的并发。
* 一个程序至少有一个进程，一个进程至少有一个线程，线程依赖于进程而存在；进程在执行过程中拥有独立的内存单元，而多个线程线程是共同享有进程占有的资源和地址空间的(*线程共享的环境包括：进程代码段、进程的公有数据(利用这些共享的数据，线程很容易的实现相互之间的通讯)、进程打开的文件描述符、信号的处理器、进程的当前目录和进程用户ID与进程组ID*)。**进程让操作系统的并发性成为可能，而线程让进程的内部并发成为可能。**
##### 谈谈多线程并发
* 将程序的执行逻辑与调度机制的细节，交替执行的操作，异步 I/O 以及资源等待等问题分离开来。通过使用线程，可以将复杂并且异步的工作流进一步分解为一组简单并且同步的工作流，每个工作流在一个单独的线程中运行，并在特定的同步位置进行交互。 
* 提高资源利用率，多处理器系统的出现，使得同一个程序的多个线程可以被同时调度到多个 CPU 上运行。因此，多线程程序可以通过提高处理器资源的利用率来提升系统的吞吐率。当然多线程程序也有助于在单处理器系统上获得更高的吞吐率（如果程序的一个线程在等待 I/O 操作）
* 多线程的性能不一定优于单线程，对于单核CPU，如果是 CPU密集型任务，如解压文件，多线程的性能反而不如单线程性能，因为解压文件需要一直占用 CPU资源，如果采用多线程，线程切换导致的开销反而会让性能下降。但是对于 IO密集型任务，肯定是需要使用多线程的。而对于多核CPU，对于解压文件来说，多线程肯定优于单线程，因为多个线程能够更加充分利用每个核的资源。
* 使用 queue 进行线程通信。当线程之间如果要共享资源或数据的时候，可能变的非常复杂。Python的threading模块提供了很多同步原语，包括信号量，条件变量，事件和锁。如果可以使用这些原语的话，应该优先考虑使用这些，而不是使用queue（队列）模块。队列操作起来更容易，也使多线程编程更安全，因为队列可以将资源的使用通过单线程进行完全控制，并且允许使用更加整洁和可读性更高的设计模式。
```python
import threading
import time
class GetHtml(threading.Thread):
    def __init__(self,name):
        super().__init__(name=name)
    def run(self):
        print('get html start')
        time.sleep(2)
        print('get html end')
class GetUrl(threading.Thread):
    def __init__(self,name):
        super().__init__(name=name)
    def run(self):
        print('get url start')
        time.sleep(4)
        print('get url end')
if __name__ == "__main__":
    thread1=GetHtml(name='html')
    thread2=GetUrl(name='url')
    start_time=time.time()
    thread1.start()
    thread2.start()
    thread1.join()
    thread2.join()
    end_time=time.time()
    total_time=end_time-start_time
    print('total running tim:{}'.format(total_time))
```
##### [线程同步方式](https://blog.csdn.net/ebowtang/article/details/29905309)
* 线程同步就是协同步调，按预定的先后次序进行运行。如：你说完，我再说。这里的同步千万不要理解成那个同时进行，应是指协同、协助、互相配合。线程同步是指多线程通过特定的设置（如互斥量，事件对象，临界区）来控制线程之间的执行顺序（即所谓的同步）也可以说是在线程之间通过同步建立起执行顺序的关系，如果没有同步，那线程之间是各自运行各自的！
* 线程互斥是指对于共享的进程系统资源，在各单个线程访问时的排它性。当有若干个线程都要使用某一共享资源时，任何时刻最多只允许一个线程去使用，其它要使用该资源的线程必须等待，直到占用资源者释放该资源。线程互斥可以看成是一种特殊的线程同步（下文统称为同步）。
    * **互斥量 Mutex**：采用互斥对象机制，只有拥有互斥对象的线程才有访问公共资源的权限。因为互斥对象只有一个，所以可以保证公共资源不会被多个线程同时访问，当前拥有互斥对象的线程处理完任务后必须将互斥对象交出，以便其他线程访问该资源。(RLock 和 Lock)
    * **信号量 Semaphare**：它允许同一时刻多个线程访问同一资源，但是需要控制同一时刻访问此资源的最大线程数量。一般是将当前可用资源计数设置为最大资源计数，每增加一个线程对共享资源的访问，当前可用资源计数就会减1 ，只要当前可用资源计数是大于0 的，就可以发出信号量信号。但是当前可用计数减小到0时则说明当前占用资源的线程数已经达到了所允许的最大数目，不能在允许其他线程的进入，此时的信号量信号将无法发出。线程在处理完共享资源后，应在离 开的同时通过Release将当前可用资源计数加1，在任何时候当前可用资源计数决不可能大于最大资源计数。
    * **事件对象 Event**：通过通知操作的方式来保持多线程同步，还可以方便的实现多线程优先级的比较操作。事件是内核对象，事件分为手动置位事件和自动置位事件。事件Event内部它包含一个使用计数（所有内核对象都有），一个布尔值表示是手动置位事件还是自动置位事件，另一个布尔值用来表示事件有无触发。
##### 线程有几种状态
##### 分页机制
* [分页机制图文详解](https://www.jianshu.com/p/3558942fe14f)
##### 分页和分段有什么区别（内存管理）
* 主要参考
    - [分段和分页内存管理](https://blog.csdn.net/bupt_tinyfisher/article/details/8939689)
* 段式存储管理是一种符合用户视角的内存分配管理方案。在段式存储管理中，将程序的地址空间划分为若干段（segment），如代码段，数据段，堆栈段；这样每个进程有一个二维地址空间，相互独立，互不干扰。段式管理的优点是：没有内碎片（因为段大小可变，改变段大小来消除内碎片）。但段换入换出时，会产生外碎片（比如 4k 的段换5k 的段，会产生 1k 的外碎片）
* 页式存储管理方案是一种用户视角内存与物理内存相分离的内存分配管理方案。在页式存储管理中，将程序的逻辑地址划分为固定大小的页（page），而物理内存划分为同样大小的帧，程序加载时，可以将任意一页放入内存中任意一个帧，这些帧不必连续，从而实现了离散分离。页式存储管理的优点是：没有外碎片（因为页的大小固定），但会产生内碎片（一个页可能填充不满）
* 两者的不同点：
    - 目的不同：分页是由于系统管理的需要而不是用户的需要，它是信息的物理单位；分段的目的是为了能更好地满足用户的需要，它是信息的逻辑单位，它含有一组其意义相对完整的信息；
    - 大小不同：页的大小固定且由系统决定，而段的长度却不固定，由其所完成的功能决定；
    - 地址空间不同： 段向用户提供二维地址空间；页向用户提供的是一维地址空间；
    - 信息共享：段是信息的逻辑单位，便于存储保护和信息的共享，页的保护和共享受到限制；
    - 内存碎片：页式存储管理的优点是没有外碎片（因为页的大小固定），但会产生内碎片（一个页可能填充不满）；而段式管理的优点是没有内碎片（因为段大小可变，改变段大小来消除内碎片）。但段换入换出时，会产生外碎片（比如 4k 的段换 5k 的段，会产生1k 的外碎片）。
##### 什么是虚拟内存？
* 主要参考
    - [BAT面试之操作系统内存详解](http://www.imooc.com/article/11015)
* 内存的发展历程：没有内存抽象 (单进程，除去操作系统所用的内存之外，全部给用户程序使用) —> 有内存抽象（多进程，进程独立的地址空间，交换技术 (内存大小不可能容纳下所有并发执行的进程)）—> 连续内存分配 (固定大小分区 (多道程序的程度受限)，可变分区 (首次适应，最佳适应，最差适应)，碎片) —> 不连续内存分配（分段，分页，段页式，虚拟内存）。
* 虚拟内存允许执行进程不必完全在内存中。虚拟内存的基本思想是：每个进程拥有独立的地址空间，这个空间被分为大小相等的多个块，称为页 (Page)，每个页都是一段连续的地址。这些页被映射到物理内存，但并不是所有的页都必须在内存中才能运行程序。当程序引用到一部分在物理内存中的地址空间时，由硬件立刻进行必要的映射；当程序引用到一部分不在物理内存中的地址空间时，由操作系统负责将缺失的部分装入物理内存并重新执行失败的命令。这样，对于进程而言，逻辑上似乎有很大的内存空间，实际上其中一部分对应物理内存上的一块 (称为帧，通常页和帧大小相等)，还有一些没加载在内存中的对应在硬盘上。注意，请求分页系统、请求分段系统和请求段页式系统都是针对虚拟内存的，通过请求实现内存与外存的信息置换。
* 局部性原理
    - 时间上的局部性：最近被访问的页在不久的将来还会被访问；
    - 空间上的局部性：内存中被访问的页周围的页也很可能被访问。
* 页面置换算法
    - FIFO 先进先出算法：在操作系统中经常被用到，比如作业调度（主要实现简单，很容易想到）；
    - LRU（Least recently use）最近最少使用算法：根据使用时间到现在的长短来判断；
    - LFU（Least frequently use）最少使用次数算法：根据使用次数来判断；
    - OPT（Optimal replacement）最优置换算法：理论的最优，理论；就是要保证置换出去的是不再被使用的页，或者是在实际内存中最晚使用的算法。
* 虚拟内存的应用与优点：虚拟内存很适合在多道程序设计系统中使用，许多程序的片段同时保存在内存中。当一个程序等待它的一部分读入内存时，可以把 CPU 交给另一个进程使用。虚拟内存的使用可以带来以下好处：
    - 在内存中可以保留多个进程，系统并发度提高
    - 解除了用户与内存之间的紧密约束，进程可以比内存的全部空间还大
##### 颠簸(抖动)
* 颠簸本质上是指频繁的页调度行为，具体来讲，进程发生缺页中断，这时，必须置换某一页。然而，其他所有的页都在使用，它置换一个页，但又立刻再次需要这个页。因此，会不断产生缺页中断，导致整个系统的效率急剧下降，这种现象称为颠簸（抖动）。
* 内存颠簸的解决策略包括：
    - 如果是因为页面替换策略失误，可以修改替换算法来解决这个问题；
    - 如果是因为运行的程序太多，造成程序无法同时将所有频繁访问的页面调入内存，则要降低多道程序的数量；
##### 进程调度算法
* FCFS(先来先服务，队列实现，非抢占的)：先请求CPU的进程先分配到CPU
* SJF(最短作业优先调度算法)：平均等待时间最短，但难以知道下一个CPU区间长度
* 优先级调度算法(可以是抢占的，也可以是非抢占的)：优先级越高越先分配到CPU，相同优先级先到先服务，存在的主要问题是：低优先级进程无穷等待CPU，会导致无穷阻塞或饥饿；
* 时间片轮转调度算法(可抢占的)：队列中没有进程被分配超过一个时间片的CPU时间，除非它是唯一可运行的进程。如果进程的CPU区间超过了一个时间片，那么该进程就被抢占并放回就绪队列。
* 多级队列调度算法：将就绪队列分成多个独立的队列，每个队列都有自己的调度算法，队列之间采用固定优先级抢占调度。其中，一个进程根据自身属性被永久地分配到一个队列中。
* 多级反馈队列调度算法：与多级队列调度算法相比，其允许进程在队列之间移动：若进程使用过多CPU时间，那么它会被转移到更低的优先级队列；在较低优先级队列等待时间过长的进程会被转移到更高优先级队列，以防止饥饿发生。
##### [进程同步机制](https://blog.csdn.net/wangrunmin/article/details/7941592)
* 原子操作、信号量机制、自旋锁管程、会合、分布式系统
##### 进程的状态
* [进程的基本状态及转换和阻塞及挂起的理解](https://blog.csdn.net/Caoyang_He/article/details/80791581)
* 进程的三种状态情况：运行态（占用CPU）;就绪态（可运行，但暂时没有CPU分配给它）；阻塞态(除非某种外部条件发生，就算CPU空闲，也不能执行)。unix用block阻塞。状态转换表
* 就绪状态 ：一个进程获得了除处理机外的一切所需资源，一旦得到处理机即可运行，则称此进程处于就绪状态。
* 执行状态：当一个进程在处理机上运行时，则称该进程处于运行状态。
* 阻塞状态：一个进程正在等待某一事件发生（例如请求I／O而等待I／O完成等）而暂时停止运行，这时即使把处理机分配给进程也无法运行，故称该进程处于阻塞状态。
##### 进程间通信方式
* 主要参考
    * [进程间通信（IPC）介绍](https://www.cnblogs.com/CheeseZH/p/5264465.html)
* 进程间通信（IPC，InterProcess Communication）是指在不同进程之间传播或交换信息。进程间通信（Inter-Process Communication）方式：管道（匿名管道/命名管道），消息队列，**共享内存、信号量、套接字（socket），后三种较常用**
    * **管道**一般指匿名管道，是 UNIX 系统IPC最古老的形式,只能用于具有亲缘关系的进程之间的通信（父子进程或者兄弟进程之间），是半双工的（即数据只能在一个方向上流动），具有固定的读端和写端。它可以看成是一种特殊的文件，对于它的读写也可以使用普通的read、write 等函数。但是它不是普通的文件，并不属于其他任何文件系统，并且只存在于内存。**命名管道（FIFO）**除了具有匿名管道所具有的功能外，它还允许无亲缘关系进程间的通信。
    * **消息队列**是消息的链接表，它克服了上两种通信方式中信号量有限的缺点，具有写权限得进程可以按照一定得规则向消息队列中添加新信息；对消息队列有读权限得进程则可以从消息队列中读取信息；消息队列，是消息的链接表，存放在内核中。一个消息队列由一个标识符（即队列ID）来标识。
    * **共享内存**可以说这是最有用的进程间通信方式。它使得多个进程可以访问同一块内存空间，不同进程可以及时看到对方进程中对共享内存中数据得更新。这种方式需要依靠某种同步操作，如互斥锁和信号量等；共享内存（Shared Memory），指两个或多个进程共享一个给定的存储区。特点:共享内存是最快的一种 IPC，因为进程是直接对内存进行存取。因为多个进程可以同时操作，所以需要进行同步。信号量+共享内存通常结合在一起使用，信号量用来同步对共享内存的访问。
    * **信号量**主要作为进程之间及同一种进程的不同线程之间得同步和互斥手段；信号量（semaphore）与已经介绍过的 IPC 结构不同，它是一个计数器。信号量用于实现进程间的互斥与同步，而不是用于存储进程间通信数据。特点：信号量用于进程间同步，若要在进程间传递数据需要结合共享内存。[信号量基于操作系统的 PV 操作](https://blog.csdn.net/u014495460/article/details/82883282)，程序对信号量的操作都是原子操作。每次对信号量的 PV 操作不仅限于对信号量值加 1 或减 1，而且可以加减任意正整数。支持信号量组。
    * **套接字**，这是一种更为一般得进程间通信机制，它可用于网络中不同机器之间的进程间通信，应用非常广泛。
##### [僵尸进程和孤儿进程](https://www.cnblogs.com/Anker/p/3271773.html#3777880)
##### fork进程时的操作
##### Socket编程
* [Socket Programming in Python (Guide)](https://realpython.com/python-sockets/)
![20190507170534122.png](https://i.loli.net/2019/08/13/e1MknSJRAbXI3du.png)
##### Linux的五种IO模型
* 主要参考
    * [聊聊IO多路复用之select、poll、epoll详解](https://mp.weixin.qq.com/s?__biz=MzAxODI5ODMwOA==&mid=2666538922&idx=1&sn=e6b436efd6a4f53dcbf20f4ce11a986a&scene=23&srcid=0425xFfzV9LmmVrdeEQ4He1W#rd)
    * [漫话：如何给女朋友解释什么是Linux的五种IO模型](https://juejin.im/post/5b94e93b5188255c672e901e#comment)

* 在Linux(UNIX)操作系统中，共有五种IO模型，分别是：阻塞IO模型、非阻塞IO模型、IO复用模型、信号驱动IO模型以及异步IO模型。 I/O操作，以一次磁盘文件读取为例，读取的文件是存储在磁盘上的，我们的目的是把它读取到内存中，可以把这个步骤简化成（真正的文件读取还涉及到缓存等细节）把数据从硬件（硬盘）中读取到用户空间中。关于用户空间、内核空间以及硬件等的关系如可以通过钓鱼的例子理解。鱼塘就可以映射成磁盘，中间过渡的鱼钩可以映射成内核空间，最终放鱼的鱼篓可以映射成用户空间。一次完整的钓鱼（IO）操作，是鱼（文件）从鱼塘（硬盘）中转移（拷贝）到鱼篓（用户空间）的过程。
1. **阻塞IO模型**。应用进程通过系统调用 recvfrom 接收数据，但由于内核还未准备好数据报，应用进程就会阻塞住，直到内核准备好数据报，recvfrom 完成数据报复制工作，应用进程才能结束阻塞状态。（并发低，时效性要求低）
![utf-8165bde9e5723181b.jpg](https://i.loli.net/2019/08/16/PbuHlOjvmwNdTV4.jpg)
2. **非阻塞IO模型**。应用进程通过 recvfrom 调用不停的去和内核交互，直到内核准备好数据。如果没有准备好，内核会返回error，应用进程在得到error后，过一段时间再发送recvfrom请求。在两次发送请求的时间段，进程可以先做别的事情。
![65bde9e699d0713.jpg](https://i.loli.net/2019/08/16/48SqhVp672HUZG3.jpg)
3. **IO多路复用模型**。IO多路转接是多了一个select函数，多个进程的IO可以注册到同一个select上，当用户进程调用该select，select会监听所有注册好的IO，如果所有被监听的IO需要的数据都没有准备好时，select调用进程会阻塞。当任意一个IO所需的数据准备好之后，select调用就会返回，然后进程在通过recvfrom来进行数据拷贝。这里的IO复用模型，并没有向内核注册信号处理函数，所以，他并不是非阻塞的。进程在发出select后，要等到select监听的所有IO操作中至少有一个需要的数据准备好，才会有返回，并且也需要再次发送请求去进行文件的拷贝。PS: 这种方式的钓鱼，通过增加鱼竿的方式，可以有效的提升效率。
![165bde9e6e6da275.jpg](https://i.loli.net/2019/08/16/MFGRjAe8ontQ2U1.jpg)
4. **信号驱动IO模型**。应用进程预先向内核注册一个信号处理函数，然后用户进程返回，并且不阻塞，当内核数据准备就绪时会发送一个信号给进程，用户进程便在信号处理函数中开始把数据拷贝的用户空间中。PS: 这种方式钓鱼，和前几种相比，所使用的工具有了一些变化，需要有一些定制（实现复杂）。但是钓鱼的人就可以在鱼儿咬钩之前彻底做别的事儿去了。等着报警器响就行了。
![ut165bde9e6c6552e2.jpg](https://i.loli.net/2019/08/16/7hV4NISfOwTktWE.jpg)
5. **异步IO模型**。用户进程发起aio_read操作之后，给内核传递描述符、缓冲区指针、缓冲区大小等，告诉内核当整个操作完成时，如何通知进程，然后就立刻去做其他事情了。当内核收到aio_read后，会立刻返回，然后内核开始等待数据准备，数据准备好以后，直接把数据拷贝到用户控件，然后再通知进程本次IO已经完成。(应用进程把IO请求传给内核后，完全由内核去操作文件拷贝。内核完成相关操作后，会发信号告诉应用进程本次IO已经完成。)
![](https://i.imgsafe.org/60/6095077381.jpeg)
* 五种IO模型比较:以上前四种都是同步的IO模型。因为，无论以上那种模型，真正的数据拷贝过程，都是同步进行的。信号驱动难道不是异步的么？ 信号驱动，内核是在数据准备好之后通知进程，然后进程再通过recvfrom操作进行数据拷贝。我们可以认为数据准备阶段是异步的，但是，数据拷贝操作是同步的。所以，整个IO过程也不能认为是异步的。
![](https://i.imgsafe.org/60/609e06b39f.jpeg)
##### IO 多路复用模型
* I/O多路复用就是通过一种机制，一个进程可以监视多个描述符，一旦某个描述符就绪（一般是读就绪或者写就绪），能够通知程序进行相应的读写操作。但select，pselect，poll，epoll本质上都是同步I/O(epoll是Linux所特有，而select则应该是POSIX所规定的)，因为他们都需要在读写事件就绪后自己负责进行读写，也就是说这个读写过程是阻塞的。与多进程和多线程技术相比，I/O多路复用技术的最大优势是系统开销小，系统不必创建进程/线程，也不必维护这些进程/线程，从而大大减小了系统的开销。
* IO多路复用是指内核一旦发现进程指定的一个或者多个IO条件准备读取，它就通知该进程。IO多路复用适用如下场合：
    1. 当客户处理多个描述符时（一般是交互式输入和网络套接口），必须使用I/O复用。
    2. 当一个客户同时处理多个套接口时，而这种情况是可能的，但很少出现。
    3. 如果一个TCP服务器既要处理监听套接口，又要处理已连接套接口，一般也要用到I/O复用
    4. 如果一个服务器即要处理TCP，又要处理UDP，一般要使用I/O复用。
    5.  如果一个服务器要处理多个服务或多个协议，一般要使用I/O复用。
###### select
* select 函数监视的文件描述符分3类，分别是writefds、readfds、和exceptfds。调用后select函数会阻塞，直到有描述符就绪（有数据 可读、可写、或者有except），或者超时（timeout指定等待时间，如果立即返回设为null即可），函数返回。当select函数返回后，可以通过遍历fdset，来找到就绪的描述符。
###### poll
* poll本质上和select没有区别，它将用户传入的数组拷贝到内核空间，然后查询每个fd对应的设备状态，如果设备就绪则在设备等待队列中加入一项并继续遍历，如果遍历完所有fd后没有发现就绪设备，则挂起当前进程，直到设备就绪或者主动超时，被唤醒后它又要再次遍历fd。这个过程经历了多次无谓的遍历。
###### epoll
* epoll支持水平触发和边缘触发，最大的特点在于边缘触发，它只告诉进程哪些fd刚刚变为就绪态，并且只会通知一次。还有一个特点是，epoll使用“事件”的就绪通知方式，通过epoll_ctl注册fd，一旦该fd就绪，内核就会采用类似callback的回调机制来激活该fd，epoll_wait便可以收到通知。
###### select、poll、epoll区别
* 支持一个进程所能打开的最大连接数
![Snipaste_2019-05-29_10-08-08.png](https://i.loli.net/2019/08/16/YDrUzSZBdHOCFeN.png)
* FD剧增后带来的IO效率问题
![Snipaste_2019-05-29_10-08-18.png](https://i.loli.net/2019/08/16/jdLBwPryzn5Mp2W.png)
* 消息传递方式
![Snipaste_2019-05-29_10-08-28.png](https://i.loli.net/2019/08/16/koPVBeFp1XIYGfS.png)
* 最佳实践：表面上看epoll的性能最好，但是在连接数少并且连接都十分活跃的情况下，select和poll的性能可能比epoll好，毕竟epoll的通知机制需要很多函数回调。select低效是因为每次它都需要轮询。但低效也是相对的，视情况而定，也可通过良好的设计改善。
##### 谈谈死锁
###### 死锁的概念　　　
* 在两个或者多个并发进程中，如果每个进程持有某种资源而又等待其它进程释放它或它们现在保持着的资源，在未改变这种状态之前都不能向前推进，称这一组进程产生了死锁。通俗的讲，就是两个或多个进程无限期的阻塞、相互等待的一种状态。
###### 死锁产生的原因
* 系统中的资源可以分为两类：
* 可剥夺资源，是指某进程在获得这类资源后，该资源可以再被其他进程或系统剥夺，CPU和主存均属于可剥夺性资源；
* 不可剥夺资源，当系统把这类资源分配给某进程后，再不能强行收回，只能在进程用完后自行释放，如磁带机、打印机等。
* 产生死锁中的竞争资源之一指的是竞争不可剥夺资源（例如：系统中只有一台打印机，可供进程P1使用，假定P1已占用了打印机，若P2继续要求打印机打印将阻塞）
* 产生死锁中的竞争资源另外一种资源指的是竞争临时资源（临时资源包括硬件中断、信号、消息、缓冲区内的消息等），通常消息通信顺序进行不当，则会产生死锁。
###### 死锁产生的四个必要条件
* 互斥：至少有一个资源必须属于非共享模式，即一次只能被一个进程使用；若其他申请使用该资源，那么申请进程必须等到该资源被释放为止；
* 占有并等待：一个进程必须占有至少一个资源，并等待另一个资源，而该资源为其他进程所占有；
* 非抢占：进程不能被抢占，即资源只能被进程在完成任务后自愿释放
* 循环等待：若干进程之间形成一种头尾相接的环形等待资源关系
###### 解决死锁的基本方法
* 解决死锁的基本方法主要有 预防死锁、避免死锁、解除死锁
* **预防死锁**的基本思想是 只要**确保死锁发生的四个必要条件中至少有一个不成立，就能预防死锁的发生**，具体方法包括：
    * 打破互斥条件：允许进程同时访问某些资源。但是，有些资源是不能被多个进程所共享的，这是由资源本身属性所决定的，因此，这种办法通常并无实用价值。
    * 打破占有并等待条件：可以实行资源预先分配策略(进程在运行前一次性向系统申请它所需要的全部资源，若所需全部资源得不到满足，则不分配任何资源，此进程暂不运行；只有当系统能满足当前进程所需的全部资源时，才一次性将所申请资源全部分配给该线程)或者只允许进程在没有占用资源时才可以申请资源（一个进程可申请一些资源并使用它们，但是在当前进程申请更多资源之前，它必须全部释放当前所占有的资源）。但是这种策略也存在一些缺点：在很多情况下，无法预知一个进程执行前所需的全部资源，因为进程是动态执行的，不可预知的；同时，会降低资源利用率，导致降低了进程的并发性。
    * 打破非抢占条件：允许进程强行从占有者哪里夺取某些资源。也就是说，但一个进程占有了一部分资源，在其申请新的资源且得不到满足时，它必须释放所有占有的资源以便让其它线程使用。这种预防死锁的方式实现起来困难，会降低系统性能。
    * 打破循环等待条件：实行资源有序分配策略。对所有资源排序编号，所有进程对资源的请求必须严格按资源序号递增的顺序提出，即只有占用了小号资源才能申请大号资源，这样就不回产生环路，预防死锁的发生。
* **避免死锁**的基本思想是动态地检测资源分配状态，以确保循环等待条件不成立，从而确保系统处于安全状态。所谓安全状态是指：如果系统能按某个顺序为每个进程分配资源（不超过其最大值），那么系统状态是安全的，换句话说就是，如果存在一个安全序列，那么系统处于安全状态。资源分配图算法和银行家算法是两种经典的死锁避免的算法，其可以确保系统始终处于安全状态。其中，资源分配图算法应用场景为每种资源类型只有一个实例(申请边，分配边，需求边，不形成环才允许分配)，而银行家算法应用于每种资源类型可以有多个实例的场景。
* **解除死锁**
    * 终止进程（简单粗暴），就是字面上的，你们死锁了，我就把你们一起杀掉，缺点就是如果一个进程跑了很长时间，但是被杀了，还得从头来。
    * 逐个终止进程，按照某种顺序，挨个杀死进程，每杀一个进程就去看看死锁解除了没有（每杀一个进程都会释放一些资源，如果释放好粗来的资源解决了死锁问题，就没必要再滥杀无辜了），没解除就继续杀。
#### 计算机网络篇
* 主要参考
    - [协议森林](https://www.cnblogs.com/vamei/archive/2012/12/05/2802811.html)
    - [HTTP协议详解](https://www.cnblogs.com/TankXiao/archive/2012/02/13/2342672.html)
##### [从URL输入到页面展现到底发生什么？](https://mp.weixin.qq.com/s?__biz=Mzg5ODA5NTM1Mw==&mid=2247483803&idx=1&sn=460597ae3bd3ec10ad3426b7db605074&chksm=c066800df711091b2b6e005a922fff4a6a8e4b7930928a1c60fc0ac657c3ea5061cf1b51563d&mpshare=1&scene=1&srcid=#rd)
* DNS查询，ARP解析，TCP三次握手连接，HTTP请求，反向代理Nginx，uwsgi/gunicorn（WSGI服务器）,服务器响应，浏览器页面渲染，TCP四次挥手，拜拜
##### ARP 协议工作原理
* 网络层的 ARP 协议完成了 IP 地址与物理地址的映射。首先，每台主机都会在自己的 ARP 缓冲区中建立一个 ARP列表，以表示 IP 地址和 MAC 地址的对应关系。当源主机需要将一个数据包要发送到目的主机时，会首先检查自己 ARP 列表中是否存在该 IP 地址对应的 MAC 地址：如果有，就直接将数据包发送到这个 MAC 地址；如果没有，就向本地网段发起一个 ARP 请求的广播包，查询此目的主机对应的 MAC 地址。此 ARP 请求数据包里包括源主机的 IP 地址、硬件地址、以及目的主机的 IP 地址。网络中所有的主机收到这个 ARP 请求后，会检查数据包中的目的 IP 是否和自己的 IP 地址一致。如果不相同就忽略此数据包；如果相同，该主机首先将发送端的 MAC 地址和 IP 地址添加到自己的 ARP 列表中，如果 ARP 表中已经存在该 IP 的信息，则将其覆盖，然后给源主机发送一个 ARP 响应数据包，告诉对方自己是它需要查找的 MAC 地址；源主机收到这个 ARP 响应数据包后，将得到的目的主机的 IP 地址和 MAC 地址添加到自己的 ARP 列表中，并利用此信息开始数据的传输。如果源主机一直没有收到 ARP 响应数据包，表示 ARP 查询失败。
##### TCP 三次握手
* 重点记住每个阶段以后客户和服务器的状态变化
![20180717202520531.png](https://i.loli.net/2019/08/15/xpwUj2QYqrEz5a3.png)
* 为什么不能用两次握手进行连接？
答：为了防止 已失效的链接请求报文突然又传送到了服务端，因而产生错误。客户端发出的连接请求报文并未丢失，而是在某个网络节点长时间滞留了，以致延误到链接释放以后的某个时间才到达 Server。这是，Server 误以为这是 Client 发出的一个新的链接请求，于是就向客户端发送确认数据包，同意建立链接。若不采用 “三次握手”，那么只要 Server 发出确认数据包，新的链接就建立了。由于 client 此时并未发出建立链接的请求，所以其不会理睬 Server 的确认，也不与 Server通信；而这时 Server 一直在等待 Client 的请求，这样Server 就白白浪费了一定的资源。若采用 “三次握手”，在这种情况下，由于 Server 端没有收到来自客户端的确认，则就会知道 Client 并没有要求建立请求，就不会建立链接。
##### TCP 四次挥手
![20180717204202563.png](https://i.loli.net/2019/08/15/yqCMJ3jxzErW4it.png)
* 为什么TIME_WAIT状态需要经过2MSL(最大报文段生存时间)才能返回到CLOSE状态？
答：虽然按道理，四个报文都发送完毕，我们可以直接进入CLOSE状态了，但是我们必须假象网络是不可靠的，有可以最后一个ACK丢失。所以TIME_WAIT状态就是用来重发可能丢失的ACK报文。在Client发送出最后的ACK回复，但该ACK可能丢失。Server如果没有收到ACK，将不断重复发送FIN片段。所以Client不能立即关闭，它必须确认Server接收到了该ACK。Client会在发送出ACK之后进入到TIME_WAIT状态。Client会设置一个计时器，等待2MSL的时间。如果在该时间内再次收到FIN，那么Client会重发ACK并再次等待2MSL。所谓的2MSL是两倍的MSL(Maximum Segment Lifetime)。MSL指一个片段在网络中最大的存活时间，2MSL就是一个发送和一个回复所需的最大时间。如果直到2MSL，Client都没有再次收到FIN，那么Client推断ACK已经被成功接收，则结束TCP连接。
##### TCP 怎样保证可靠性
* 数据包校验：目的是检测数据在传输过程中的任何变化，若校验出包有错，则丢弃报文段并且不给出响应，这时 TCP 发送数据端超时后会重发数据；
* 对失序数据包重排序：既然 TCP 报文段作为 IP 数据报来传输，而 IP 数据报的到达可能会失序，因此TCP 报文段的到达也可能会失序。TCP 将对失序数据进行重新排序，然后才交给应用层；
* 丢弃重复数据：对于重复数据，能够丢弃重复数据；
* 应答机制：当 TCP 收到发自 TCP 连接另一端的数据，它将发送一个确认。这个确认不是立即发送，通常将推迟几分之一秒；
* 超时重发：当 TCP 发出一个段后，它启动一个定时器，等待目的端确认收到这个报文段。如果不能及时收到一个确认，将重发这个报文段；
* 流量控制：TCP 连接的每一方都有固定大小的缓冲空间。TCP 的接收端只允许另一端发送接收端缓冲区所能接纳的数据，这可以防止较快主机致使较慢主机的缓冲区溢出，这就是流量控制。TCP 使用的流量控制协议是可变大小的滑动窗口协议。
##### [TCP的流量控制和拥塞控制](https://blog.csdn.net/yechaodechuntian/article/details/25429143)
* 计算机网络中的带宽、交换结点中的缓存及处理机等都是网络的资源。在某段时间，若对网络中某一资源的需求超过了该资源所能提供的可用部分，网络的性能就会变坏，这种情况就叫做拥塞。拥塞控制就是 防止过多的数据注入网络中，这样可以使网络中的路由器或链路不致过载。注意，拥塞控制和流量控制不同，前者是一个全局性的过程，而后者指点对点通信量的控制。
##### TCP 与 UDP 的区别
* TCP 是面向连接的，UDP 是无连接的；
* TCP 是可靠的，UDP 是不可靠的；
* TCP 只支持点对点通信，UDP 支持一对一、一对多、多对一、多对多的通信模式；
* TCP 是面向字节流的，UDP 是面向报文的；
* TCP 有拥塞控制机制; UDP 没有拥塞控制，适合媒体通信；
* TCP 首部开销 (20 个字节) 比 UDP 的首部开销 (8 个字节) 要大
##### HTTP协议
* 超文本传输协议(HTTP)是一种通信协议，它允许将超文本标记语言(HTML)文档从Web服务器传送到客户端的浏览器，目前我们使用的是HTTP/1.1 版本。
* HTTP协议是无状态的，同一个客户端的这次请求和上次请求是没有对应关系，对http服务器来说，它并不知道这两个请求来自同一个客户端。 为了解决这个问题， Web程序引入了Cookie机制和session机制来维护状态。
* HTTP/1.1起，默认都开启了Keep-Alive，保持连接特性，简单地说，当一个网页打开完成后，客户端和服务器之间用于传输HTTP数据的TCP连接不会关闭，如果客户端再次访问这个服务器上的网页，会继续使用这一条已经建立的连接。Keep-Alive不会永久保持连接，它有一个保持时间，可以在不同的服务器软件（如Apache）中设定这个时间。
###### HTTP 和 HTTPS 的区别
1. https协议需要到CA申请证书，一般免费证书较少，因而需要一定费用。
2. http是超文本传输协议，信息是明文传输，https则是具有安全性的ssl/tls加密传输协议。
3. http和https使用的是完全不同的连接方式，用的端口也不一样，前者是80，后者是443。
4. http的连接很简单，是无状态的；HTTPS协议是由SSL/TLS+HTTP协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。
###### URL详解
* URL(Uniform Resource Locator) 地址用于描述一个网络上的资源,  基本格式如下：
```
schema://host[:port#]/path/.../[?query-string][#anchor]
>schema               指定低层使用的协议(例如：http, https,ftp)
host                   HTTP服务器的IP地址或者域名
port#         HTTP服务器的默认端口是80，这种情况下端口号可以省略。如果使用了别的端口，必须指明
path                 访问资源的路径
query-string       发送给http服务器的数据
anchor             锚
```
##### HTTP 常见方法（GET/PUT）
* Http协议定义了很多与服务器交互的方法，最基本的有4种，分别是GET,POST,PUT,DELETE. 一个URL地址用于描述一个网络上的资源，而HTTP中的GET, POST, PUT, DELETE就对应着对这个资源的查，改，增，删4个操作。 
###### 安全性和幂等性
* 安全意味着该操作用于获取信息而非修改信息。幂等意味着对同一 URL 的多个请求应该返回同样的结果。
![Snipaste_2019-05-09_08-39-20.png](https://i.loli.net/2019/08/13/Z74rHxcqbkM93A8.png)
###### GET和POST 区别
* 最常见的就是GET和POST了。GET一般用于获取/查询资源信息，而POST一般用于更新资源信息.
* GET提交的数据会放在URL之后，以?分割URL和传输数据，参数之间以&相连?name=test1&id=123456.  POST方法是把提交的数据放在HTTP包的Body中.
* GET提交的数据大小有限制（因为浏览器对URL的长度有限制），而POST方法提交的数据没有限制。
* GET方式提交数据，会带来安全问题，比如一个登录页面，通过GET方式提交数据时，用户名和密码将出现在URL上，如果页面可以被缓存或者其他人可以访问这台机器，就可以从历史记录获得该用户的账号和密码。
##### 常见 HTTP 状态码
* Response 消息中的第一行叫做状态行，由HTTP协议版本号，状态码，状态消息三部分组成。状态码用来告诉HTTP客户端,HTTP服务器是否产生了预期的Response。HTTP/1.1中定义了5类状态码，状态码由三位数字组成，第一个数字定义了响应的类别
    ```
    1XX  提示信息 - 表示请求已被成功接收，继续处理
    2XX  成功 - 表示请求已被成功接收，理解，接受
        200 OK :  表明该请求被成功地完成，所请求的资源发送回客户端
    3XX  重定向 - 要完成请求必须进行更进一步的处理
        302 Found :  重定向，新的URL会在response 中的Location中返回，浏览器将会
        自动使用新的URL发出新的Request
        304 Not Modified :  代表上次的文档已经被缓存了， 还可以继续使用
        （提示：如果你不想使用本地缓存可以用Ctrl+F5 强制刷新页面）
    4XX  客户端错误 -  请求有语法错误或请求无法实现
        400 Bad Request ： 客户端请求与语法错误，不能被服务器所理解
        403 Forbidden :  服务器收到请求，但是拒绝提供服务
        404 Not Found : 请求资源不存在（还有可能是输错了URL)
    5XX  服务器端错误 -   服务器未能实现合法的请求
        500 Internal Server Error:服务器发生了不可预期的错误
        503 Server Unavailable:服务器当前不能处理客户端的请求，一段时间后可能恢复正常
    ```
##### HTTP 长连接与短连接
###### 长连接
* **长连接定义**：client方与server方先建立连接，连接建立后不断开，然后再进行报文发送和接收。这种方式下由于通讯连接一直存在。此种方式常用于P2P点对点的通信。长连接的操作步骤是：建立连接——数据传输...（保持连接）...数据传输——关闭连接
* **长连接适用场景**：以下这些连接，如果每次操作都要建立连接然后再操作的话处理速度会降低。所以操作时第一次连接上以后，以后每次直接发送数据就可以了，不用再建立TCP连接。
    * 即时通信系统：其它用户登录、发送信息；
    * 即时报价系统：后台数据库内容发生变化；
    * 数据库的连接用长连接，如果用短连接频繁的通信会造成socket错误，频繁的socket创建也是对资源的浪费。
###### 短连接
* **短连接定义**: Client方与server每进行一次报文收发交易时才进行通讯连接，交易完毕后立即断开连接。此方式常用于一点对多点通讯。短连接的操作步骤是：建立连接——数据传输——关闭连接...建立连接——数据传输——关闭连接
* **短连接的适用场景**：短连接多用于操作频繁，点对点的通讯，而且连接数不能太多的情况。每个TCP连接的建立都需要三次握手，每个TCP连接的断开要四次握手。web网站的http服务一般都用短连接。因为长连接对于服务器来说要耗费一定的资源。像web网站这么频繁的成千上万甚至上亿客户端的连接用短连接更省一些资源。 
##### cookie 和 session 的区别
* 会话状态保存在客户端。客户端请求服务器，如果服务器需要记录该用户状态，就向客户端浏览器颁发一个 Cookie，而客户端浏览器会把Cookie 保存起来。当浏览器再请求该网站时，浏览器把请求的网址连同该 Cookie 一同提交给服务器，服务器检查该Cookie，以此来辨认用户状态。服务器还可以根据需要修改Cookie 的内容。
* 会话状态也可以保存在服务器端。客户端请求服务器，如果服务器记录该用户状态，就获取 Session 来保存状态，这时，如果服务器已经为此客户端创建过 session，服务器就按照 sessionid 把这个 session 检索出来使用；如果客户端请求不包含 sessionid，则为此客户端创建一个session 并且生成一个与此 session 相关联的 sessionid，并将这个 sessionid 在本次响应中返回给客户端保存。保存这个 sessionid 的方式可以采用 cookie 机制 ，这样在交互过程中浏览器可以自动的按照规则把这个标识发挥给服务器；若浏览器禁用 Cookie 的话，可以通过 URL 重写机制将sessionid 传回服务器。
* 实现机制：Session 的实现常常依赖于 Cookie 机制，通过 Cookie 机制回传 SessionID；
* 安全性：Cookie 存在安全隐患，通过拦截或本地文件找得到 cookie 后可以进行攻击，而 Session 由于保存在服务器端，相对更加安全；
* 大小限制：Cookie 有大小限制并且浏览器对每个站点也有 cookie 的个数限制，Session 没有大小限制，理论上只与服务器的内存大小有关；
* 服务器资源消耗：Session 是保存在服务器端上会存在一段时间才会消失，如果 session 过多会增加服务器的压力。
##### JSON Web Token
##### IP 地址的分类
* IP 地址是指互联网协议地址，是 IP 协议提供的一种统一的地址格式，它为互联网上的每一个网络和每一台主机分配一个逻辑地址，以此来屏蔽物理地址的差异。IP 地址编址方案将 IP 地址空间划分为 A、B、C、D、E 五类，其中 A、B、C 是基本类，D、E 类作为多播和保留使用，为特殊地
址。
* 每个 IP 地址包括两个标识码（ID），即网络 ID 和主机ID。同一个物理网络上的所有主机都使用同一个网络 ID，网络上的一个主机（包括网络上工作站，服务器和路由器等）有一个主机 ID 与其对应。A~E 类地址的特点如下：
    - A 类地址：以 0 开头，第一个字节范围：0~127；
    - B 类地址：以 10 开头，第一个字节范围：128~191；
    - C 类地址：以 110 开头，第一个字节范围：192~223；
    - D 类地址：以 1110 开头，第一个字节范围为: 224~239；
    - E 类地址：以 1111 开头，保留地址
##### OSI七层参考模型
![OSI网络参考模型功能表示.png](https://i.loli.net/2019/08/15/HKS5TkxRfrbMVpC.png)
#### 数据库篇
* 主要参考
    - [MySQL 学习资源整理](https://blog.csdn.net/orangleliu/article/details/54694272)
    - [知乎龚子捷的回答](https://www.zhihu.com/question/34840297/answer/272185020)
    - [高性能MySQL》](https://book.douban.com/subject/23008813/)
##### MySQL 基础问题
* 常用 SQL 语句
    * 内连接，左连接，全连接
*  mysql 常用数据类型
    * 字符串
    * 数值
    * 日期
##### MySQL的innodb引擎是如何实现MVCC
* 全称是Multi-Version Concurrent Control，即多版本并发控制，在MVCC协议下，每个读操作会看到一个一致性的snapshot，并且可以实现非阻塞的读。MVCC允许数据具有多个版本，这个版本可以是时间戳或者是全局递增的事务ID，在同一个时间点，不同的事务看到的数据是不同的。
* innodb会为每一行添加两个字段，分别表示该行创建的版本和删除的版本，填入的是事务的版本号，这个版本号随着事务的创建不断递增。在repeated read的隔离级别下，具体各种数据库操作的实现：
    * select：满足以下两个条件innodb会返回该行数据：该行的创建版本号小于等于当前版本号，用于保证在select操作之前所有的操作已经执行落地。该行的删除版本号大于当前版本或者为空。删除版本号大于当前版本意味着有一个并发事务将该行删除了。
    * insert：将新插入的行的创建版本号设置为当前系统的版本号。
    * delete：将要删除的行的删除版本号设置为当前系统的版本号。
    * update：不执行原地update，而是转换成insert + delete。将旧行的删除版本号设置为当前版本号，并将新行insert同时设置创建版本号为当前版本号。
* 其中，写操作（insert、delete和update）执行时，需要将系统版本号递增。由于旧数据并不真正的删除，所以必须对这些数据进行清理，innodb会开启一个后台线程执行清理工作，具体的规则是将删除版本号小于当前系统版本的行删除，这个过程叫做purge。通过MVCC很好的实现了事务的隔离性，可以达到repeated read级别，要实现serializable还必须加锁
##### 事务
* ACID 特性
* 四种事务隔离级别
##### 如何解决高并发场景下的插入重复
* 使用数据库的唯一索引
* 使用队列异步写入
* 使用redis等实现分布式锁
##### 乐观锁和悲观锁
    * 悲观：先上锁，再操作，一锁二查三更新
    * 乐观：先修改，更新时发现数据变化就会滚
##### InnoDB 和 MyISAM
##### B树和B+树
##### MySQL 索引
* 索引类型
* 创建索引注意点
* 索引失效情况
##### 聚集索引和非聚集索引
* 聚集和非聚集指：B+树叶节点存的指针还是数据记录
* myISAM 非聚集（指针）innoDB聚集（指针+记录）
##### 排查慢查询
* 缺少索引或者索引不合理，查询慢查询日志
##### 内存缓存（Redis和Memcached)
* 缓存的使用场景
    * 访问热点数据，减少响应时间，提升吞吐量
    * 数据类型：字符串，链表，哈希表，集合set，有序集合
* 缓存使用过程中的坑
    * 缓存穿透
    * 缓存血崩
##### Redis的使用
* 持久化方式：快照方式，AOF方式
* Redis 事务：
* Redis 实现分布式锁：
### 最佳实践
* [Phodal的全栈增长工程师实战](http://growth-in-action.phodal.com/)
#### 编码规范
* PEP8
* Python 之禅
* 了解 dosctring
* 了解类型注解么
* Python 对象的命名规范，例如方法或者类等
* Python 中的注释
* 优雅的给一个函数加注释
* 给变量加注释
* Python 代码缩进中是否支持 Tab 键和空格混用
* 是否可以在一句 import 中导入多个库
* 在给 Py 文件命名的时候需要注意什么
* 例举几个规范 Python 代码风格的工具
#### [正确的流程开发](https://www.zhihu.com/question/300762444/answer/529335326?app=zhihulite&utm_source=zhihu&sign=MTU2MDA2NzMzMzYzNw==&utm_medium=social&utm_oi=758575502888824800&invite_code=7JV2EK)
  1. 用GitHub或类似的现代平台
  2. 平台上设置禁止直接push到主干，所有的修改必须fork后走Pull Request
  3. 启用CI（持续集成），提PR时平台自动执行CI步骤，失败的不能被合并（不准开任何后门）
  4. CI加入linter，确保代码规范；所有代码规范必须要可由linter检测，代码规范/linter配置规则也要针对实践中发现的问题不断补充细化和更新
  5. CI加入单元测试，代码的测试覆盖率至少60%以上，核心模块测试覆盖率必须90%以上；所有发现的bug必须由造成bug的人负责补上单元测试
  6. 每个PR强制要求改动代码行数小于100行，新人要求小于60行，以利code review
  7. 每个PR在CI通过后必须有其他人进行过code review并approve，否则不能被merge，新人的代码必须至少有两人review和approve（比如新人的mentor和相关代码文件或目录的owner）
  8. 针对每个PR自动部署一份到测试环境，方便自测或提供给测试团队进行必要的测试
  9. 每2周检查近期bug，总结经验教训，特别是重复犯的错误一定要建立机制去防范
#### 单元测试
* 单元测试可以防止回归的时候出现问题,一个函数，一个类的逐次开始验证，自底向上测试，易测试的代码往往是高内聚低耦合的。
* [Django测试](https://docs.djangoproject.com/zh-hans/2.2/intro/tutorial05/)
* 单元测试相关的库
  * nose/pytest较为常用
  * mock模块用来模拟替换网络请求
  * coverage 统计测试覆盖率
* 测试用例设计原则：
    * 正常值功能测试
    * 边界值（最大最小，或者最左最右）
    * 异常值（none，空值，非法值）
#### CI/CD工具篇
* [谁才是世界上最好的 CI/CD 工具？](https://mp.weixin.qq.com/s?__biz=MjM5MjAwODM4MA==&mid=2650721534&idx=1&sn=1db6a5f66ee4d6b3d336c082ed04f1e0&chksm=bea6bd2d89d1343be60df41638d0b2992684b1a140d15ee25ac332ab2cbd9708a0fb675fe90a&mpshare=1&scene=1&srcid=#rd)
#### [Git 命令应急手册](https://mp.weixin.qq.com/s?__biz=MzAxOTcxNTIwNQ==&mid=2457914802&idx=1&sn=a8d2cb9b626da84d94d8b2ebd9e85c24&chksm=8cb6a858bbc1214e62feff7028ce6b6e942556e42d5f2edbedb8216a03c0b54fa52ce378256e&mpshare=1&scene=1&srcid=#rd)
#### Docker 篇
* [Docker由浅入深认识](https://mp.weixin.qq.com/s?__biz=MjM5MjAwODM4MA==&mid=2650721530&idx=2&sn=a3e3c68c710fdab2b9cad9f28f25d692&chksm=bea6bd2989d1343f3277ee2ac3ed3f6c39d8d3523ae4e8ae7b797b5ea630bfeb8caf62a3320c&mpshare=1&scene=1&srcid=#rd)
* [用Docker部署一个Web应用](https://zhuanlan.zhihu.com/p/26418829)
### Web 扩展
#### Web安全篇
##### DDos 攻击
* 客户端向服务端发送请求链接数据包，服务端向客户端发送确认数据包，客户端不向服务端发送确认数据包，服务器一直等待来自客户端的确认。
##### XSS 攻击
* XSS 是指恶意攻击者利用网站没有对用户提交数据进行转义处理或者过滤不足的缺点，进而添加一些脚本代码嵌入到 web 页面中去，使别的用户访问都会执行相应的嵌入代码，从而盗取用户资料、利用用户身份进行某种动作或者对访问者进行病毒侵害的一种攻击方式。
* 主要原因：过于信任客户端提交的数据！解决办法：不信任任何客户端提交的数据，只要是客户
端提交的数据就应该先进行相应的过滤处理然后方可进行下一步的操作。
* 反射性 XSS 攻击 (非持久性 XSS 攻击)和持久性 XSS 攻击 (留言板场景)
##### SQL 注入攻击
* SQL 注入就是通过把 SQL 命令插入到 Web 表单提交或输入域名或页面请求的查询字符串，最终达到欺骗服务器执行恶意的 SQL 命令。
* SQL 注入攻击的总体思路：寻找到 SQL 注入的位置，判断服务器类型和后台数据库类型，针对不同的服务器和数据库特点进行 SQL 注入攻击。
##### 加密
* 对称密钥加密是指加密和解密使用同一个密钥的方式，这种方式存在的最大问题就是密钥发送问题，即如何安全地将密钥发给对方；而非对称加密是指使用一对非对称密钥，即公钥和私钥，公钥可以随意发布，但私钥只有自己知道。发送密文的一方使用对方的公钥进行加密处理，对方接收到加密信息后，使用自己的私钥进行解密。
* 由于非对称加密的方式不需要发送用来解密的私钥，所以可以保证安全性；但是和对称加密比起来，它非常的慢，所以我们还是要用对称加密来传送消息，但对称加密所使用的密钥我们可以通过非对称加密的方式发送出去。
* [用于消息验证的hash算法：HMAC](https://www.biaodianfu.com/hmac.html)
![](https://b2.bmp.ovh/imgs/2019/08/a94b2ab7387fe433.png)
#### Nginx篇
* 主要参考
    - [nginx源码分析](https://blog.csdn.net/yusiguyuan/article/category/2091295)
    - [深入浅出搞懂Nginx](https://zhuanlan.zhihu.com/p/34943332)
#### Vue篇
- [Vue](http://yangyi1024.com/2017/05/31/Vue%E6%9C%80%E5%85%A8%E5%AE%9E%E6%88%98%E6%95%99%E7%A8%8B%E7%B3%BB%E5%88%971-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA/)
#### Django篇
* [Django初步使用Celery](http://yshblog.com/blog/163)
* [URL Dispatcher](https://blog.csdn.net/hackerain/article/details/40701099)
* [Class-based View](https://blog.csdn.net/hackerain/article/details/40919789)
##### WSGI、uwsgi、uWSGI 区别
* 主要参考
    * [Web 开发规范 — WSGI](https://blog.csdn.net/Jmilk/article/details/52036911)
* WSGI：全称是Web Server Gateway Interface，WSGI不是服务器，python模块，框架，API或者任何软件，只是一种规范，描述web server如何与web application通信的规范。server和application的规范在[PEP 3333](https://www.python.org/dev/peps/pep-3333/)中有具体描述。要实现WSGI协议，必须同时实现web server和web application，当前运行在WSGI协议之上的web框架有Bottle, Flask, Django。
* uwsgi：与WSGI一样是一种通信协议，是uWSGI服务器的独占协议，用于定义传输信息的类型(type of information)，每一个uwsgi packet前4byte为传输信息类型的描述，与WSGI协议是两种东西，据说该协议是fcgi协议的10倍快。
* uWSGI：是一个web服务器，实现了WSGI协议、uwsgi协议、http协议等。
#### 正则表达式篇
* [可能是最好的正则表达式的教程笔记了吧...](https://juejin.im/post/5b5db5b8e51d4519155720d2)
### 其他
* [优质 Python 播客推荐](https://mp.weixin.qq.com/s?__biz=MzUyOTk2MTcwNg==&mid=2247484132&idx=1&sn=fd88c8c3b993eedb2f5b0b62052476f2&chksm=fa584561cd2fcc777f2c4a268a0dc56bf2df1cdd5242d124ba50285b56e1d37834b620006cdb&mpshare=1&scene=1&srcid=#rd)
* [PYCON CHINA 2019](https://cn.pycon.org/)
* [JetBrains IDE 基本快捷键](https://nextfe.com/jetbrains-ide-shortcuts/)