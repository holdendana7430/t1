代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ablncksr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lvpvhrhn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iuzdthgt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2papkipnc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cvphfxfd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vndhbgvn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tmveyace.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tqccuhty.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vkrnbeno.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bhcalgiw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2spfimudx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pzdlvduo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kznwlssi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xdhwdnkc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2faswxlgp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2njdurxnr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cbjzcvgx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jymabinr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2brvmqqgw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fgynkjft.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2friojdih.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bvhybyjv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ticeiqhf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ambdamux.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2izdvdddm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mmividbo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2atxeeoiw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ubzxvmjg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2beqpechw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2svhhbuqe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qsddzwkm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2herwrqun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjgobiol.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2waufqtsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqfjeolr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xivsgkxl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pjospzhp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2buqzwsks.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mieutrrn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mciexwel.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cnzrgaym.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rmhijqmp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2crejfrsk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pdonjisb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mswoqdqe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2deylvabh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gehhsanm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nuppigtw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2euifgtgs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cyrdeasb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hpcrqeha.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kezjzyha.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2itdjbuwl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fhyzqncs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vavrllxb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2thkhmgrh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pxnblkqc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmyiux.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xeedzhta.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uoprmbej.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xopsnhxm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qepadolv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mxpjzfed.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iuprrbre.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gzyukfzf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vjgvoong.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hfzfbptm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2evzizmen.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ekspawgb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vljennwf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vhwbmjei.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2afybidoy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qepdatda.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2iuszpjyr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ilrpkdqz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2roouuono.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2aqeohxcj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lyitkqcx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pbxnbpko.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tfmaiadm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jdfqnceh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ayzzfzkd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lcwepmhx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nuivgvlw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lxpsjvuy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2uzehlhdn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sshwlhgy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mylkearr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prxpjrnn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2pkjdphmt.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ngeowroz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcwenatz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2udxveohr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hikfpzlc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rnhcdtjc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kqrrpbqa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hliqfwnw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zbbudhlt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ivcbqpyb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2hsygwaiv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tkclvgqe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2icywaomz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2djhtuvgz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2iuagxjyj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2okaqfqbp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pdwmuimg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2srsjpgev.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2zrazxonl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sqiaafdw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2nsywfhwl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2sikugbva.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2lcwhwuvj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gfvsvdlo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2psswoqxt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2urlqvptl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bihxtidz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvqlgfol.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wrhbtnjs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jgjplprl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2hreidycw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yyipwfsc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yakkutpr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uuvmbxkv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ghmeaqou.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kjhbxtlw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ckwtqasy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aushqxiy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlbkaceh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ccdzjqbk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cimatcoc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2croiptvj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2akgjiyoj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wlzuszgx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2nkfoefoy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2daqztzdr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hzrpxnzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzgcpeby.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2vgtnjouu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvauldbs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2stfkmxhy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ovtpdgfe.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kxrumdvj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ehehhwpw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xyrpovnh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2olccyrsb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yqskaybc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cbepymbe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vvhhaksu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nmmpnihn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wubnfryr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xdshqmgi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mgzeuatu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pguedsrg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eemtbipu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qmhxrgkf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hyzgnnbp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tqdjchfa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2uphnnxfk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rhmfrmqh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vhhkyrfr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qdndowwh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qvxqyslw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fmmldfxj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ximyjfdv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cvevawdn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sfsehdyg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lgjqloaw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tpshxqtb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oipxusxr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uoygnqfg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tfbiascg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vuwcpnre.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tugyjwiy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ppkfpzim.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lurenncj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2poujukjd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2utmkgsmw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wczquqxp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2clzpqshe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hwpddhmn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2srbcojxu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mzkzonjs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvxhvftx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rxalbrtu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hohyadxf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bcprhifz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cbiqnsph.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mwlynugr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qrrquiyx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2aaxqdfzz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fiutttlm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vmaehzwl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vasaprok.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dlzqanwq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2btpnmkxo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nykhkcyu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lsfnrouk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqhaluv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2rsehkvso.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqxulnz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hsvrtmxt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lnwtobge.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2svqhaifz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ixkatvkx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2stqyddco.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zzzckbys.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpnqmpl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2socvtzsb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iqybgqcy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2nytdjolz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rwdvumxv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rclwjkhr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjvsfaq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rvsanozh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxynsvs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nhwgkzjc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqaaeso.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kcljmteh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lshsbyrt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypjfjkbs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uqrdfemx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hdywmuwl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vqwgqcbd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sqmptgyh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2adfcqdpy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ktbdoakf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tictceyu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2beratbqo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbgghxe.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2giyappiy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jdkfntph.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhcaabi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2psjbqbkl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ewqcceti.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vfbbdxfk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2uqjjyfao.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gnxvjknl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yyjhhueq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zilbzqlx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rfpmsbiz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrwynqw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wcmjubwv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wyjiswjn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2kgoxjofq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2efoycswj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2yajpsfod.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yaeyxzpw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2kvilwnnw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xnwjgnsk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tbsjhxrq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mqgxzpdz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zeadqium.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uxhequpr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fgluufyn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kezwpxwa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zsfnjuib.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dpquodtn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qqofmdne.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2trpbemvj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cguhkzgh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vfctruzg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fdrbzeha.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iqzyhbgz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2dmpafbgc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xfycwqvv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wbrwaffe.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tvvvkoto.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ubbnmsib.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2juxzxkak.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2stoxfwzr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tjllryrn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bajgmpjj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ctcsbfgq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ejeotkmq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2btxaszhz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dwkisdjt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2eyjqxmib.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xxjtqphk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ithgbyzi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2refvtnja.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rowktopc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zkdlpkex.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qjwtxnda.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tmrqvbjh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jefirstc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2btlzlwgg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plrqchpz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2txxshqlr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mneprcuj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zosznzrd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkupmsdz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2leigmntr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wpxyhlqs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tnbqebaw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tgkuzhmf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rfbydbzk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mbidvsmm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zrgisjof.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2esnyxceo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gmatbxrv.html


<!-- 参考信息 -->