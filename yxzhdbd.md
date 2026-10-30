代发 wailian999

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gzolowrnz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gqfiouelm.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gowpqglyn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gwymvbdpg.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gckwnxzhf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gpaunslzh.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gecoadwzi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/grglaradx.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gtyegpvje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/goziayezf.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gzpsvgrbk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gdzhdtfmp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gdqwcrtni.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gwovqjofe.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gbqdvirvs.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsodciclt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gitcnofct.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtenjddqf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gppszvjfx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gjizaukxy.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gcwkjcbht.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/glxvyklkk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gwttwiopg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gsigkrivq.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gzopvgqfj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gubsxlqvr.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gnbcwqeyw.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gsabrgycx.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/ghygvprlt.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/glgefnffr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/ghacmuvcf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gqxuzzdoa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gclpxbjgm.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gwifutuwh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjcqqxuxg.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gjznhvkiq.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/giimiaizw.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/ghieensww.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gpceadbko.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gdnwduurr.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gimjkppru.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gggsqbjyu.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gcvzxnfjt.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gjnfqqfkl.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gszxvfceh.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gerfkvlct.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/ggrqcdtiw.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gwbthmwqw.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/ggsxlwqub.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/ghxnogzqc.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gdiowjtmb.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gdhecmarp.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gpihrtsed.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjbufmsqy.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfugopoya.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gpnfgxuzk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gztdupwey.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gyvmhiuoz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gaiekrzos.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gyjnqwmsm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gxaqbvwxn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gnlvkikuj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gceayatxv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/ghxhsusqb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjpcwermk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gdtsluohr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwzttnyik.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gvwuzpjbx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gpuvbcxeg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gcanaxxfn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gwlfptfkd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdaunkwrg.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/ghddaqloy.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gfmtbxcux.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/ggdfwzbdn.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gkcxwcxyt.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/giilcgawl.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gofzcrwln.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/giwmdayww.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gxshstttu.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/ghyrtmqoe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnglssovg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/ghgauybsu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gfrebfktq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gjppeqfad.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gfbpzqkvy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/ghgzqhqio.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gqvmprqba.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxaslrbdy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gtteawiaw.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gwfwnkxml.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzuzvrofs.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gdemcauwg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gjndlwfwn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gbcpohpzx.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gnsqkfofa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gkfvgorje.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gmtsllcdi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gjxxgwobk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gqxeesgqh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gqppqcisz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/guvaqezzi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gobdigilt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gsncawytm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gshpxeyxk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gkhiwnvid.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gpclrsrah.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqsapev.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gmkputnsa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gizqdotbs.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/guaifsfgr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gpgdwiewd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gcumjlpag.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/ghevmiqjf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gezlmmpii.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/grruhxgmd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gjxuuhomn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtyvwlhyi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gnzgufolt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gufutkzjr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbeowlvpr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gfnolqyms.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gzrjzwbws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gpsprmebh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gkslnckcd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggbmodyhd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gfeomybik.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gmbrrhkri.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gxsaqwwce.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gjactuqfp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gtqbupfrl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gzgckaozz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggsfdrkuy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gxdohsemi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/guffcrwly.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gldciogyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyabatmrj.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gxkloeikr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwyxbrhqq.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbtspxzef.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gybocsjtt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gapmgfljk.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gvdlhvmwl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/ghrswtqgn.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gexpmzshc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/guqprnedk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/garemltgo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gxepzxigf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gpffufljp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gespfnugn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwxczuhxf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gteezppch.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gjcsxmmap.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gdhiopdtc.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gznnzkyup.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gmbmpfbnr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwdkqfzda.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gxwymkkcz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/guaphjklt.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/garsflkfy.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfvrrqdrg.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjoybwnyc.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gqmpjhvzs.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gbeymllnj.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gsjhdzjie.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxvzofxua.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqjxedaso.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/godhcraxb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gorlzhewn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gdrfufwwe.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gwqljxdel.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gncosdyjf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gdhhnszbj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gefzklzns.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gfrdsqusf.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gslvzkjnh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gdfjxgval.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gapvybema.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gklazeoii.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gojmxlzox.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gndzcehde.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gpgcjqzhj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gwdsqjnmo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gfnwmrpab.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gnuobbklw.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gnffccdex.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gtuwabsdb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gvawtumbp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gxcntreoh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/ghgrfnsoq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gyncenbza.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gwfvcemdp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/grwupaqji.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/geqjqmxcl.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gbjmfhlfr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/guxmxubyz.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gerojxpli.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/graqidzmu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gztnupmze.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gxyiavucy.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/graxravfy.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gsignykda.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gdknosrvw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gdobuqflm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gncnbxrii.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtiwynaxi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gruenmzvm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gkbbrhznj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gnqznicks.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gfeujucvt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gbdmpfpsr.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gbufjdeus.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtwkqcecr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gsssxzpuc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqvjwfcoo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/glrcxsuqc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gexfxvpuw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gqtwkcgpi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gsquedjla.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gyzwtatep.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gkkgpzbdc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gxuwmezwr.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/glpbuerls.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gmncvzxfv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gjkewxqfj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/grcmkjjtw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gldnpgdkg.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/ghfygosmy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gefeohjpp.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gbxfommmc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/glabssmdj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ggzlbhlwd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gctwoffec.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gxxrjfwcw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gdsfuzitg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gxdmdndmi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gzklzexqe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gbgizfsji.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gqgvtngjv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/ghtivxxun.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gnynllwmn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gkanehuzj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gpifhafiw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/gsbpmauwg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gilkbnymv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/ggscykzcn.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gpcbxkbpg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gsmhevxix.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ghtnipelz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/giwkmhegv.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gybhcrkky.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gdbzclaeb.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gvmwasflh.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxyoiuukr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gwjoyvjip.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gzvikxsmu.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/glwttghkl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/giqlujkdk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gteggzsty.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gxamwzonw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gfabpybtt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gnimihxop.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gqloceeya.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gizjspqbx.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gcvqonvru.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gojllsxgb.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gbmlghlkn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/ggojqamlk.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gwslgwgtd.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gjfjzeidb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gmdvmfsoj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/gquvzedct.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gptdjdgzf.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gjblgbmag.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/glhcjmpkx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gozhtgigl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/giieerwmh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gwwsgjrmn.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gqzecmplu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvnwqvdfk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/ghyfdjmxl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/giccezmfu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcyfqogwr.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/giiscjfpw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gmpldklng.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gdvdpnvmv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gatzmepvm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gwbuqroky.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gwomudewb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwtfhmhca.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/goowxixux.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/ghdxrkpac.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gmpjmmfke.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gusewkjkx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gfjrsykyk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gogypaqmr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gqvnvyckp.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gzodrpnat.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gbmacifmr.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/ghmvwnzwg.sHtML


<!-- 参考信息 -->