代发 wailian999

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gaxvszgot.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzrnyojz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglskxyw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gjagtueic.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtipktgxc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/giflrvtse.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gxynwkojv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsoyinym.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gvzksqdxf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxosvxh.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbgljim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gdifonalf.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvjliuif.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaqpimdc.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaplylfdn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gwrsckcwm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugmxmxu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvulprlu.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gchlnjcra.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gievzptrn.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gueqmrltx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaomkeuuh.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/grgusvpqj.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjziscwis.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohejmpzo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmksbpeee.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbugqzfe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/godlqrvyw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknnncmqr.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gwpvumvwg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gdqcnnvlv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grjdcmmcu.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjfastc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gdooigzxf.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gofnqwecz.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gpgzyqqmh.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gnstdvwjz.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvhkqqyw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/galnpnfyg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlktgojx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmsckyapy.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlbdwmgt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhgxijl.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvuksyns.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaokdpyzi.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gglklzxak.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guguvehmn.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gccfueqpg.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgnfbhem.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gfhvxgelb.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggvzaeojt.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/givmdrxzg.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwfqmzu.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdtczvsn.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqjqguna.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gwapkxlvt.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gnsymhboy.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gtxiwzkct.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqjvordy.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/greicxfwf.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjjuyoyu.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwehwcw.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrdoqlnt.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gapsktjwp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gueeragda.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/goygyakrt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjuogrm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpboyoqsy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzqcluoi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gapucahsi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzpezqu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/glctwqpym.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/goopvhepz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrznjotr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gekixzjdc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbofiusvj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gshhwcfir.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizdqjdev.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gzwnxaeco.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gikmynffk.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjpsrvq.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/glhrfsvvv.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gxowonmql.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepvjragk.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gijlncaai.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gsyqnztlj.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxekhjz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gaojyddjh.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmmjnzg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gaevtdkgl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gqesyxnie.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuqhkshw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gbqfmemzl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhksawkn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gyomgxaar.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelychdgy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gokxyzryq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gdseffjnp.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gceolicqd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guafblrxq.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/ghomoydik.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkvxetr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gkiaapmuz.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gjgozyhxh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkbrixnx.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbbfdzxj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gqngispbs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gxydchdls.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtimwmupv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbesloraj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdswvyem.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/genzzhomv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjioxgpp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtrowusn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwpyqbwk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gqkcsciau.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjotshkaf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gbjsfmzvs.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gmzggcbbz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gypunrsiq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqnqhjei.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/grunshuuc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/grvioqujl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giaefavyf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkioqtdaq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdltncnt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmpljcjna.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxgnsilk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeebifao.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grrkqoaan.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpbvsvmyp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjribunn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpytzxxff.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjkmsycpg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfliowuby.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxrvzwlff.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmmkthaxb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/girrfopoi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgoqldsd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/goqsqkcum.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpjcxidjh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfizttrno.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaxilsdr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaknniroz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghzefwams.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmplzojsp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gytnqjbrb.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcnugftj.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gpejgoxvg.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/ggvbxoigr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxcrhxdk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrymzkph.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwnmzpzb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqxgnkoi.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gfxalaezb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqxzaqxv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/glszgyscc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gejscnfwu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtguifht.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gmycyzpjh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gpchavbok.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gsttpekrd.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gycndudqc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtoaljol.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacmtlpeh.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqzjtcj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmevtnt.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/grtcfmyor.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqymitxs.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqmsszck.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdvltnqz.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gykykawcv.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotkvbtfx.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhiihhpu.sHtML

[A04] 判断变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gffbqfkkx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzsoexhf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwbnyem.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/goktgpagu.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlupzwug.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gflcaenyo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gmaqwoxex.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/guonjviul.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gluhhszmd.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyjfiurz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvroorjnb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsjkymtrw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsuwqpmb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjlmpngn.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gninoxoem.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gexkvoylm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdimdhflu.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glpsorggi.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjeoslcjl.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gadgbtzlp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnhflas.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqzftqcz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gzpzqgsgc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehzlpkcy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gubjryjer.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gnpoldnth.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfacewvk.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gexwwbxvk.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbjytrt.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsldwvuq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gztiqyens.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdofyuxzk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtccikoe.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqjptdu.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwuavkds.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiywoaod.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqymbwml.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtsupaks.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/geslmddmr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtslexehy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxbsdoze.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvtsmpre.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyvmwagw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/gpecabyyb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/geakfeqnq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzxighemj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfavtty.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjieaqrjy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrtwkqf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwgtjnkcp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyurqqvs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuyeqwze.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gwciitwou.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqddotrbi.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpmtsafb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdsrycsl.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fanxiaobao.xyz/Article/details/gtwvjipvm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvzpxfuw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxioqsywo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/getqzxsjj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqopggf.sHtML

Ruby: rand(1..100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpszqcgbz.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/geqawvyzl.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpiiyipy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnydjwsor.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaqldfsx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzunyjw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzuidart.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gasfhmfqi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjjknkj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqlactpm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/goscoqflu.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grpurrebm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggquiqkkn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijbuzyx.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gornebgef.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gipgmxodl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/grvyeieju.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhlzpee.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gosgalerp.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gptpptqmr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/glmbbhenp.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmngbvviv.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxajawj.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtogxiioy.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gwvrjogou.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gotfizncf.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlubbswa.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcyzkfz.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnysevvym.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gwdqaxhht.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/glspywvll.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlcvjgon.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gozcuyylc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkojaodee.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrxgrdcr.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gcghluvpd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gwganwpvb.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gdemctrsh.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gveptoptl.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/geeueczdw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gjqjzjqvf.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gruaysgal.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gmlltends.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuonkurv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdxkbmxt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gonixggqf.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gxdrhndjy.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/gseeudrvi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmkmvkhr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gorlibnxv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwaowzyx.sHtML

TS:   if (!x) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guvoafdam.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwbmuey.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtxguxzhq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtqqaswd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnpbtdsq.sHtML

[A17] 位运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnvituhe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gevvefzyc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gszhgviuk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/guyiugyad.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gqwerocfm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqoecxja.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcjcsvkn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glmnnnlfl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvzcevvb.sHtML


<!-- 参考信息 -->