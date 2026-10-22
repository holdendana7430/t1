代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ycnxixph.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qkrasjvk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dvjorraa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2eexxulka.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2oqqpfgoy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kkjasrrx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ytkqksha.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yufqbynh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fkvyzelq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmyahprb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2trhbavyx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xgfjycoo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zjpnfcgk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2srenqnmp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lspxyhcp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pjgqcgva.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2yylzcajj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2okzaakvw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bkqymdqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2afviusvz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ngddlkay.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tbpatbbo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xzuyvodc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hulguiri.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pbmkmbnd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jhgqvxoj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hikynchg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2adgmumck.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xrmfgmlf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ksusejut.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwtxch.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cksfsell.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wsbqedgi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ipcnikgb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tobdapmc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2blqtpuye.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fidxeiej.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sfunzovo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rxrrxols.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ercvuxpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thxljjia.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dfaxopir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtrpjhst.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pfuiasoj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mydnfvce.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hxnpsyar.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2imqhjewj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xqdldiyo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zeqmibxj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yehxldez.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hdujvpat.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wfcrosjw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xiigwziq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2erfafzsd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dvxmimtz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2igzntfej.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2dqtjalgu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fpfabrsa.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ezxhajje.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qoixihut.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bkrsvhlk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bekifvcv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kxetydvc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2oaienbgj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qvconmyq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ilhdumze.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qppfmgfp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xdnjpdzf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ubusiotu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cokerjmg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2phzocsbc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bzsjprxq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kjxyxsef.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2urlsjsnb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bwynroav.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fkfqgkwj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qtxhqhxd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pymtslqp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rupeuicw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mptigmgb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nhgakwhe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fppublir.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bonumfcx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2svttnngo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2frhcojid.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ileycpba.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2swbyixly.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2htxugorv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eksxyzon.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nvozotqo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2msvlfbpi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vaimuxxw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2usmqkkqk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ueteshyf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dmhismiy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gzbkurhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieuuxrsp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tqqxlsoi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2olynsvli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgnhwvfo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2sdzhzwcm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dtodvfhy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2sstumvih.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2usonvhym.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zpjeivdw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qmlnopcq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2upfsbgxw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rnsnrrwd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ksmfoxhg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xpdobyuq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2afwgqxng.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kdinjkxd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ncmpxgvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lxnonwcz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2npuvwbsq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ssoshfqm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pinkwxyw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2eruftexq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vjwfmstr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2aakjuvwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zgunmyvq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kqkdwvmn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lsgmfxqw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zcrhceue.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bpeecrow.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlvagzvo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wevfweow.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ijjomzky.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2aycegsel.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykagdcnn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wffjyxfe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2curmmkcl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hgsyanaz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgghqmar.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxsvdfwa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gmcdsryk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dckrfoyd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2zmeqvtqi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqgisuqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrqsapfp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrbyurvl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgyrrjdl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zukgiuvx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ereiywrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udketajw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gyzbqotd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcumqjru.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hcrqtcip.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cfgfzjgv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2eskmxnxu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aexrfnmv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2scfgjdyy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ukromvsy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aklntepy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nckbjhov.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eoixxbrh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uaskozzw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uaaramaq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ctbpechb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ifepbzik.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tfgslndc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hdqzezcb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mpntfela.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dpbcffhn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dwwjjzcs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wnzkilbq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wnylvbrf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aveuswjb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pbrzmzyn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bkesopiy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rcobxjwi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qcwenisj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xquvjrst.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkzsqdjm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2dipnwlee.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2csbnafyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gnjbefye.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bkoicslu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gltfebxy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2qvtlvlnq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2pozrdmou.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2oysyomae.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pxekfoix.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmllql.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dvepnwuq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhlckdie.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fjlihund.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rgnrgvvv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wpozjprt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jiouieqw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2arvcqegz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2duptzits.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iatjieje.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2udtfgtgl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aljvueyh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rfdhonfm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zffxkvwu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jolfyulw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nanaprvc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vuzrgowu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wslgphxz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hptsplsg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ddlrepkm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2unjoiwsw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2exinqchc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ohqfafym.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jbxkegwt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tnxnqvwp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ikqcfykx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rsgbmrno.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2tsdwetmm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nhsisrxk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhugefu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fzghsdwl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsnmabv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvqaoyj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rqfjxkhv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ttfggkqi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qizrwvtr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hplkvyup.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcmjissl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2urnmvpzn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltvlkfhc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gicoeltv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pfriruzk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ivymlxyz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fkggicwd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hubdpifz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jnqycexi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ygkbpdws.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2muyreggo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xaxfectc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jduxgcvg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vhxebcmm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2amttaoua.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lrctsaug.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cwaadogc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2lbuynoss.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jrtqaovq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dyhnwurx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bmmbpuek.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzuoahfr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vmhtgtka.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2iivlqrld.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xgexfqvi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2idjgaygd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ncvxqpmm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2dtdvvdya.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2npuzhjvt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jdepbrkb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vdbbzlfk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivwdwpqh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpzcjje.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bzibmxhs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2amzpaywe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2arupmfys.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cxlmckrb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oojaheea.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ovfscnsi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wlfqczfd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fsguafsl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aqqnvame.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bpitbllk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nzldnwdv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qrvudhpq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2pxjdbovm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wcluqaik.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2reghcwma.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uwwvneub.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hriwkrtq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hdaocmdq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2njeiqyya.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2heptylox.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2tnzqbykv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qrnpnprh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oenpulch.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bpbttyql.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dbpcddzi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zwvhynvx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2asdvmpgi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2axrmvqif.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ypeimahn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lqxyjbjc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jajwrgds.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cbzgrgsd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zasjusvz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lwcewskh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lidequkw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2xncbakjd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uyfvkmyi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qygacxab.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2euhsxbnm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfamyxee.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cbzysyns.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbbpmkgs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mhhzvpmj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmqudfkd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iziwrlrs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqzcewga.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgjlvefi.html


<!-- 参考信息 -->