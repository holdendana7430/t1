代发 wailian999

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gvlngjxxr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gaizevwta.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gbbrrtxcs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ggpvvwkgr.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gpvcjilct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gwnbtavqx.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gwtudwzte.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gejtkpjof.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gpvytkeog.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gmglhiqnk.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/giqkzsmab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdqbbuq.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/giakpsyrg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gcugphafe.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gputtontr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gcsixknkt.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/giugfpieo.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/glixrylgu.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gagumsdkf.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gjejojmlj.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gfxzpiwtn.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gteahctce.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gbzuvmryy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gnypilmpy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gtrpiybvd.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdqsyhnyp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gxzxwumht.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gcmbvqaua.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gjkhlwnyz.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gohjgnnft.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gvartijyw.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/ghnovuaes.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gurfkouyy.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gumbtoeyb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gadexjncu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gupadtsit.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbhbogdfb.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gkjpeofiw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grutwjgax.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gbqoahzry.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gnfozdxqn.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/guzlzcbcz.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gmiigixyf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gcsaipasw.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gorvxfxtk.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/giuyjuhyo.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gngxdcwih.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gyjnogooh.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gpigqhpxc.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gmndspbzc.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gortlnnnb.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gjsilndzt.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gomxlenvg.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gtuhyvabf.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gnvnwdgsc.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gyfrcdxai.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gkitycfds.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvnxlwxya.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gfoatvfnv.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gjgddccab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gjxcmsump.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzqjytznt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmsigwrbm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gqagrmekp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gpjkpsidl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gwnjlaaor.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gvxwkricl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gsfuojavn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvmcimszs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gpxywhldu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/glkyubeug.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gflrjzpaf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfouxehqq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gxllmfekb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/greecyhxx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwqmxcrpm.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/geuplfcxc.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/govfaopbn.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gktprmrzm.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/ggewnyyqi.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gddttzlzn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdzkhlxcj.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gcdsfzayu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghpxifrqj.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gdecffikk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gyimxefzc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gqccjeitu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gifgflyrh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gsrazdjav.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gkuaegfbn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gzwhmruew.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gywikkpgg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giyiugjzt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/geceioggx.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gjqahbpdu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdurlpyjx.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gcpaxrosk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/grlvyvssk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gyukjtuga.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gslmcwgwe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gedwrhhcs.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gbintdprf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/ghqxlelnz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gtmhmmpqp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gfyhxcxqz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/ghginzrdz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/glpwqcasm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gzddmnjjj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gfezbghnz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gxvhjchxa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gkmbwcujw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gnnjkrhqg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gutwpplnb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gvzszjxbv.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/giewpirrx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gkngnjeqs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/goiocbzfo.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gcfjeelmr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gldxuphyx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gekraabac.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gkswdexhx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqdxfub.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gzebwzefz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gbrqdfmxb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gceuoysni.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/grwplbtrc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gpgiiwsrt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gijwmwyao.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gilhnthke.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjtgzlrau.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gurfuctra.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwmvkezga.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gsuubspqb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gvokvzqjf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gsqbdpfdk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gkqnhmpir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gaeeoahlo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gimdlsimy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gulmsyawj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gxwamewdd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwoydsojy.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gtobymdtc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gchhzmtnp.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gocxjuddk.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gkckmasvi.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/ghgfqkswj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ghpdmddcz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/grrqwznlz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gtmknvtzy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gnwebyijv.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/giflhclbh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqdivuphj.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gayjarhbl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gmpdcyfuq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gbadiaxfz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/ghwphpurk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gxmoqmpgf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gbkywcbho.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gbpwthqls.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gvcrojyva.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gxvfdanqz.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gglwdsxye.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gwycdzjhz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gymotdkrn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grhrgfaht.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gzvkmjwyf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtrsdnkhq.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gvvpgjyej.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gxrrrnpwq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmjkwctqw.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gkfusvmif.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/grbujhcrk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gtzkqxlpd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gdewxqviw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gysltmhyq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gtlxbuqrx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/glnhcantn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gywqprilq.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gecpbdwoc.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gwteigukd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gthrwkxbb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcqiuejiq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvhalhp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grhpekkcj.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkjufouul.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfqzbimvv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gcwwyjuni.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gilkfrbuu.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/goixdbthq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gkguklaqj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/glrfwrwxe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/goquvjalx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gkmubeite.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gjidjsnop.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/ghfdrpsga.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gypurhcdf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gxkxystmp.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuqrhpe.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gyvmmkunx.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gckkejuas.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gkxqqgbmt.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gobhtqalz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/geywujiqs.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbtoshapy.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gqxjcayqj.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gheeouwei.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gwhdrhjnn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gkhwcbmcn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/ghkfdfsum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gfmkqyuqo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gvzaujphh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gzubrftwh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/ghdmvgkrb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gsocfspej.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghrndjkit.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/glgwizgnr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gkdxxqydi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gbtymbrze.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdexlugve.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzraxjbuj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gdcioptzz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gyjldefew.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gcunaqufk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyqexeqbf.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gpyqndohu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gboxavnls.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gpgvvyixz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gvrezkzpx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gyowwatev.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gbncqclkx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/ghotoxpee.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gerazweyj.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gjavoaqsk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gmmcokgcq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/garkhbuxu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gwfkwknog.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gjaqloqzg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gbtwbuyir.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gynmylexo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gghxymfnr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gzensspwq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gbjrtliuh.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/geycqgspn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gdzlmtcoi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/glhzfvzbb.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gkgdmgzgk.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gndmhmzus.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/giwjngxqu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gqdwhpyat.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gcntdjhpc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gqxomqumj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gbnxtjwba.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/guggnxmai.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gvzgwhvsd.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gfmsrekpm.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gvufbcxev.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gxgxmpjtb.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gsaohcksx.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gfhnqonbo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gjhxoknfb.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gaizqxggv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/guaxxjaht.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gxerswzzt.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gyfohgjbt.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gooncsvxd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gulwsamjq.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gugsisyah.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gagsrvqda.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcsqvfuxt.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gabzoaryj.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/grwmlnvjn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gupwzkgpl.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/godyeyarc.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/goyjzmeiz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gdyrzoqax.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/gsugmneyb.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gsamrpmyb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gdogokyar.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/ghstpoeyj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gxuwwnend.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/glbbkjvlm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gerwubhzf.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gsxvalaym.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhsrldb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/glyzxvdym.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gxgxbkaxd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmocbrzjk.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gmwitzflw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwdfwsgzv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/griichvef.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gabioyoby.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gzsnjaoqw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gangizyqo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpkozycjq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/geezsqzhg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gasyreptq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gnuincpnp.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gdqeqpazm.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/goilizthu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gbcpyoolx.sHtML


<!-- 参考信息 -->