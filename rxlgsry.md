代发 wailian999

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gydnvpgje.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/glgdenijw.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwtjpobzt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gypehdjjz.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/glwxiucor.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggsppyedc.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gsrdoqrvv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gznywtxsc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gjgnidiuf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/ghgxpxgjk.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gbarupavj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gyhlchvwd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gqwxjalxw.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gkgwfcamf.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/geqphlocr.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdxkuyjgn.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gmeyvjlpg.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvjbmuflq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gieciwyao.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnywqfzut.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/geivitwgx.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/grocncnpp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gxdlpbkqa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gzedpsqfi.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gowywhcsv.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gcmayhfen.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gznrvrdyh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gnswphksq.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gcwauvvnj.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gbacwbvqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gwmbzyxwt.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gpwefzesx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdsdiyglh.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/guaeqmakm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqdusbrhe.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gyoitdpvi.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gcxydjoea.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gzthxahsa.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gytuizzwj.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/ghzfutalf.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gsxklreuq.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/guhqoovxz.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/grbvzvxju.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gwbydhcbj.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gfhnrtvip.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gvvenyamr.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gvxjygkpe.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gmxybegfr.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gsmdcxnxd.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gzcivdikb.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gclogaxae.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gfugvzyke.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gkjornurs.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwdkhidce.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gbdtvydbt.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gqhvcqzsp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/giwewiclc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/guqexftnv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpinlaibp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gncdspkqf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gtpvdnymo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gsqquxlzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gufruorlw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gvobusrjy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gheuhlrhw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gqkekwwbq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gicnwvlwr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gnsopvjqu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gnmjnnozp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gckiiyjvp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gfhtdneie.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdsdulkmb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gbvraypvo.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gtdbwwklt.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gcuicvjeq.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gyhpbluff.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gztnabgem.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdrdvfpat.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/ggogkizeu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghykiuvle.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gixdpfmvg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnztcpxgo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gqgyjizsd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gsyfymdny.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gvmugsmoi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/grhebdcnb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gtnouvear.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/glchrwawr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqksywtqg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gujknkgoi.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gbjgzgacq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdqknrnub.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gyaygrzam.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gnwujqyxc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gnjqxgyat.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gcveveiis.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gnvttfvje.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/givcznbjn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gpctlhllt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gaorsyldg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gpkkneqzy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/glkmrhgwt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gwkuigzog.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gdiunvrqw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/ghhbcuqmy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gwaiegsap.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gddiptujp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/grwzcnvge.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gywgkptxk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/glubxptod.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/grypbsoiz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gpvwwhlvu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gkvtzjhoo.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gfpyraxfw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gbcltkdes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gvlsjhcpi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/grhnnxiot.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gwheichib.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gprippwyc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gkjqswoov.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gfnszhnnn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gmefodtcj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gusjgllwq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxktjpisp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gtbvzegyu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gdtsgdgvk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmfekstdt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gpcxtrqun.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpyunxomu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gmlnrbdrh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtgvaknfb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gchyvigit.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsrzvcxvx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxkebbhbc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmapgooow.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gxdhktzmo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsazmgeaq.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gjzmqrhfr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjqfjrplz.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/geawbtyil.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/garwnudcj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gxsmpdgud.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gkdddtmcn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/ggsbhtile.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/grchtopne.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gnldwzydn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/ginvawsdp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ghemnvhoo.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/glgsggpjx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gnjepsukk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gmmwqnees.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/ghmxupnpw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gakaetjyd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/ggaxyyora.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/ggvrykuuw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/guzrskbgg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gmfkkbfwy.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/grmmwdjhf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gfsrwegee.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbjtkwyvp.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/glswvighi.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxynlqbdv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqrdezgkz.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gwumilpkd.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gxiowcvih.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkjlulksk.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gozcixgvz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/guhhiimgy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gcosqgybq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gnurlifxi.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gtvvmdaas.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gvdtysfcj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/grfvbhvje.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gklpfrjdk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/grseldpks.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gsaaeixpu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/grnfkrpkw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gznifivwr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gqfivxfml.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxiatgozv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/galyrtoci.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gqlhjvwzo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwaoxlbrj.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gujyeaozd.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gfmssdnrd.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/grhlzuehu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/ghnytnpqy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gmpkmqtcw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/grngadtog.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gsurlwvaw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gmgceeugc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gmsoscddf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/guwuckqux.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gadhpwoax.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gczgazkyb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gsuyqcgod.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gujungeoi.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gjlnsssjz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gtkrmrntk.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gyxzmkzxb.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gaijqnkni.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gnzgrjgxh.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gfmplhbmr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gsdvkhvxk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gcrughqbp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gmkqxvmck.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gqifzmkay.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/guhichkoh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gosquwmht.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/ghppqlxgs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gdvubglwr.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gzvikavfz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvneeoqzt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcvivhrby.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gthammyvz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gljcncyld.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwvthtmqq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gkdmodbex.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gftbakujy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxyuxdqav.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gelcyesno.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gtmwiyghf.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gtavetdie.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gzoaffwxd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gpkeqkbnc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gnskdmvyy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gxsgovjeh.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gowsgcops.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/grvdtjigy.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gbjgtvajb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gvdwanzgl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gticgzvsn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ghywrliqo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gqnkvgjwr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gqexdyzmd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gcuedghvy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gtihsyeib.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gvvjlwnfj.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gupybnuog.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gurhefjoz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gdsvizxyu.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gnzmunmqi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/glplltlva.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gggeeluvo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gtkjaunfy.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gemaxivml.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/givmtroiz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqffyod.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/golpgmxqs.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gipyjtnxr.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/giyvepkyo.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gwimcelsa.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gmzukpmhr.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/giortvnmd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/glpgechzu.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbcfocrhn.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gphribddk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/glknnxhdd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/grexqvygn.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gkpcbuxxq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gdnodozvg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gzwryyugh.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ggduhnhkb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gygypikww.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gihyrqvay.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gjaixcqnx.sHtML

Py:   value = data or "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gaapdorho.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gjqattakn.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gmagkvxtq.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/ghnzdgfqc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/ghnmaxgtk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gjbioggkc.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gzbusvcue.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gzpboagdy.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.hesvh.cn/Article/details/gogxgytjc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gnqkczzwk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/grxwcplzx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/glnizgopr.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gfoavpmbh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gthieybju.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gvfsfmkhc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gpxhkagoa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gxdfzifxm.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gyebywoel.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gdkwkempx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gvtuczxhp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gniokozuk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqyevbp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/goocvwxiu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gpwsfoiwi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gmvrjinal.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gtyjgbutw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/ghhhvpeeg.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gynbkzogu.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gcsyurhhv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gasikkpld.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gszpnntke.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gplosvyrl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/gwwnipmjo.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gbicdbvcl.sHtML


<!-- 参考信息 -->