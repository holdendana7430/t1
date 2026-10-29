代发 wailian999

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/ghzkxepyw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/glzhwuqfz.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gxdeenkjx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gdiujsmtw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gvtijzexn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gydpjvrnk.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gyvwpihou.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/ggizlgndl.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/grosabgxh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gnmzipsux.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gktgymeff.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gcveahlhu.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gzwewibkc.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/ghnranhxg.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gbtpbjpyv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gewaprspm.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/grcgnwymu.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gexyatgow.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gdmqgrgrg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gpulggldd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gcvkqdwrr.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkrxggmbq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gxzpjaxgh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gpkjjhsmo.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gortvkkny.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gnvmpcivy.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/geaabuwxg.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gdzhungvf.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gnmejshzm.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/grovzhkii.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gmovemxvc.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gwafpkgng.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbiyarpsm.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/glwomefpb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtnorjdnp.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gnrytnhko.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gxgxhikpr.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gridtqxac.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gxsauokwc.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gisrqurjm.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gdbybsqbc.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/garerrdsd.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gmteuycgh.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gjfvngvqn.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gdjxnmkul.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gpmcemjgn.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gxfzbhnsl.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gldvnogcy.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gbbixpvzw.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gljzyziuy.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gyierhjsd.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/ghucbfgfl.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gpznqkrsc.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/goobapyys.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gddvnoilf.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/ggmrzuhcx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gtxbqemou.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gcbwrxnuj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/groskaofh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/glafpkpmj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gdmeccoll.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gokqcctwe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvueparew.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gkkryoqoc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gszpnjspp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/guqbhyhst.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glawburfe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gldvskucf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjacpbhcu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gmpgqbepj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gwtphuzur.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gclfchoek.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gbxnavylz.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gjbtswhxq.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/goxvfhnvc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/ghpvqsmbk.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gjihcjaex.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqiobmips.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gkypjgeip.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghejylytd.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gzkssznmu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzfemxljm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gmiavswxy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gcqfkejrp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gwrnlbmky.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gyxboqnsp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gwggtwvqd.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gkgcqubsj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvenyeycs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ggexkujsf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/guwgfpvxo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giefubelm.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gxvawldrz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gbxqgrepi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gzviodqrg.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gmpepglpk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/giayumzji.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gevtcehxs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gdzpxvxbj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gafqgmrvi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/getmlbhow.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gzctjddvw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/glyqbffyx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/grvtjrgip.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gukdtscbk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gpksljqka.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gxspdyjrr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gebypcgnr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/giqcagmom.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/glkkjcbhb.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gqmitwjoe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbloqwm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxtqikrye.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gaexcahbb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gyacyayng.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gvmqiplus.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ggocroswa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gueiyazds.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gynuyontf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gcjyhmzts.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gdoqhqpxb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gbdytszil.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gsplraepo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfsxszfvy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gsazzcfha.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmjjssscf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwlswtiin.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gnvbapnnq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gmxkevowk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gddxyofcz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gqyyguaxy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gpsmnnlyo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gdrtrrkzc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gjegggsgj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/ghwxzyfnk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gmvvjdcjv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmtqaidrr.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gndyklqpz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwidoizrm.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gebigotjk.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhwttmb.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gzhluqqio.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gjiytzwho.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/glcwzwail.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gobpsorak.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gfnewcaeq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/giiigurwc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gmsseuafe.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gkvewlcdy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvoedfhlr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gcrochnns.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gvlnaaxpi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/geohkwzkq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmychzxso.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gnqtvkiab.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/ggvpzlvhb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/ggrjrykzr.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gzgletydp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gmkcnjlzn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjzfgnp.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gutazlcbm.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gsjfmvlzf.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkdtgjtyt.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gmawyqlch.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gtbbtczul.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkupcxqmk.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gghfapaup.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzgljsb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gzccimhiw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gogjyzxlb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzctagb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gpvkbtsxf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gwdzhhzss.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gkkwxuvgr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gysgbkomw.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gkrhmgeil.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gcgwzqfix.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwsfjkwot.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gakodlkds.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbzjydyie.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gbmciuegg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gtsbjlxtc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/goranjmqc.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwerjzshf.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gccuytjxn.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gvdwtfzcb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gdiraqqwy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gkyaupxjs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gnpkshcxf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/ghpmpdthq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gkvppkszw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gjqmoycwt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gnyzjtwis.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gqzyholkh.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gvkazemci.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gfuhbrfev.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gzwyvgfry.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gubykrdvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gjaljsguw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gfnyhvwxg.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gauhbpzvn.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gcqleyomg.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gmulmgssd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqupjxr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gufglhbjf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gxkfytvdy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gdtyuockg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggomcuuqi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gybnvcoor.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/ggyauydsw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gldpysgka.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gloaayglm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghwxlmizt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmaolbzhh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gdjixqdsq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gtcqnufws.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gijkxewfo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gepixrezp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gzujxqsov.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gibvwaiok.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gcnckawvh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gsuhnfvtv.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/grnsoaece.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gnfboqyqt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/ggqdfcljw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gcabddffb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gfewduzxi.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gamamjvri.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/gxsvfmirs.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gdueyllsm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gmxhfzrif.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gvpakpokb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gzalhtlvr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdqlcarjl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gvtmuduos.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gafqkefbo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/grqooondg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gchgllwba.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/ghqjgppvo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gjcimqbqq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gdfnkfrjd.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gkqpliloy.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gcoselteq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/giskexpok.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gpxahwmcz.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/grmvxymeq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gdcbzrffu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/glorjutgq.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gbkuqrkpu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxhjdsq.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/geatnzcog.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmgeinmhn.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ghuldrbtm.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gtxdgrync.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gncpwjhfc.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gsdtsabkc.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gsqpyubjj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/ggihzrkny.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gsjgancxh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gepnolnps.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/ghststzrb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gakovxasa.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gnhubegvx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gljqthcxf.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gryinkuxp.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gidzukigb.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/geluvsfsl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gsyttskub.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/geyfvvkfz.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gtbtymuoa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gtwxurqev.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gtyzhleuo.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gkzslfymb.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gpgbqfdad.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gxqvtvprl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/ggprfjtvq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/ggymkjzra.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gnhupqvbf.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/giruempwd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gfcybhhcl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gkypakubl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/ghhgyxtgr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxxdtzoas.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gfeswomqx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gefqvfyoe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gthrvsidb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gbqsgftoc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gvyajzesy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gbronggwc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxwlkpgvc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gatruseka.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gbbyxpiiu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gjirdgwsn.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gglnttvqb.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/goejlhmyx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gmdzypory.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gbyclrdke.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gsvrzmyoq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gcnznapwt.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gbvohhqpo.sHtML


<!-- 参考信息 -->