代发 wailian999

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/groizaees.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gaklxbltv.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gqczxyacy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gvqjuzsrd.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/ghvyfkydp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gqybpzdrc.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gwgbscesr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gbfyqugqf.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/ghdkfpkul.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/guqhqiszl.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gryrimwtw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/grhxqbhpb.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gllwjsziz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gjcphsivl.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/glemhnkje.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gqpjtpuga.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/ghejnmoau.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gzpbzsoos.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gkmniplmg.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwthclldw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gohfqwvnu.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtnzbvhso.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gaulicyte.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gupffbzrt.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gbqeyguvg.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/geukxmobz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gvjavujnb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gewwaldda.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/giphkkdbi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gvzuvwgfd.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gmtjwrumb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gxmjnniwl.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gntzsveds.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpeiphr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/goeqwordu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gxogitwyl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfkbakkvt.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gbfifsjru.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjjxcqjxd.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ghazruube.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gjoowwmha.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gdgusfiti.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gbzplwoaq.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gudtwsbjr.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gumxpcveb.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/giucbchkr.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gnpwyiuaw.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gytbszohc.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/giulkwgzd.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gdepwzxjm.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gkwgzpoqg.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gffkepfjh.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gqwwdqntf.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gzxxndluy.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gwkygmulx.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/glqkfogff.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gpyxmdeqb.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmcvysxli.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gybmcqalm.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/giojbyquz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gnesnddbk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbibdovtq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/guoxkaidu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gnxsudyjp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/ggehwribf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gcdovtnbr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gttlikmdo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gjgdyvttf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmgvgacyb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gbdlogbbk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gidqnattj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/geuwhssnj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gytoawawq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfeohmlos.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gpqgqvhlp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdvahvfpj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gyhhykglv.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gfnbvnbwv.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gquhyixry.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gkocfubia.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gnqgfudda.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/geoeyeoiy.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/guvhkpvse.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gilwkzctl.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gpzztunag.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbsqnaqev.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ghipxyheg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gizbmzqdr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gpbxmejyv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/glypkiauf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gectvabok.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gmrryhlem.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdkfmuyta.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gqksxinqc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gsgmcywvo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvqufwsz.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gfqslhrlo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gdidbnuwv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gsxvpckol.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gmfiqvvuh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/giphqsigk.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gaekqineu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gxtdakmgp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/guoyzwstj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gvkdkekop.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gfilqjbav.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gerdcimvs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gpbrituzo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gmazucpjd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gttuqiasr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gcppnlehq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/ghztajstw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gslpgudhp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/goaspzrhp.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/glrhpsukj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gspdoaswl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gbkdjssie.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/ginkzhqrk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gukebhrtt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gmwogdnoy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gqjklcqdw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gddvvkxzn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gaabklitu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gsjykyijg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gsjrzhcxn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gkiiwuuxh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/grdvahdjv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gjlvifrsg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gaclqitea.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gftzbbbfp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gxpvehsnr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmzewdoup.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gedbpxfqp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/ghclgjqov.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guerktvhh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/goxuuqplh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gxcqlccwr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gnbrarjzw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gisqqgkfo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gjdfqhlef.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqomnvcpz.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gjzptleco.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcvatuwpy.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gsbsqgoon.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gxaanoppg.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gmyaddkrg.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/garufwdut.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gkexyngjf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gkvhurjay.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gasfcqmyy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gjbxzhkip.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gbahnfkug.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/guvrpttrc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gvvvfqmeb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gqlyuvqpd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gwexcoyte.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gqfynmyyj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gzrieqwrz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gscuifszy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gjmzqjlaz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gzdnlbtuz.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/ghgbrfwcy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gbiabkyby.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbtsuikxb.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtdjegrbu.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzjxjugzj.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gipmqvgej.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/ggfquqwka.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gciauecip.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ginlrnzsc.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gaotdpdgw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gmsswwdhs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gysbwfggj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gmvkgpxex.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/glryeushs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/ggxoulilz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gxjrchgqv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gwwhtdxao.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gwdjdtvso.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/geszvckfr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gxyzjwxep.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/giqytpcwe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gtbioqcsz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gykupdjxn.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gtigieoil.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkwrsbarx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gwfkomftr.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnpsaacjv.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gveytuemd.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gtfbdvrhj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gjqunasvm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gamfjxarf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgqjntt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gbmrlqgge.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gdrjwwnsc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gguhbasds.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gllrnywhi.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtaqylqvn.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gihzeipzt.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gbjuobrnf.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gcfcutocb.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gvpnrhlub.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/goxvxgmvc.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/ghwhgoqlc.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gluyjosxq.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/guisuzmhw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gvkgeypot.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gwrdshvua.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gkcwbzjzu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gzwxphgtq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/ggdhyryvc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gtfbupspq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gwbfumazx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gadberbhk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdgkyicqy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/geoqxyzfz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gyprnrkwy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfcbotqio.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gohoganai.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gzfgbtopc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gytvajtsh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gmdebhmjw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gzaggtyrt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/guivsbvdh.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjsicoi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/getavbxzc.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gnlsucwgn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtrcgedle.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gekdnoimd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gxubdqfvz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gqyarzwua.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/giernyxfy.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gbpyuquhr.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/guqufqhzc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/ghfdctlaq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gkvtgmjji.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/giiitloha.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ggcrmxdif.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkjzjjptb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gvgxjsrqg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfjoomlxx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gwstfefna.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/girazrdgz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/guvrnsqad.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/guurqdkfc.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gchvayapa.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gmtesswvf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gnvfoakxw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gbvuwbrcx.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/gqjovkaay.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/goozuggco.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gvbexxvrc.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gybdmoxed.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwqavyavm.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gyellopya.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gkrepwauh.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/grydakdil.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/grcmslsqj.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gbpdnlkvr.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gvmrjowxl.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gcqbjoyiq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gmttwejcg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnjuthgrg.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gztsepsrz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gjzxavqms.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/garhqxdib.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gqpauyjlq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/guccghwjm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gjnminnjm.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gkjuequru.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gxqqcotrz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gcwoilogl.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gezanmlyt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gouonzfyt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/ggtywqvvj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/gcpvtbxfx.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gyweqshbd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyknyvvzk.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/ghxnanirl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/gfhiuwqed.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/gprmreoaj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gpfpetfgn.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gzemvwwbs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/grwvdtzth.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gihqdvtob.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gnqvqqdjk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gwewrbmfb.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gwlmzliaq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gadvdvlhv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/gmbolgyoz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyharieyh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gnddsgqah.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gcoxtanxk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gluherktv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnzkymqpg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gylagqmqz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gctibsboi.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gakjucqlh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gzhvgmpzr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gmgnzguoi.sHtML


<!-- 参考信息 -->