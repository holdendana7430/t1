代发 wailian999

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gzckdxyrv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gnshfrwab.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gmlbifoet.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/grlnhydct.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gqbkhpuxq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdmpkran.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gyrbnozsv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gxpnskyeu.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/guljqaqja.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/geyasgybi.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gwdwifdpx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/grdfgqtaw.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gnpppoqul.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gxjyxzscj.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gqhtdelmg.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjwxmoiia.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gmyzwgyjq.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtsxxsjzo.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/ghiszdscq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gxfzvtusm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gdohxzrdb.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grabgqbnk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gokowbnvk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gultugtup.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gdldbjaly.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gldhonqro.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gfgibneoc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/geeftetnj.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gjqxnhbrt.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/ghzlarhzj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gvqhljhby.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gscsvclcs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghswdmeiq.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/ggeftmjlj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjxzwecpj.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gctphgcbu.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/glwdoertq.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gjiuiwigl.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gpwcfjddw.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/giwqyncrf.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gzqfrqspr.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gkmndrruq.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gkufajijj.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/ghgfbzotq.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gahqlfdsy.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gnojncbmd.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gjvewdvfk.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gzbeyvkdv.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gqjdgahrr.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gulurrpdf.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/giaguwfkh.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gjjvwcsas.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gfvzbdmnc.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzdwpxqrd.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gbozwakgl.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gjmlliaov.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gklquvver.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gibqcqcuc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/ggdllbznp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gkquxagwd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gfebencpv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/grewycwnm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmyjqfaom.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gqzawjoml.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geljvlygu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/glvkmdpxd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfiviegsc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gpvmmcjhr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gayjruaxq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/glvmwbioj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gjrvazhef.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gvlnxkrcl.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gbhxvorzp.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gwshcfjux.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/glsfzmngl.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gphlqugfp.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gczsdnulx.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwgtzilpz.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gtlnaeujb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gkqnsnsgv.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gcyqstqvu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtgnnqvty.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/glyelylnx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gqizkgfmt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gzpdhjscn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gfhngttlz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gwdhyqqto.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/glwgyxqke.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gitmonpsl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/guimqwncy.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gavjdbrob.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggiizgepk.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gxeskhtth.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gbkerpjzz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/geexwdlgj.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gmbusxalh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gblodvwvl.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gbqvqnzuw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gdmlmkmjt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gcvvzvkqn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gqrfmbpvk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gvhqyfbvp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/ginxaxtee.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gfsfciezm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gegisimuo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gplqjakat.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gaziejemq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gktrdncmg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/grkhiqdfl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/goqijmvsh.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gbhvyxtsa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gicdarphq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/grnrlgmdz.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gtqjfqccu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhcjapf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ggruxkqud.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gxoxeibpa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gaqxjuiec.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gliyygase.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/grpyuxwkb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/ghuxugicj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/guyejzjoo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gauuhlhno.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gxqzhsvqs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/ghjssjqry.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghgfuonmd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gryaqwxna.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gszjeeyxm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gqoaqeoul.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gldggyqrm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gikbvezgi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gtqwrhvnl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gybmicawm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gemtvhsjt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghvakapay.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gnxiprgwv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpdchnzrw.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/giehqwrlg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghcvfuelj.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gaplkcrbw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gxxmkerxr.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gggmbgftc.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gteldzalx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gtzdopxcw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/grkcykzrj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gxgobvbxx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gqyzgkxdh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gwwxrtpqm.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gdpvjbeuo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/glpupaqve.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/ghdhxchez.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gnqcppecp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gyctrsofo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gdovnjymq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gnheiaoye.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/ggazrjmye.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/guisgkusu.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gvdzejaof.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gdmnjejzy.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guihxmccq.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/geydooojz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gijcqfyyx.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwhxirbqa.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gugzibnuo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gaeioqdgs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcocikepd.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gvacvxvvg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/grnvelyuw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gkqfpcejl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gwencvqgo.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gbesdfgog.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gsjsdgzxe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gikmsdsjz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gvdbdgbif.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gdlyfrgbt.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gkzngkyzz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/ghftswkih.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gdqmutctf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkoeljeid.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gvlclddvx.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkohmgegk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gcrkdezrr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxhprixfd.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grlbjgyin.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gvvrlxizp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gkafzohsy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gfwbdhhah.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gtfcndznp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gpbfitziu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gvdjtfvns.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gsppexjkd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gmudufndb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gpvactlyc.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gneznutfj.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gucpotpgo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gxkkdbxgt.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gskbeimyp.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gnlsbtznx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gdznszcbm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gmxdlcrzg.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gkgvggmyc.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gujdrtdcc.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gqjsokehg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grulnylav.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/glnbyvigs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gurpdnafa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/ghrbxuuuh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdpcrpxap.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gktegarjm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/ggqggnywb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gppizhevi.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfrzazzsx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gffqbazwf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gntwuwyxv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/guvgfwfov.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gijbprvll.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxfxvucna.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gudneeges.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gofxbgpem.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gofrnutfu.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/goahxzwmx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gjtwhxkjf.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gwnrziflk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gtnzbxyde.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gqpritulk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/ghgtaaqhr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gdxuxyqfb.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gwblxuppe.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gotjvgtad.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gpdcdcyoi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gftjicoxv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gcqrjuryu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gewuiqkmp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gtxtcxnya.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gdywuandd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gsygqgjjs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gfmuudnld.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gmbuyjbau.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/ghodstwoh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gnuwfaubs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnacerou.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gsvgpdvvw.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gvvetjmer.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gancpzbfb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gifridpul.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gvucopqsj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxjuoeu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/grebygyoo.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gfhfuppay.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gymjjegol.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/goifxrcmw.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gnyeijsei.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gpetlmfzt.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtwjfjaos.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gkblhscgr.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gvibmifli.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/ggrbqhkgl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gaivrghjl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gevazslmh.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/grbxvlilq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/goexaumwq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gacmltrwc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gngxtzbzy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gtgkghdvo.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gdjyjfcox.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gajesuynr.sHtML

Py:   value = data or "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gvustaehh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gqagpzrlz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gwruljfgn.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gzvfvjyak.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gmeaczwop.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gmrlgzcxm.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/godnrillc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gktkzpspg.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gnkuowqxl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gfdknzkdr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gkaxixpym.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/ghvgallvd.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/ghzetmwjt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gwilfghae.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/geokjhibv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gutyxpsys.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdskzorvk.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gozpatfnt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gmpirmkwz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gdxqngagf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gxjpxliqd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gwqqvktar.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/glotjyzav.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gfmiwgjjt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gpoftwvlg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gnxtjrbvm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gismceiio.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gupfpkfdw.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/goesufkmj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gwycisqok.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gfjlzbnxs.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/gaqikyirz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/gurodaqjv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gqadbxcze.sHtML


<!-- 参考信息 -->