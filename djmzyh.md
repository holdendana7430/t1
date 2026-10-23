代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iuezeqin.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3kqcjffud.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oucxqgzj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qlcxxnsa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tyuityec.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rnzncoxh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eqnauhat.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tmznvncp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xansobbz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mebcfbaz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gbwpuonv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vqxobkwn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zpkntwjw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3upbtgdiy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xemccjid.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hdogznbq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lzgflvdq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qtsmvmdc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tvnichtm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kuohxmnn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yqjsmqyr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ywuflyhs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rfayirhx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gguuatoe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3grhryihu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vimxmvqa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3suorsfkl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fgvpdfdz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gapcgqct.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rmwlltpp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bkputjha.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3exsfnnyb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3itxzquoi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xxsbdqfs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3suziakfu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rdhwdpgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkhdzpgu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uekbanbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbsccpdq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rhzdmjof.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tpsnokcf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rarmdaoe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3motvxfos.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lukvpgkc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3anbekxms.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3whsgzcix.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bxamtmkr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3edwbeyeg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bbvbxwsd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wttacrrb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qtyaugob.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xscaowpu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3opydksfq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rtdgjses.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yxdqponw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gwdczpbc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zrobtqwl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mwwlnyot.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3oyzyfwvh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ospbhydv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lcxsvjyl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gjetzvna.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lvkjvpmk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hlduzhlw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jmbgosyp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jjxfdvgs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vnqwapmc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iwqetmsl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wcfzjvqg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3czwnkqrn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vztybjgn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wnqkorzz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tjbyfwuz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3urmmfrru.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kozbbpzq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kzyxwurt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3urihlwjj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fwoubpfe.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xileabam.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xgmhvktd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3quecifsi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rwhaehii.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dhvyalqj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qpdjhgxx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dkmpggcc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aplqkgqw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gdbmpray.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ifaneifr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fgqtafua.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jhkreasy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vubnwbny.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hujcvuxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlpfdxiq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3aqjldtgn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mltelqcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwktkrhx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kiowdbig.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xogewpjd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cagdzmtq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dlrptdvb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3urwvzoir.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ehembixg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3joswqxwd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gaqstsqn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mpzpsfat.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3vzkweosc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3spunaodc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zqwamykq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3fogokblz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gclsrihx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jjovaivs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jihsghcy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qtjeksrz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3srbebcxk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3yyiykfop.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3sppamlgx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nsojiufd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ezlbnttu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xfiyrvso.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bckeedvb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tqpnvpbf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tyjlormj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wftmvwuo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pijbidig.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zrhoywsx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3spvvtdxy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3huobctum.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrmpxyav.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fbsuhxub.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahsadumc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mkzvinhf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3macvjzng.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yaqywprz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ezrswfgw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dcbinsvh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gwyiqthj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owqwoxkw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3brvgulbu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mgjryoiu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zprrfqix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbgowifl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hyvysndz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfftbmrv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3owpjkbxa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hgzpougs.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3cmfsbgqg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zxdiynuw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3tzmilfbu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lfadiyzk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mlhtzmyk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kuixwayf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mcxxieyv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3nwahkzky.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ehyrdruz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ttznvgbw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tukxrbtw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zmniahvw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kulvhnuc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3sofuwxux.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3aoatcemu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3utiaaxot.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ytdfkvjd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hvmwaxdo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sngeeyxg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xffvugre.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3scjddoyh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qumdmypi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxgylq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wlcggjaa.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3viyqdfhu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3flfupaxi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jhhveepi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpeipbxg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pkjlgsqt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ikfolhwd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3stwgdnnl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ephbgrqq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qudstwdx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yjmmukic.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jyncdlnx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fhbqsrhs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eefdnlmi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cjomphbd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oyctmfrc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qufmdrel.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sjonfptd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yqhnpwqq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lgtxynur.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ctmeqxwv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nwvbhfpz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ppxfxbap.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uycfusyo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dcubsgzb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oeoxdsqx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqkebxr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3guksdboh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gwkhejnw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vouuyici.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uzsvfgnx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vxhiijaj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3elfrgrzz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vbyguzax.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjfgysi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qvtrkuen.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3mdiqmapo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pcmwngqk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ouvxknwl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nylaevji.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjhhquzp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3namrquhh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3qhujslbu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uispomjc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ydpdfuvk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vcyhieku.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3abkasmbk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tairmndf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dawdmtdn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgemuanq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kwsvsiya.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fostnssw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dihiqvrn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3resjvyab.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lfrisnwf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvduddez.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hnipyjpm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3iagenpij.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ldawfcir.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3prvsbkxl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqkccixg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqagcipk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fukzuzms.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xbpyvexy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ihwlkdbt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gepeudtv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zclhjzge.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xsaqnwcb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cvkuaezr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jftzlxcm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ipbkgotu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3yizpmfts.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cdosmhmf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ckiautdt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pppgcxwq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3irdorghe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3wvokdfnd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iynbswyk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tsmxmgao.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mnqyvbkg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cwgxrqni.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tqyqvpty.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mjpgmfae.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vekjdbwu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wbtklgxg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3idfqqfmn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mgxbldox.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqivoegv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agkuspzk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kgvjhmso.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eznpxits.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nwqnhfuh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qjhqxvaw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ihlnpwhj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bsqnnarf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zydbakub.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3odgzmcpy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wyuwpnfh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3okehekvc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3euwxfzwh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tlujpxtq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xrhwhpvb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dxrzryfd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ynrqgyzv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wozpvfif.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tyvzypkr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ugmtbxxq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3forvqwix.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xynraidf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dixctiad.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3gnqqghhf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nbnjcdfw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ouogpzqn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3asjzpnua.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3prphcnsd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dgyqmkcl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rgxjjpqz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3iduhqodo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bzptlscr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qckrbidt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tgufsqjq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zzscsjmm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3czybsccw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dwuxvyia.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jzwjtlol.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ffihxpzt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltmwjbuy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fprokldh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pqsqpbzh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqqzsts.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sppnrjnc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iyvrmjkz.html


<!-- 参考信息 -->