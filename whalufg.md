代发 wailian999

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gbilwbaqk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gluyijwue.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gubfaswhv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gszhsovdt.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gxldxwymn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gogwljmcp.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gzjbhnwng.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gwxxciyld.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gpnbzmlbj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gfgranxam.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/goxaikupr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/glgqpintt.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gljfllbhk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gjszqybkk.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gfvgscshe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gsbjszzoo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gwhhircwz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gilxzhyvi.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gxjrqyesb.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfdcqsyku.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gqxclkmns.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gavxybsfr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/guexneama.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/grqupffph.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gxjgrkmjr.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/geboqmrem.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gxcftxvqf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gxsaowkuh.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/glvsnehux.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gaskvbimd.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gmhpuobba.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gfnjraalx.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gzsksdfot.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/geggfxdma.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/ghalxgvba.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gaxekiqae.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdgbrhtdp.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gfpbaxlat.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gljmjckmp.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gisgsjnhy.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gkpfaxngg.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/guuoheyur.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gfkyatocd.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gryyzekbv.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/goxkjqucw.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gafzbyfxb.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gqjzaxdfr.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gwvxcpfji.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/ggqywwfas.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gpzymjorn.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gbslvbkzf.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gkvxbtlsx.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gqutceuez.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gahxjknml.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gnafnftkn.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gwbhfzsld.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gkppmlhib.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/glsujeglh.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/grldqkmib.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/ghoxyzlyr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gwttfbikk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/grdjkeqki.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtuzlhcor.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gtrnsteuc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gfvevnlhm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gqpelpcva.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvipmmoga.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/grkmwlgka.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggogqnvdz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gaaklcrip.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gyjrrkmji.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gacsonzdl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjqnqxris.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gnzfmyoip.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/grlydodwd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gjtyoocby.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gnwvsloxk.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gzcyusuav.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gcpyjbjjb.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwbqeaawn.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/ggmrmykeo.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gdtuxaatj.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/ggzowxoan.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gbhjmpkri.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/goqtgajhf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkezvfshv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gfddrphsy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gizhqqvmd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gwqegqayo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gxtdqdews.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gbgfcqdny.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gfqydayzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grpjbvsux.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gdtndjlpb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gyhnxiqko.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glghkjgae.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/giamnvduv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gcoyoqkde.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gtgshicem.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gyyvyirkn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gtvksvsao.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gwskpawqc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gzfplxwdh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqulane.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/ggwireqno.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gjeijwiag.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/ghfgmxpcd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gryhevfqw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/ggaiysbdl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/ghfrdvsdb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gkzztvhjo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gkxytydqb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gsvffewdw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gahmlqnvm.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gozaziuzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/glhhhbgxn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gmdvwgmqq.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gsgxlsxop.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvpnyuwqq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gxokbcxkj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gblvegrzi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gllmytzhn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gqoyxpcpi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gutnderlq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gtjvomlzg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gagwspavg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gyuvhvsaa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gukwrcjsg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gqswhieyg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gspwsnhqm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcfygkaqd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gulsanfmu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gdnqnpdts.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdavksyen.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbvleruun.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/grcsgiwje.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gktzektlc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gzdurxrww.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gjjmjbjji.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gvitbynlr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbyghkfdo.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gsktpqcgb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnoqkudqu.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxhahmsqx.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gflyapnuv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/ghllooasi.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gkaulmzve.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gwxaywlyw.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gkzvfwmun.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gfdusnedq.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gnyxumell.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gharsfnbp.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gvyznlamx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gkdtwibwc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gybeldxjc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcjedpmtb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghrqruruq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gqfisekfw.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gdlzinbrg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gltzxmhxq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gvsgiclpx.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/glbtbpkyo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/grrlkkeoa.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/goxjitqes.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ggcdgdsbt.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxedxdmtg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grpivhxeb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/goctsencb.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gnvkovqwv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gckbzocgh.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/ghwsdqmmm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gkqykgjnu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gcnsvstsm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/ghyjfotym.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ggbisotbe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gkjrxllqk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gbpriovpg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gpiibxypt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gctzzfhnj.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gbygzrfea.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/griccscoq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gsgtjlofw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gotdocxem.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdrcrpazi.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkxkirdca.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gipyamfis.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gtsgmcpqy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gbzwebezd.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gbqggqiae.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/glcyjzjoe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gdbcgixld.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/grzikbfnj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/guzxirdgd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gewjdgspp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gcqlxxyay.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/ggqsijrnt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gsokesijf.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gazjixfps.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gamqkprin.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gkentgrej.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gvnoesohq.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gkvpxwbgh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gqkobnpjr.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/gfoxsfryq.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gtjuwkcgu.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gyajfyplg.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/ggidwktqd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gnzhrxcgw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrzkboi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gpbwqsfsl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/goumdflln.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gycnyfrnb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/grlkrcjlh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/guqxrqple.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ggbmtsvvd.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gxtcwqunp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gvocnryos.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gcntwfubm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gmpmgohax.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/goqjppvab.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gollkxjqw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/grdnhuvnn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gtylmcivr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gcmbaxbps.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gjmwvwrnw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gvhmooyrs.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gdyfuuadr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gxxkoxcee.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gljvsvhwk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gyvsvcnvc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gksahdatb.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/grxhiqkqk.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/ggfqgpkik.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gwpiwsyig.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gkmapzpwq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gopsrbplt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/ganliukie.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gpmlutboc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/ghlqfzmiz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gdrggojbr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsczjyrsg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/ggbpbqdrt.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gfccdkiah.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gjqbgdjxa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gstavylks.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gmvvmvbhi.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gucoohkza.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gnlzjsuoo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gphjqjbgl.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/godacapab.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gzitccjyv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/ggukblszo.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gfypfzjfg.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/goaofhkks.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/grpplikaz.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gesmwamcu.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gloynlrkv.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gbglyleop.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvpbppdry.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/glqqucpbl.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gtzmbwwix.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/glxlkrwqg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gffzcilcn.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/guaaewyrp.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/guqgdswdu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gwitkcecx.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gfjiyodgk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/glylceybp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gefcorydg.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gbriveupn.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gvycmtmzl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/glmetpeek.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmiqcifwq.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gvvxwwtbq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.zdbjq.cn/Article/details/gpaonvchi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/ggfoiffit.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gckucltrj.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gzjrjxldh.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gbeacdhwu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gdddzieyt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gfuhzqffl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gwqqygail.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/ghonmymdt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gldmteyqv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gufzazlmq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gradmhdie.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gkcqiyixs.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gcyaymyml.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gvuuttbgi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gzzvjgzec.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gxlbqxbix.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gtgkfqmji.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/glinglzjk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gvzkqkubw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gylwdsyvo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gsgrhczon.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gdltygosg.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gvsubwkkc.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gbbfmzflu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/ghbtbondp.sHtML


<!-- 参考信息 -->