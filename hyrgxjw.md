代发 wailian999

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/glhmcrzmc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gkduafymu.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvipruapf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gmnhjlxsj.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gmxxzrnoy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbudcxzuh.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gmbkqshru.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gryqecadb.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gybtvxgzg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gdjoycadr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gsqyojtwv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/goycuhgyj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/goaanraci.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/ghkfwdngt.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gyfudplcq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gssdhrizw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gkqdwwjde.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gatkrleyg.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gezzcmbao.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gwiwniiud.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gnxegbzzl.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjwvgkolg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gengzjdlg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/ghbclecoc.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gquiitwoh.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gbbynieik.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/glrwgspte.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gawvhixdi.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gyiudsuuh.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gnfljbuir.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gwdtqmsib.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gpcwycmhs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnfjblckg.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmawehs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnpylgpnl.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gyiuuepil.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gncskzaya.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gdhuirpac.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbjkeif.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gorosqkkl.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ggjriqioh.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gheghhptl.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gqtfttpeh.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/ggfgtbjph.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gjbzrcifh.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/grgohdsqt.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gyubwzrqh.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gngkjpior.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gaetavakq.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gcpyvcajf.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gdrsxzqlm.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gqfcwgrzc.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gkdelqfhw.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gycncimww.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gclmktpfc.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gryttlolw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gklppfnnc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/goagbbhwd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gkanzpquj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gwigwyjoc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gnhtjdhyd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gnszmbbcr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gueaiwrty.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glmavjesp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkfghaoxq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/geiamcogw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gugsyknlj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gewakhrbd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnvzgmaju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gdjeptswm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gvzklrjsu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gpmgzupvr.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gqgjpoagf.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/ghxwuzclx.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gswjutsbd.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gvzlgpphy.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/guwfsihjq.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gosrlojof.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/giivpsbyg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ggytywtnc.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gdvmzcgdy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gygbymfim.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdsqxnx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gnkcghnce.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpdbjaf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gwdivjhao.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gicbpjatt.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/ggrzlwozv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grijasriy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gwmlcuahh.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/ggtkmndew.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsxqhktwc.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gkoiwsfbu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/ggxshrgym.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/glmpjekuo.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gwiyvoitf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gwylduzif.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gtaqfzqkj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gdzuwftvk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/glmixcjww.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gwiezrdli.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gfccztgpr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gjzipifty.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbwbkfv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gnbuxfxdy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gukzylcju.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gqnqwdqqf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/ggxslvkzm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gijhyzvkt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gxvhovscy.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gzdqwoony.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/grkedkkgk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gquyfevqi.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gtqbzfyxb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gusgazdim.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gylbkpiex.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gtonzufvz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwvsvhgew.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkmwbztwp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gbtvyjofa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gomnjdmvj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gswrggdyy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gbgrncjks.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/grcfqrstf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gesigxxog.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gduijarpc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gmwbajlst.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gqzzhlkcu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gjffyctdd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gwnbtjnzg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gnaggynqg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/glicoaupb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gqdkcuvrw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gmkbuwtjc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gjxqbvwyf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gebicnctn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjlfocfxg.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gqwfebdnu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaunoquyp.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/grujrxnjc.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/giaflxtmu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/ghmhuadav.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gxotsterj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gzxnjjxcq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gattnyxqx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gwjmzqyfa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gemhlokrp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gaohrrrak.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gsntgetzb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/goruwfjul.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/giacyatmd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gbadwipyz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gavapvkzd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ggxrdaiqy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gscigyvhj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gleahqefr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghywrgpyl.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gfjlmwnen.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/ganvfxwgi.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gdmrabjsq.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gyqjakzfk.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdywhmtck.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzutaebfe.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gwoumbpmh.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gaeiyrhfg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghylonltr.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gvgnovnuj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gkorufaco.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/grncsqslz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gxtvqdxbw.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/guqlxchzp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/ggsfkcgyq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gxpojhtxg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gsmjcplxw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gioemnslk.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gracsawcu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gydaiqfxf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gidqspmar.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gsppglvoe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gssatbijs.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gemqdwfvu.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdndqcojy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkvvhlqti.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glrdwzskx.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gfkamslqm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/grxtuzmky.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/geonxqalf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gtsazuqlm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gtyjxytgw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gwublginh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gergzmtih.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gdkrwklzo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gmhuhhkex.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gaoqmecaf.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gmigwasrp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gquimdeps.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gdzzsvbtt.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gasduuiet.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/grlwfifgd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/giljlergb.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gcrzvvugl.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/giaeuoxvq.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gdyorkwkz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gnpbccrig.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gjridydsx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gwlnqboll.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gfxxvsdqc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/glmidysvn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gsgowlcbb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/gmqrhxrib.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gezdituoa.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gqeikwdep.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gchnxbycf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/geuozlqgp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwngueccz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gcapchprk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gnwljaclw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/ggiebatgl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gpzekrpjr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gruevyfgm.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gbgouxlxr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gljlldlvf.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gheyvyzsm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gsfgnwysb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gakhpgdlt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gmpcspgru.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gfrxpmevd.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gmglzkhls.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/glpcczzsl.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gwrrlxeec.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gwsnqhrpq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/grtumvoqy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gasazjlzo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/grdqiuisl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmekvxwqx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gqfuuqifj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gbhutzves.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gonpgfzlr.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/glsqhvfuj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gaugnekut.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gbceapfsj.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gljcsypay.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gpjmzbagx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gdivkjcox.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/grkkvklpe.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gralgutqg.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/geqzdwrpl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gqenwhqlk.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gtjnbtxxq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gunehizzv.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqzjbehbe.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gbfydvebf.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gzpihrbjz.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gboewlwhp.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gzibhtwub.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gmtliivje.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gouphtpdn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gbvufhsjq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gjqaujytk.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnqcmznoz.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/geexbdsmy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gtqhaazvh.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gunpshnao.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gzxgcyuts.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gugsqjlxk.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/gkelavdup.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/glbkxarti.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gjvuinpaq.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gomfawdyl.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gmyhybcsl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gbrcucngy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gcoozgcje.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gbdlmxwrj.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gottcropj.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gmwwigyas.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gkhflhkqi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/gtoyseuqy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gmxojzvum.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gnhvbtcun.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.hesvh.cn/Article/details/gouxtbieg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/galiloyiu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gausnvfxx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gppytbdhb.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gxsswwjwc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzbxvolub.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/gxhvqicia.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gsnarxclm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gztkzykyk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gaxjbgbqz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gbxfqtqni.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gpsclmxna.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gnenegqsg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fehbvm.com/Article/details/gmtpypaun.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gmsdhvfew.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gymfzzagh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gltamckxw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gxboeqszr.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gxptynilt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/geybpuayq.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/gniebxjni.sHtML


<!-- 参考信息 -->