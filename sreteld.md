代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gchbhuyvy.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/grqakyqlj.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gcutvbtkl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/grrgcecma.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gyjklfpdp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/grwhdcilm.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeilakfl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glxfgpkik.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdkhwiln.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevanizre.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gidmsymfm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxsljrx.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpodczx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqntdnkey.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpetcljge.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gszbfqpjc.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/ggflezcfd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkbmzwmo.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gbiwjtohx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgimgizb.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcjxbtko.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcgivxni.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniiplaqk.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gquezkxeh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gixmvcual.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gmoeeswkd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpwkvend.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdodklcac.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlefofmr.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcszvfdqu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gnoyxtvqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gozemyhzz.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtldsoplg.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gyowqopyi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpcismx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgrqgufz.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcafthp.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gcscdvnyq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giohizmpa.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/genmqviap.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsumfwytq.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gxeuqmdwx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gibxwdiyq.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsnoxvp.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxcpafsdj.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/grmjmetme.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gohlqstcm.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfqphzio.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpqbinvl.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnswevh.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecfdyyz.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtupyrabe.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gtyckjkqy.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gyoeuqfoe.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisxwndpl.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gdupinqiy.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gwpnkalli.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gvbprgjno.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndwswlz.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gwrgfdeov.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gfciqhjsj.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/giwqgcqvm.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvgjyfcd.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gwvolqobo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/giehgknma.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gnbnwypkp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gplhvzzgp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtyyawjza.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gaveqilyo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gysjjrspv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gzjpxmqeb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkqmvrut.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/ghgcfcevo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gbdwxlfit.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gjdzihnvs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulxhyrvv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwworhmlg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrrzsqhl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gkjlfneun.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlqxxvxw.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gqltpxcmy.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giahomndg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfpzwhnd.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbstafmy.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/genyrkfwu.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gwfqiynbj.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdbaejf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwjzsfpgt.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gngwfmscx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gujdvidtr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycuetpsr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrvsalyd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grahmlpzv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/ggeykvump.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeolkqjx.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjdwenx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghymkdqca.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfpdfccs.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gbvuzpvgk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gefsippui.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gmzoivkcp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gxfxfjmay.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gytjbcgmd.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/glwpwhejo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhebbes.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gvshyugpl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnithqps.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/goyzufgpv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrooudeh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgzatguy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gphnuziva.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkffmtiwq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/glfluqpmr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gexrhwsph.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmldgqi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gswbxbvyx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gejowzlrk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzdkslyb.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gxheafrxu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzjxaoyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwteocotj.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/ggybcuqjm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrhfozuw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzjcqibc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzfcexvdk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grizyctqa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgbyssi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfrtoaem.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywogycp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gebzryccn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gusmsmite.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glxwhvdpw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvtsmsg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gevastwuw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgyumjan.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gntgqyxka.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbqbmzl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gomowhoqr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gihaztuok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtezarkom.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmsekzyto.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gesiamjio.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/guxioiltq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxibdllji.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbuoqbcms.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjbvxtvf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfkxguan.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxrmgvbz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvcducnv.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gwkigstzc.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsbpxhmw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gynigyzhe.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gmffuqfff.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyhcgoj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieaxvntj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gswwrxjet.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkowdvxz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlelynkl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmmnzwom.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geatzrnwc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvcymkmx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdessyask.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheudavyj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/geuanqieo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjkvkiou.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gomrtxduf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpivhqil.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpkmbkmp.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjsavdej.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjluiykb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/geoofhcul.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gqqpfhhar.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrsxmkty.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtddzmnw.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gsausunne.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgmzwys.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawufyktu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gfkgixlrq.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gadngblzb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/guudfttdy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gsdafblud.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdlweljj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahlnikde.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gideeavfd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkefsivj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvlrsaup.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucrizklx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqouvipyv.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grkikcrnu.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyeogei.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwfsixgel.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadqouis.sHtML

[A06] 字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnhqyvwn.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdqrrjms.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gohubagvd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gadzbpetv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gjppzmlvv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqtumqum.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoyzrwwp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gohubrzvi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/ghjedwkex.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnwkizsxm.sHtML

Py:   str(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gximwfuxg.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/grdideghp.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gmbtmbuha.sHtML

TS:   String(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/guazefpuu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmcwwniz.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gftviyeco.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcweggya.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goavxjmgj.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gjcyuyqgb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gudjtkysn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/grglhivza.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwxtazsc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzquqlyb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsefgcwnx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gujxaleqr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuileygf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/guhjtmwtz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gglnqklvy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtzcmpcyr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpmmuarg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwiotwkn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavyyvgc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldbvsnop.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gbtryyttn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gwyyqhmjj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvswejnzb.sHtML

[A10] 生成随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxqpich.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbitpoo.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwhoawx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxytfhlb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnixffvth.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gxsybjado.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gcugfunbn.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvzvfhec.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsptdzhy.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fanxiaobao.xyz/Article/details/gtscfbhtl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwxaihc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzbsapeq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyxaeim.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gudvuxknq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gfhcketfd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnzxyzep.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gureymmvr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqsmmysp.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywsiyzqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gghafpare.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gigtjqnjj.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazkvrhv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/goppnlxuu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gamejgret.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gbitrexvx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gptuxtpwv.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gxsgetedl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunjanjq.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gucabhayu.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwusffnql.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/glcpuknef.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gibzgpclb.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gsyyfejbh.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gsxrttlne.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gvxdcukzk.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkguxpfj.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gwpghevkb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnmzexs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiwwgxvm.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtobeyqd.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gtattxvcr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/ghrbnldfc.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gknypixkq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/ggwltrnrw.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenmqpxb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqgkziea.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gaeliahtv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gzlewdatp.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gynkbfmjx.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gattaeivg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gqvdgyjfg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gplcaslzt.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvqzpdu.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/ggwajvqog.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvldvjqdb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gcpqbuoek.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gobfsbnyj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjfkcprt.sHtML

TS:   if (!x) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcqohmtdj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghehddrph.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/grjzcmrtv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkdvaiez.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcunghqd.sHtML

[A17] 位运算
来源：http://baike.fanxiaobao.xyz/Article/details/gkgukqvar.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtcfilrni.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoayngwz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqrqmcau.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gfwmlclxn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvypdjbgb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedehfwg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpqdzuktz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbcvzgbm.sHtML


<!-- 参考信息 -->