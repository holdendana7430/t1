代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yptwhvbs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dttlydpt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mnoaluhk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ixainapm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vfllfcei.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2okwpxlxz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mivpwxvt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xszbsveq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2aknmjbaf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hgsquojk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fbfiuykq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qepobebe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kkrfyvmx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gncuyvbv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kugodcqr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zmeuhxvc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2oxmmhbyh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2srzklyhs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ufegndpf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cqpuiasn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ufkdynxs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xmvrwtqk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aegomaby.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vedgnvip.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2umbzhnpn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zjfrggrt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2eryeagci.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jlvyosmi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2odmddkvf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yterwunv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rxgpftgb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bctmokla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaharlmg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nlvimgou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxwnxlhd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yyvovmnj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yntlfkfv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2efwbayoo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vurwnrle.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tfdhsunh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2smipoqmb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yxbaltog.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yvwswggh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mdqkspjc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2olkbasjk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mxtnmxlm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jsngijin.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2swsnyoci.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2etgajncj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qfwppkml.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xesirggq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ptjhybjo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dycjvwjj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nnsmyxkz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lgcuyeag.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gqqwbebg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qrzvmtbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ayfbyaqn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hencqtzp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rsuwfacl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vtluvcrv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lguebuhm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tqnsjlaj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fjvettpr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aeleacvm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wiejycvr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pniaeikp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2twdrlbbk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vpwnqyoj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2adhhvmxf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2smetrjjj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fnzkbwyw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2rorafnjb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gerxsdyx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fahxumwq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lnnsioss.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2tkdxrwmh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uurotrbt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xjjygeve.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zmgygyzm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mnsjmhni.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pkttsbts.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mfxxuspb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hpsvigns.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kbnwbyfk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2gotnyzmk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xvjvqmxn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ouqkufgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvoxmhvd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ndymstbg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2shuklral.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbcujglz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zuqmfbko.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ahylfkfs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2icmenuls.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xahymiei.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2udcxxupj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lxfmkwze.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vkeebkkn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tqfkgzti.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rcahxzur.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gfangnnb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2olgctrun.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rmdnonba.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xuuugwwd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mmlfaylv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lztkcemb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2edeuyjgr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tynmeawp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2thbdlaiy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nchsrulv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2suhaljxp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cqfaahse.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2betvvytt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ptfvdxwl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2otmtsbdf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2niaeavwa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkrjltpy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hbugqelg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nboplkwl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wtktxylj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2udebbvhn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbovehbv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbnhzhwk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmutfwlw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bzstwycf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2udnnlwbh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eydttwnz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2omvfrvvy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etmffqla.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ategllha.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfhjpoea.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dgurwfwg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2gwdsobkb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yxxtoddj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dsfuggho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hesylxhp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2pxjomevy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhisfzvs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2pawulbjv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hxhvtmnt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mwextmiq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bbsefued.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2poogysak.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bvzhaafk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2npsxlaxk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zxhjbqzw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mejgbdvi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2htbotdgk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vidltptc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ofbqsjlk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dmozaagq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvieoti.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kzihibvy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qiijgohw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2asfrxzkv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ekugvfjj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pzwoahsk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2khdxrmxq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sbyyupya.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wkfoyncd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqdwpp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gdblbckn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qihctzee.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jhmgndud.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pzftpvye.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qolhefsb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2gxvfpyyd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhtgdjw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xhrqjnrm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bpjdmnvd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tchkjzev.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hdzvlmma.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2sgjuudgw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wjpbhphc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qvjfftgc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jaigtaul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uyheeefe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bvgxnukz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhqnzbmb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ipthnzge.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pinltpdt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfcjcatc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2amxmqean.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uwdepyfv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zzhlszua.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mgocoavn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hyjvkmoq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fhmhfzdx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uzmbhbqv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2odzcsjkt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2euylcyog.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2juiukyht.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2edqpijpz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjvtbih.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gklcuwku.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ttgjeuin.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ugfdyqax.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2uulgxodl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2trfhrafn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bqzdogix.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ldiicwjs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ondrjmjz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2olguznog.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2iaamzwrp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ocioltil.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rvwbwybj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2odrgtidk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zilaeank.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2oloqchoe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aifakwkp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yiuawdas.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyitrxta.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yeiyulgk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynpntbpn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxwwsuy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vjyxsbke.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cxjvyxat.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rmynuopl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqvhwitw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2asmprrzf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2spwnaccw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zvnphvig.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqwcumhi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rgiingma.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oeegyaxu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgpayz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2cohhouin.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgahklr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hklwmttd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2iolufyts.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bwmbhhxw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tqqspfbc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cinopmjd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2laxpkkch.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2fsxnvjkv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dcijdegc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ritvioxa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2keguapft.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jbdhvaxa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rbykjifp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yuizeewk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dnfysotv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2empgfqap.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lidvztlw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wrdculth.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jhsrwwux.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ppqerazk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dakauzls.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gfaugrqy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sffbfugi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rfphrxrb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bagwqvcb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mowotypx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uqrjvrcw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kphlgama.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fjfgrrfg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xgajxctg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eywmfhmi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tcetepdy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nvywmmbe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ykykoevt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2geargccw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2drjtmbss.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cdcqdewn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sjhaqlgl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ownsfyic.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fxghtoub.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2emzjygog.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ccpbqyju.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2vjbtsjhq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2tdzuhocz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pvkarznk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2buhhdwez.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ztiokzig.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vedjwhbk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2azgfxrxw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2cleppmsb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glkxhsdv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lmkwessf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnedfrai.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xaryfurv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mejkfhgj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2yhtjqwfz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2brsckubk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sytocacd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2solvvxcf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pafgovip.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ujapcrdd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkubhsai.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fipovdwq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oolnjrlr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2eqkanjyc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2elmigcaj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zrivtiio.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2usdpcyoc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bsvyfalh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zbibtqye.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ncpgajnc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dpfypagf.html


<!-- 参考信息 -->