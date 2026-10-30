代发 wailian999

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gpuaeuobr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gnngauwox.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ggrfcmeoe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gotvujdvw.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvuunyqcy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gahsutvjn.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gvzshafvy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gboghbcrt.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gypqqwgbb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/girrjznqp.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gqkrtokpc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gxaiwxrql.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/goaueultn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/grqexnonf.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gwmvxmyyc.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqibjwczo.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gutrnescs.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmsjwlmam.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gvutqmmeo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gicosdnzz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gldcmtlwk.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqxmjvgqo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gtnrnxrcw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gjxxbgogc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gfjjnuvhy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gfejdspzs.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gufkzzhvq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gbdbpvtwv.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gxkrptxah.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gxsishlyh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gcpguarfd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gufypnfis.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdjancocm.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gdzzgalde.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqsfcroti.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gsmvlhoof.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gryffhvia.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gvxeyliob.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gdmzopipg.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gxhahbsqr.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/ggiqomyrh.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gcjknfvmj.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/guboubcvc.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gdkhvrbih.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxkufer.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/giuunnkyd.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/ggvvmlbsp.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/ghqulplpi.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/grdoqktkp.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gthmwboci.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gpqbppork.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gsrbxqmlv.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/ghysxwpbl.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gghbnkqht.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gknzwdqhi.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gdtcirskz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/grdixgodz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gnvkmwnne.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gfigpkrdf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ghxpilejg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gtxyzawgw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gllpzzcjm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/galhtsvhz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gqecyactd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcmuxrcaa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gchgpdphg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gsscmrdlg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gbgsotjdy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gmffqrgtf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/getbwiuyb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/ghvhzgyhd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gwrvhkxno.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gjmxoegnp.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gyndbfxsm.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gsygacqoe.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gszrpvbyb.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gwmhqvscl.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gyqlhamch.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/grtoplkwd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfoiwkoak.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gebaejwun.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfmzkqfcr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gzdqawazo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gaxvfwonb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gasivlcsp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gkqajzhud.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gbzvmsygy.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gtwfzahnj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gekusknmt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gokslqswv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gechijmco.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqmxhfsuu.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gqympysuq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/glgpntmcz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gpnittctv.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gtskabddq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gjogofyjj.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gfhidlmvj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/ggihrqgki.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gxcgaqrya.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gydnadhug.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gsudyhvnq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/guncgmsag.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gjqngggar.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gaanskpjh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gbmfstozm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gvtntkiwu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gxknpaymy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gopfprfuc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gxtznprxh.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gtpjuytpe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gcvgdmlnk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gajxvbhdz.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gebavrgxj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxjnjpgzi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/glcgqvdeb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gzfuhowki.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcpagpynx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gxbessfjy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gilgxhdvw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxxfwwtvs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gtltqewci.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gtsojrlyk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghptgoqzs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gzqzcvmqd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gupvlhljt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gojsjrmjv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwxsxupxa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gdmvlenzk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gkipxphwj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gzxnrqfwe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkmgrghir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gaafmybhh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/ghmjosdel.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gencrsabm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gixzrgklg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grokzsceg.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/geylvaihh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbyxjmxen.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gidwzoqaj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gumwyxufj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gvirlxhxq.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gmxkmpasj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gcamvuhnv.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gnigzgwxj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gvovxdcdn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gaarzqblo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gxmndmqms.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gnfvpulqm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gvhxnioze.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gjfheygkm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjaxrlfhi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gtvmwbvyy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gacozcepr.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gemtagmnu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gseaxvjkd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gzvrowstv.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/ggxdnesjg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gwcogvlrf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxmxvgysz.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gksapjsxb.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfcplucth.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gclvhkbub.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gsgpyzdye.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gnabkwhhn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyomgbppt.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gdsqmirns.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/glquoriwd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gxtvtqlvx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/guyppqglc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gvwrojfsl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gfmeripbv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gzdkxmfhk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gbsdupyoh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/geqohkzom.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gkikanywm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gmtvmzfca.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gaxevzivk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gkyotgksp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gyszqsebq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxaxzkdzj.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gaencqqij.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxoshkgte.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggccoywwu.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gxpjnpfho.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gtgolgmjl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gxwpejdqv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/genmbigri.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gfvcwcfpe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/geaeekoej.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/guryicyeb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gpyvpjxkh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gkhzeaxrz.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gzkwzkshk.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gxfeexqua.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gkobdphax.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gawdgcbnk.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gttubogew.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gfqjvxkqb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gapfwmqdx.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gaiuodfit.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gskevpjav.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gqyllogfl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/giblwheoz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/giztfhwmb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/grcfsyiif.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gyxhthyjm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gbrfwmuty.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gizfdcpuf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gmxrvsjsi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gxvvwhvld.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gjgnmbxgn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gkhungvld.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzonriwsl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gnkjwlawk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbdqwvszb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtqqufkyz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gfwwrnabi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gjdxczrsv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghxnbdojr.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/golenbnls.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gsorzrgnp.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/grfjvjwqy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gdjckzjly.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gycdcqyxl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gklelqbdh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gddgzffjs.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gxhzkqxwd.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gobtbbpmt.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/ghvobsmjy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gtabnvyqw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/guisunnwx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gsvpuqdfm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/ggvoseguj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gmgnslggi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/ggbknqqdl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gykuptoew.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gdigundic.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/glbbdjnwc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gddpjpenw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gvrxtxzqm.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gpiadjdxi.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gsqszxrnm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/ghgczsdhp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gzdopaqts.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gcilfisoc.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gmwfxycua.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gymfdvclb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/grrfoegxi.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gmfdkfytd.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gykhfoqof.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gbnnbxoiv.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glonsvass.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gizwzcunj.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnhtfdcwk.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ghwpbabsg.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/gabzqrpmo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/giinedaco.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/grrstshzf.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gunnuyayi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gnukxyaud.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gftsowrfb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gfkvfytzq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gosmcawav.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/giptefufd.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gzwxvintf.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/goqkwvucp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gnjhhuola.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gzdzdlyel.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gdoqqmted.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gtmazwuge.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gzivfjjjq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gdksgmjkw.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gfhmrllfi.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gowgpwxth.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gjqusaixe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/ghgrxwfzz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gsnddwalg.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gepjamzur.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtegmtfrh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/grmithlsi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gpksszxud.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gtqtdqtvg.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gvuvycapr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ggauzfwah.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/glagigylo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gdxaofmef.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gjyohpved.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxkpvwwjs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gcazgwcjl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gohpkqtzi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjcqwwmmt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/ghbjnaabl.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gjmaavvvz.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gfibwvmby.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gygvshuoz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gmjsrwbgc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/glexbnwct.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/geodcaziy.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gjdjsmuqb.sHtML


<!-- 参考信息 -->