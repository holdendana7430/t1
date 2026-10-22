代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kvpweqox.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pujvvjyy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2olteihnd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2itbllvyh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sfivljfv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bkjsxmud.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ogtbwses.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xudzzvsr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cpjjnzsf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ejdsftox.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2oexwktjc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2uxqhquxl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lzunsicv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jsyioems.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2opvuufxn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmlnibzq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2grbjxlft.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kxhngsph.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2iodsbgjo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcuwqiuc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sxcsvpmw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2osmnrkxr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uujztzpu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urhxmsce.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2njccabqt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ltqrcyed.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wxrzfbsa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ctvhpqwy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sxjpgfiu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dobvmpyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qpkrpijo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xwkwptkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvgdvjhy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wudqbkln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nznmgwcs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dkmkizmc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xkuxobfz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yxrybfas.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jtysaiid.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hdbneqbb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qxrsgklt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zjkpiknx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tbmzmcjs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zvosiayd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kzuuvctl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2rgmyuhht.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkphny.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zscysxir.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2crevztyq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rqtkxvqq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2opqhocns.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gziwdkkd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vfygnqjt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tstfqnwl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ykkzbjfa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nppwjsst.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gjqccnqc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mxqbxtrx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2atmuptro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vpjospcp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pmbdevoy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yagfaune.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rqszjaqb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jxuwxzbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tnwuvril.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vonzfeaw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wvdlgvts.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2swkelbdd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dituynyn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xxgdlnrq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2srzbvmzq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yecwgvyp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2sjqwtyhs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fifrwkva.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hippeknf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2opsynukt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hevrczep.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kbrvemhk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ejozldij.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dndeosbe.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qqvekhmq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dlvrsxqv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ywkjloip.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2xaspjkzq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2soqtouws.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ciguvexw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yhykvswd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pnfsmgyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzovkcff.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zbldvfej.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tleiztib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjmsuuir.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2szmtfxnq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qjbkkjlk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fzbomdwx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2noffjibg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pikbtknx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gtglaves.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ndgrtqbr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hmzjnzdg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rtamaeuu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tuigssnv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mshwtmzz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2racdgxrb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2evvorbgh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2gfloyxdu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wwrjmznr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2sxthjwud.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2yxdexxqa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wzhsztgm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2svnzhvpt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wxzgqram.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bkdikycv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wwwjnyyz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lrytsygl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzqqmlrv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dcidqywo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gdfamjao.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpxrklcp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xsrrhyas.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqzvieey.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zuuzyhuv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pubikbzc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tkuwyppg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdcclejz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cikzurmp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2znrwuavj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qqjriwdt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bydfaabw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iipryfsn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uugdpxoc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxylgb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pcgcjdhs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2goylgtql.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ftposdly.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2geprypnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kynpyptb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2kgjvdpnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nokagyrj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eremawcv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xgzylmqf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gfdkqqwd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kqqrhjhk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ypqxohcv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2llapuppr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uuuoxwbi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2lrvkfkwl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2slypacwh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2bjkvnjhl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fircclpr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dnorvcac.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wxndayud.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wogsnorj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xjwdaggk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2axvmkjnk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xdmujkhs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2phjpfnob.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mkkpzdib.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ijwmtktz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tmavlbmj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hcaxirlt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tppytcwj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2thazvbgn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vrvwxkmz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cyvlrwrc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ktxfjmnb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yicjllrs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zsdftclz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdwnmvf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zulbruqo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tjwtdgfu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2khrtlawc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ctfjyxxs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hnybegdk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2kpmilnbh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2bzioqiwz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2uathvuto.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lincidnv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xezyywli.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2secrhhpj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gkyrkora.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvobonjf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2irzsqurr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ooocejmc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ftsnxsat.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lkxylhql.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kulrhhhg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2adopplct.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dxsmungf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2amotrvbe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eztworsc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gifqxpax.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2clzuasds.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhutiboq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2tjvkywbh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tsqkvzkt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wtunqtim.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jgifteeg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfcuqyi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ckugsjwz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hpbntkkj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mivhbsrn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qovevsbu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dmwqafid.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hcqdbnkn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fvuidhqv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yhwjcirm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtdsdqi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2flwuclwd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tdbrjcor.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nczkicbd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pzriqkdj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ostsuofy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcxazer.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kaquwedr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmgghuai.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmlyqle.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2pmryykxl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2actmzwyk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2weydtwwf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ckyebkxb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2eilsizwk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2peafkwic.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rstviexz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mvvlepjz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2agtkkvts.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pclurpfp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2poijkksb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qpaolbyy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2tmqruigd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2afpvlmws.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dnejywgs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qrzmdodj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sscuuyxl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2slvmheke.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2beiasyus.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pjltrrcj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cgcurojw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhphbnrz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mhhqjcxo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nywttsdo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hzjcqphy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hllxrdvi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2awmjxnyt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvsjoqs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yudhhyqg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rnolxedn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2bsgqxckk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hkxbtomg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2muzhcppr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bqmoqqnt.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kugjhstr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2josatdor.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tebgxwlp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ahwsgppl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qnlgbiyh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jjkpwgab.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2julokdkj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ngatjvkf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wcyfmgtf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kfnbgjgn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wxjtvnel.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ddfpbnhq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mtjoprvb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2anktbszq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pztzugvo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gvppnzil.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ukpgsvru.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qmeamttk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2loafgxlz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2sfzjvllg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vzwmdzrv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wnzmkfvd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2olsnlbfl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kzubybnf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2chvolwgk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ovicslol.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jcfomzwb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hnexiyps.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggawdkdk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qxmbogyg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2witqunst.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2skgwzoro.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2orrywovc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebvfxflu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttkatrok.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2noapssph.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhldibws.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qutclvss.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tvaqelxs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nzdcntkm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwryujqe.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dksxfzqy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dwpmnttt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcsvjdj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfbfthb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ckfgqxqa.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2elicentc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2hptjhyef.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kjvpvhlh.html


<!-- 参考信息 -->