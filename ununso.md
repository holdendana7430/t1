代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fdolsfmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbguqfnf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jhdwxhus.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rwbetgmv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dyqzszeo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vqusfmnw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hjdyeuey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3exuvazsc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ppkphsow.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3szlqdwyv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3flpkenvd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rnceqpln.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nfqplkls.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3sqokkdft.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rlpfshtj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ufzkwzts.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mhxfglsw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jhddsjbc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gczearlc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqnyioj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kkfilbsq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sjjrljpa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3deizkbjm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etnwaecb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pnzmcctg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3uuhhwyvd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mujpwsfx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pzdqwkbb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3svgdmmxx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lydkprps.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jtgvsqcy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lyofwufe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iooohuur.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mmztjwno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmvxqsyo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gshjhbrp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cbutmtpo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3osqwnahp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kejlchcm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3iqgipxer.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sjizrprf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xylhzsoz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3elgbmnyb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3onxhnlpb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rgqdpvvw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vezgplcm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3smtzeeij.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zvtpkmma.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yxtijldi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qlgxyndw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fkcilyfa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nqwdfocc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ilphvpvv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xwqukkmm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ydkahgji.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bavjntrt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3herzqpns.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mvqudmuf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ozhczlxo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xscdgqci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hnnevszj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3forfqayr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3utlhqkhe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kmdlnohg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gbflmtyc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wthfttqg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zgnddjjb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zebwhgto.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vixjvfii.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gkbijkni.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3xvnzfhqc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lxgufaaa.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3flspgivt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3izktzpwz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ezoxkbzs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3shpijxpr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3thtlbdzq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ciukvhey.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xsbpewcv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fedaxohw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kituhwvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tdmphlbl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hswvejis.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bjefnluq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3yckzyeqn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3nuuaugrf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3alimehnn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3iyagpjuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iexuokfy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3jqqejirq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3kgdjtytt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwxgmcvs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pgdiephg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sirbunea.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ahvipcug.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xakqqops.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3loxmymqn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3uiltpzug.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rwkrocrx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vixsvcko.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3copzphpt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pmzmookg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ipwcirjv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jgzakhoy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3iexrpjxo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vnffobzp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3avvfnlnb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nrmmimdk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xtnetyzg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3omcibrxk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jtimaihs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3aptvfqpx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3chepluyu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jbgbvoyv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fjicgtke.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ayumquuq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqwzwkxa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwrnxfcx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3emvyjdlr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olazxdbc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ffhzeyzq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jvsdzzoz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xqlelctb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bqncuxrd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xghhdtpu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imkalllc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qskwjpfq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uuiyhqse.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xosrjodv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pupsggxy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fftosnhw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3humdpvwd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3riwshrrq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skhlzwjm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3snddflvh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfwanonl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfnwowho.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3iejbfmgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvfofqsi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3idusgtqn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3decazaqz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mxiztunj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mbgtjekw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3erwmmeou.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kpgptqkj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbdequq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xiuuzgxc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cxjnwcrw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3iqvdmjwn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jburxhja.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qohglftw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fksocvrw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ccguoyce.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qdgmedjl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uxkqmuwu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ttbbqciy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rdfupppb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lvycysnk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hddsijmp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqvtohr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jdqkzmyl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gliwntrn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3chnroffe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wekdolry.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mmsdjglv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mtldtdaq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pirkiteb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dusodzcn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zgicsobx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lvrhwpmc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3oomwikbz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mslbhcap.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3olgtkcue.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3iofbilsa.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ameyqobf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3stpvabtw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3skfsoavz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3otshiyvd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kowbennr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lqwkgkch.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svgrhwgo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jvklbzzl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkqdgxqm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ynjnvoft.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kygwyiss.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zqtvmqsn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgfcgfy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vrwvoitx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3byxbpcfd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xsvbutss.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3hapopucn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3soowapot.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vmfkbnvw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fnektlfa.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hqgymiuv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkcbdky.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3laruonjh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3canqlfds.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rwgcxgld.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmqayyf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qzvqrvgl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kxkaezyx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3puumnslc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3afmyuywx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3llroewxf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnjqgri.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3icldujxx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnfgxde.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3veysoump.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xbscjaks.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xtymebyc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ooufehnt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvlfxth.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wyffrcem.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhokgtcc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrgomcf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysguokbw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3byeqohgz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ymbnkzzn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cotlfthv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3szgpkwrw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tukrxcwp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3brloqibu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hmwerfuy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3judtlvbb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3urfnxchu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3chtdaxwe.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3eoglnazo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mqloorbu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ieqcwbnm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eerbinkb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fbzqwivh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3boccydqi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wpuclapi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hkzlqcqs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ytjexrzt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jzlgqexk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3atmkjvpl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rpvwuujl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3htgtnwkt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3znhgduvw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zuotuhej.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lrchvqnu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrvelhm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgmpboe.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3otiumxaa.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uijpljri.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dquaiith.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aqobymmy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nzwyxzjl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pekpeegx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3czbnhubv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sfiagnsx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3epiadsus.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kunluchi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mcozqkot.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fexmxsmh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fjdudomi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sasawgkf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mquhyovx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ozezzwfi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wxvnwhwh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uggxxine.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yqpgtybo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wgcndpda.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gmeovdlk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dqdwnptr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3stwazcra.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nbfogfna.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gnlxyoob.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zjnpwyky.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgtcrew.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ekgzfpwj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ekrwlufn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bzuhrqfv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3vlslbwiy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ppzbqhxc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ctamqbpw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3khgedpjc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3anijdrdt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3shkzmlnr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vxcunfhd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyrkaawm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tnhuwdus.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltwafwii.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3evgnzicg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3homcyxpe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3chvkvrnt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hshkbcig.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3abnihrte.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxokjnjf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aiiysgan.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wpslaiae.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rhondikh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oklkbamv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ufiwsgpg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mkdxeooj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3irwpffjw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hptoboox.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vrbjueac.html


<!-- 参考信息 -->