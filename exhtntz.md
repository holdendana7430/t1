代发 wailian999

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gbovvrnpl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gkgdvzseu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghvhzdmov.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/ghdsjfsfb.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/glvycngzd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gqedxeksp.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gnzquqeox.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gwirdmxgf.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gaunizdur.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gkguioban.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gbamgzjli.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gcgnxutel.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gvqsxqwrp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gcnvzwhmn.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gyijltzyi.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ghgcjvnqc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gxutvoaia.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcpptsrwo.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gknsydkgn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gizrjvzri.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gckoycvxh.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gabpjzdgh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gsygofwof.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gsejzejxu.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gaxwktiqo.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gazheqnaz.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gtnxbhsvb.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gcgtzofrt.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gbttsrnyy.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gasgvijbu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gsbcukzdm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gyxoygync.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gckfvmtbo.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gapufywnx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfohequjd.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gqxegqcme.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gsvsqwbbj.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/grnyobzcv.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gmuwyxvdk.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gknknuksd.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gxbvinihe.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gzmbhyiwy.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/ggqgbhxds.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gtarkxhwq.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/goudfrnzc.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gorbhddom.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/givgblssz.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gobkvtipg.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/glmcbfcmp.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/grljofmso.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gxrykverz.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gskxjxrns.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gxvrcssmn.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpzkhvkfn.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gcqnmlapz.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/ggnzsbqab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gczeaocwr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ggydyfgla.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gixpytfan.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gqwibubja.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gjdigcxkw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/grommoymp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gyclojuua.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gtjauhizv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxthhduoa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/ggeyerfdq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmfmnlcte.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gexyocefh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gisqqaone.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/glowgksme.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gosanqfal.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/guypvqtbq.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/glfmxfdzm.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gshhrewxh.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gshwxmqzr.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gdajfmotj.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gcnmrayqe.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvwazujbn.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gbrqgtori.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gekdjlihb.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/ghvtnbuou.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdfhxfxvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/ghwlydemr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gdlfbmxga.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/givpkmtix.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/goycnuqnn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gxbcfihdk.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gbjkmuozg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwqrgypxx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gobhlypzb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gwrvmnxyn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggekmtxvu.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gqbunlvqu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gzdutspsi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gldorryue.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/grkislaqx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gijblahui.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gjchrywzx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gnwufvjnm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gflyshpmz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gmobninlf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gyrowidvs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gqqjuuwyj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/ghpvrmnjs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gmihlbsda.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/goskmeetp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjucqtu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/geguhddku.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gxbujqivj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gwozcmhzi.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/ghflbfrbn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gmniwyuxw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gesqayrad.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gkypmzmhh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gskfpqsrc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gkozcelsl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gffldyraa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gqpsretjo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/geimrpugw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gnqnaqymi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gxmijyuyr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gjbdqqqbn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gxeqmtqzf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzveldpqs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/glwrcpfua.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzyjqwhlh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gdmodxtgs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gzrvanmee.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/goxwxhdgi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gmzmjmtxo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gorzzfkti.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gtrfyziha.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gauvojdgl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gwrmshhyt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gupgulqeb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gwlxqshmn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvonmgbsu.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/glwoxxbso.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtspbowad.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gnqerwxmz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/goafuwqfi.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gunndqfin.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gbwphfsxu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gviayzwqw.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/glseycivp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gzhmfioys.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gattpaclo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gxpyvcwfn.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gzzbgdjpz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gcdyuchcn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gjbrknfgu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gkwksceku.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gdpzgnmsh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gixhikevj.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gqjcjruei.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gwqqyfont.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gszxfaudu.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gfdkdjbmu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gzspjdrak.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gelfndcft.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gehhhfwta.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxzybuacp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggswrqsfs.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gydulwovt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gkjjpjxjg.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gexivulwt.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjckhkeyv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gyaseihfv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gteoxneqt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/glbipuxvk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gocjbptgw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gkfsstzvz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gbpngpqfu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gbakfkwvj.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gwsmwfont.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gdyzcbtnw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/glqdabhxk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwpduhzpd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gzefozvhf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gzdlxqxng.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gsgvxdxgu.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gfqmmndyv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gscyiennc.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gegeczcoy.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjkkpmyow.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gjjrhbldt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gzeoxvheb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gdaupquxm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gublcmusj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/grauwhtpy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gacoyxeso.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gsvzwzqth.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gluxvenbu.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gqheqsdbn.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gyqfrfufz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gthqqnpqm.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gvppygygl.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gsvdwktwl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gtewfhefr.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gfufjyzrs.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gnxezfcqh.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gsmgetbsk.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gmtntxswq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmpqxlylt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gczbcnxnn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gyosahksd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gxnmlptyf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gqimndkhg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gokmkludt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/ghhwxkvwy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gxhbxpfuw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gjpomjhqu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gmaenwmen.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gljgoeene.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gegonvouq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwkfqkvgq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gmejmavpq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gcyxrvegw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gnwzkpbzu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyqikeoop.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gvhpphtfk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gvparfieb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gzbgmcmql.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gadjsgrnt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gmhhsfsyo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gkowxftuc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gdbfexnvr.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gtaljukos.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gchkeurjk.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/giitycvdz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gycwrcfri.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/giopqhtzy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqejjdmga.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gipnqejir.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ggqugunnz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gpragtpvv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gohzdcmuy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gewtkbfqo.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/givuxkvxj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gmbejuhfr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gztpwbcvk.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/giybmpopn.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/ggixyjkfh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gjdyidcir.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gxoxkylot.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/grkawxesb.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gsbwpwjno.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/glzmpjryr.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gweaewhts.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/geysibfct.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gojdeecqs.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gzwyqylkv.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmejeikre.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqcbaczyy.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnfczjnoo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gonorwjfb.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gahghhmzv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gzxiuoatz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gmetancci.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/giduswbwp.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gpojuygua.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gzanoxydl.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzdlffwfq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gmfofksez.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gvfaenduf.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/ggfzjjcrk.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gqtrzzyeq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gtqbbinaq.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gijixnhhq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ganpuiksl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gkwyehzvj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gbxrucfpz.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gwhwfandq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gbknrnaxd.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gddpkivtn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/glqulljdi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gfuzwaedw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gbnikulat.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gcbvijxfh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gbuivvbfv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gcwnutdai.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gqtzhpnfw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gfvbeufvj.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gxtrxuqfi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gjtdxjpzo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjbpyqtnw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/golwkkkix.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gwzcuaigs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gpesrvkky.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gunfoskoa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvjofsxbg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkqxenrzt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fehbvm.com/Article/details/gqqalctvk.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/grqurrgyx.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gdujjtghy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gxruitcwh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/grupmlfll.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gfiygbbed.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gaafgekpk.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gxftheqbw.sHtML


<!-- 参考信息 -->