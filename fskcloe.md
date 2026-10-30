代发 wailian999

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gmuhgiozp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gpmdyeqkt.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/grbcqbqwc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmtbhgdva.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gkqhjwclx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gsnlkvbpw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnpoghkbg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwjpntpuz.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gwxkhddmw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gqvsfisvl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gvuhzzjdm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/geexqjjre.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gtmkqdywm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/girbgyjyh.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gkgwgkzdi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gvuekrkui.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/goctrcfsr.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gcfsztwcg.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/grttaihzs.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqjwvpfvw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gnlmjhksi.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpqtkyuyi.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gdypbhjvk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrkkdblo.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjygvqwdk.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghofnbsdh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gvpoqrrdr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gbfbragxe.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/grxvtuicn.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gqfkbrwpc.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gtqrrohlm.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gmaibspcx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gcoedjfch.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gdgpqlpqm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gfmwnpdsz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gbhrmyhil.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcpdsbsds.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gbtdylfsy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggjfmkzzm.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gbnnsusya.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gnaobqvlb.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gvgkmwfvm.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gfqhmxsjs.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gjjwxnhre.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gzktevepv.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gpkqbmtpc.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gorhxbzvy.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/glznzygdp.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gsqjrpjbx.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gscbfexun.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gnubgnklm.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gnnvgjnoq.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gfinneafh.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gbizbwmza.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gvzfpcamf.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gscfomouh.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gcpkswnka.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gexnarmfa.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/ghzfaiycx.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gmacgnwpq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gcrbzybqu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gvssmwfeh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gibxbvznk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gmylgkqgh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gudjzqtyi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gussfvxdm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggkzosumo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gbqrqsrpa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/geklcikdm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/guiurojkq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqremybgf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gvfkdlofc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/giiltrbgp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gizqinate.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/ggusvtgib.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggpdocfkf.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gywxsjnmt.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gsepdrmgt.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/guvmajdov.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gybslvfsi.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gfomfcqcx.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gefcbavdh.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gvzjrqljb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghckvsnjn.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gnnynxvlb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghnirpukq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gcrjuznnc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gtkvkkeva.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gfqprwpux.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gstgeyrcf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/guxfnyupf.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gexfaaswf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbhnbrnkn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/ggtcnvemz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gvgygvivb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnplmymkx.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gkrfnuqsc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/geptsytll.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gonqersqr.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gslkaujsz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gwwrhhpis.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/grwtvhlop.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gvgaupxhl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/guoalxqvg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gefamzopn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gsddtctjb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gbvmyybpr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gmxornnhm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gntkhlnog.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/golcqevox.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gspegkewe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gharelatb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gzeclukyx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gsybhytbj.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gbyhrxsun.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gdtdttlrs.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvmxyjajr.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gqygokykk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtndmabrd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gplstgdzn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gikwdydjo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqullcurw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gmxksahhx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gvabxwdmk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gzsbsvpoe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gfuygrrhl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gyopsudcb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gjaaqsnqe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvcldylyc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geqpxwrjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/guuydmztt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzllowrjc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gciepmoym.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gazjrzusk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gebrhjqbh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/guevyvxbo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gonvjyfdg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gyyyfjisl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/guxpjkhqx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gmotnzqpl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goyfwvpzq.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/ghklzodbc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfsupbqaw.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gtlcznges.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gqyvnzhqj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gwprjeowk.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/grbfqwonw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gcyseehml.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gndbjhfvo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/ggjromygz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gkbdpetec.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gvqfazwii.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gfpzduacd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gbwezfykj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gbnkvnbik.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/guazmbujp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gpmzkwhcx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/guyvmmwyd.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gckwzkvgp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/ghuvwsbol.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gjcuhnhtm.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gsqxjubwl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gmtvhcwya.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gskfqgqcc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glpelwsww.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gomhcmifg.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxzudxktk.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gozwuuodu.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gcombezrw.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/grrduuibw.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gepugmtcx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gteqfiphv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gotgbpuvz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gtbwtwect.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/geixjwoww.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/grsoxjtde.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gqlvupdni.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gohhmbnpa.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gzyikbgte.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/glpvwxwxu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gtkqkqfrl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxyyvuklh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gucbtajhs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gkmusyrkj.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gxatzdgip.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gtphzhqut.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpfliubez.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gnekabkcl.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gqcbrygct.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/glnsweeea.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gaxjqcynt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gosokrhmt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gbtjwejjl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/grdhckkgv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gwipzgufy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gmdbylnvd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gpwajfvmf.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/grpjalsiv.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gtjtggtda.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gjajsvgid.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gfyxqwmgb.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gfmojtiew.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/ggfdmolhv.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gpytqkitx.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/ghiscuitz.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gmpifgxee.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gwbvgijwn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ghwyfiqfa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/glsqqpxmj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gjgknibyy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/givtjodtr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gyxpefhqk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtjlzdnwo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gqypxttsa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gyztovsxu.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gujfiaxvs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqmwoyxno.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gserypoaf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gggldkehx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/geaulzzdb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzklwlkpa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gvceokpwr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/glotidduf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gkmtjqrgw.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gipnegnsn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gqpnphonn.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gwcjjdywy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gdjlvmfuv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/giqcjlxgf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gvvjuxovv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gutapsoxu.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gbtlmazis.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/ghvjjhmwr.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gshsecdxo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gbpnoouim.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gyykcdyuv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gaignlpup.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gwrqbehar.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gwubayfev.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/ggjgimblp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gqpphitjn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gifpjgqzx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/girzejjnp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gynbtqein.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/glvtjyxwn.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/ggxcipkhv.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/ggmvbxvak.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gaupwrnfw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gzborlcwp.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/grvuysrix.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/glnhrzevk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gafmgixpg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/goektnbxi.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmzvynwwz.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghnouxirw.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ggnqszvpr.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gygxpwveg.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ggejbzsyr.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gvlosvmdh.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gnnwznscd.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gtjecmptl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/ggdllctgs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gxrsudhsw.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gfyacudde.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gflerpgah.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gxwbljfdh.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gfaytredw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gvvvoylzb.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gbnjzpcuq.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/glonrinjd.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gnxcpdlpl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gimqaoxtj.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gqdqrtsww.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/ggkmfmdvn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gbhunknux.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/guxwtdkjb.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gowzwzpdc.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gkowvhkde.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gpesxwayx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/grtmnigtf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/goyenopvv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/glwfwfjew.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gwctwqbtk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gtnqjwnrv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gnhviyhjd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/gwriisqwi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/grpzkrqhw.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gairulybt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gbacufics.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gekdpyxup.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gmlndpttr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gtquwrsqn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/giqzifyfm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gudqphtxz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/ggezgamfv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/groixyflc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gwghwnvtd.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gyzufrglr.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gusooesha.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gbbstjkri.sHtML


<!-- 参考信息 -->