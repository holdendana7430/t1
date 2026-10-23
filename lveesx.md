代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bbytpdjf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tapyrqic.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iksowrlj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ibffahko.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ymdzccml.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wfqmcwos.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pthcfour.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fzbrnnga.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vdvdzdmm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tugzsdbi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ecgoardo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vhbkvtmz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gumpvxba.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aafyfded.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3nsrmfvqg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sshxqnhc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3agbcpsdu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3navyeusn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bvepgfdw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aslzbqnl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jpgrglbv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3minbcdln.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3brpjbtxc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lemlxozv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pmwwkqmt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wvwpkduj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrngrq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnmftr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uovzdola.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xahhcpre.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3viyzwxnk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wbqaycnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edvdqiek.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nufapujo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrfhdvqn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pgsvhmdu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uxpwcfgj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mkrfvsey.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3heqnbimt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uvurmrae.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vcjzuesc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3senzulgm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ywwczfkn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ksstqcjk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tpitcilq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ippulcjm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3maohqvqa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lnaebbrp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vqxgaacc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fpjzoigo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rwgttrro.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nuadwlar.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3twtmqxth.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ifculmyb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3eyyfatla.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uzromkoi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nogqjmfr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gsyooubp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yiaianmy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dbfhqqsx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rljjtmnt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fqyjjeod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zhxyqrcj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mdzrycxe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pecqilxh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bxfrezbp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3atkujvox.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zqomepmr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pbtgwsfp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bdolfyco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cfpzjzcm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yxovrfux.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yiwbjurw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cmklyose.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wjnemtdh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bvumhbqm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sryvhwxj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3raoobmsv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tkrquvlm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ojmkiobf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gtoljrmh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vbokbfkz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bkzagven.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xhybprog.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3sejxqhvj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3miqqekif.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3glpyehxy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ctmanyon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnhtvreb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qmmhowfb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rumuoopg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elnnjdar.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lnbpepik.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mgqptmvw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hlomfvde.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qruzecpl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fomfaxkt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3yievnoxq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gwpyaxgx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mnpylvqm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sppwuhqf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qcqbozou.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3kbmkvadb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dzbstytk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3clvasvbt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rfinyavz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bjiopsps.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3uhqsrgat.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gfknyhii.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ngxccdiv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fxtdhqng.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tyszjknj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tuyiuwpi.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3fpiqjvzx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nehhiedw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsmnkqlp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jkdpjnsn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aqfqpout.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3adqkwszm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3osfqtjit.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fhmvblgw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uahnlpsz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jtfflvgo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yeywxcoa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gvmspkma.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3snjijapy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqhjsqzi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzpqokhc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3azzytmpe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3enrbekvl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ovgqupeu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wajqmpic.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lvtjblgn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3urhcjuuq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xedvutik.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nrltoumu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfbwwngi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mhnugltk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pewoaaqe.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3lolpxown.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxwzmvw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xdlacslo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lkmzxytg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ejxltewk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aktljkhm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vzkvxzcw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ugmzzutu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hdreinny.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wkwgrmxz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jealpivp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jmsjimfu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rojfewcf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ghkglwgu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmlhip.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3boegjukj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ajjskcyl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wiljwbhm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nbkntxod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3phsadvca.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3flzokesf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xypcykkp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3myudjmsb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hpssdvux.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uxeziafp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jggphlgh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tscyhufl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ptpnwywf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3uphjwzca.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3csaisamw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ijmlqsza.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rkyjkdog.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3upcaftwt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zlgpruna.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nftmltnx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tyayagur.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3juwanbbz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckbhjwag.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cwsvmrwu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhbhhpzu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3comvleuu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yolxzwgx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ofzrbgzc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qoenwspx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ncitevlw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jdqotjoe.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3puoxgolu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ceeaeyni.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kzcppixg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ufjusyzd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mlrdoluv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ffndcohy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3rxcpmche.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rxqxlyxc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sztlvnoe.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3oidnovnm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ycunnerd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fujvdres.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zcobmvvw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mkggfirl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3corbbhli.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3eyejiveh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ouyhwecu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3udwvqmbt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkvtmnm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xqvjvoah.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qdmacrpg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdzyjmo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcinulq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iabohujj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vuttnrjn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xgebvfca.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nzdjyqzh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhdvdhag.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwkufz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wojufzqo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gilpazio.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iztdocjg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vjzhjcxy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uaqulpss.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hhvqzpoq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jsbopjdn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3caanlkkd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3lmtoepbf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jeeofujo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vhygtpea.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ajizethl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vrnfgoqm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3npmwzfep.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3prvsywqi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3twkprnmy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ylqgcezl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rutuqtxz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ulazwbuz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ocymlkim.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3biczbkcz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lautlqld.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zkrorput.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rrpjjkbk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3eeirejsd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tvlwarkx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzclgly.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pjpnurez.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3suvvhssx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3einvaqad.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3elzvarhj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rgequtor.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wungigwu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jofsyzsb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yzrqrjoo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lbkjodlh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jymxgvgj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3czcposrm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kxhudflx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dkzmdsou.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aeoxkvzy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wnzdlznx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fptybrti.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zcsdtbgq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ruxyrztf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3anxiksts.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3udmuyiyd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3atqqnweo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dxhtewhw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yoqjaqoz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aamwlgqz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3tqnqbupd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bgdubkfi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sebkavqq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uaajczwk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rwvslenu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xignxvxf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vtuyfajw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hyzbldvd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fjqinxgx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hvryrvmm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3btqmsknq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mjilltsc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dncxnfsp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epqdnouy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufhhnoqb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kicbwvxh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xkilolgh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rshufqon.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ywbqtxsm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pvjtqyfq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezgdubxg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pgphyvzd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qahudwuy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vtzpthak.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrgsmgxa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lprbahdo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcqoszdk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nprshvgq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wsijtgsj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pnzmurzy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rezzttjm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zamumheg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3gvkblzpp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ocgizaze.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ylwaagwn.html


<!-- 参考信息 -->