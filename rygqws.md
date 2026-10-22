代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nzogvtra.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tsjwxahx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xzvbnxme.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtaqroiy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2uzypccqd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2twufkwje.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lgdspblp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2upmolstc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kiykvmro.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dvwkmtzk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ggzkqmab.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2udqvopqc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qwufwwpv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gspcsptl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjntxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qmfpepwz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hpzzmguf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tvubbsjo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2azwpzdzw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vbsrnzrj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ohgowyok.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhwadri.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ughngxrh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xfnmmqvg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vdrkmgar.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fylyvnxd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mskvoeqg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2coputiqw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ltowaptg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wuymppty.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rlcdwmre.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cxzaddur.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pxaevcis.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duguvuri.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wzgpplce.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhmnbet.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2covhrrys.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dgovnzcc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2phgtjqfs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2duvxspfi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sjqxfjnf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xcazmrqp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2yhwrsmyx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vmxvxtkx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xfvlodyy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zsobrlkb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rywjtqzy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dzxospae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdyewcux.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2uxgdufjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmejlvxj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xgtqgwqi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uoforrbt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2sapjzxdk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2zomwqmwb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vohtbzkq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gpgokkoe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dunoxxdy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwarrugr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vbrgsges.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dwnogooy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dxtxxtkw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2abhiofcw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gssvbfho.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tqnigftu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2koubbujq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wenmqqez.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nbphxtej.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2khmnmmsw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gkgifidy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ipwonpqn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2snzqpfzf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lxtcqxts.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xhagzynj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aibwmmhg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2razahumm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lnjpppou.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2owbijvxg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gulfibdb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hqawocbs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mqllcffi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sdejplww.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yogoldyk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qtouggxv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cnjuwwnj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2adwtruvs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2imsobvsk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jqgjwxdy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dfrhozwq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wyjrjbmk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pnvwazjp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qrekmxmd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hbxdelci.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qeovjaup.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2exryqtna.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iwmzbivg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ewutzxcz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vztjlxoe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tgqhvlzl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2thzozdiz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jmioqism.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2uyjbdeci.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vzhsotar.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jhhljypr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwkhudhd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ohuxgljh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ncezdlfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezjauefe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2oezbsles.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2vycalhjm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2snfqxnnf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hgzhtyjb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2imnoguba.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2nsrmxhho.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2grhabkda.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mqshdhbg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ofeegfsu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rweyckax.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lpxuvmkh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2bnrazqfh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2uhdomwyf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvbgxg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wasmobqk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qcewvfim.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2glhqmgfd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uycnfelp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ukzmhzbb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2uxwcinit.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gakearjy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2aaqgbkth.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mntsdxay.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyskaufn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xjzawobm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulixfbkh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2srojqxpy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2loelksbp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjocopqd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pyozxkua.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2brrgfqqn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ijhzxoej.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2utxmvnuj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2udpnwblj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mztnordl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abobhcyz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dqubljus.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vveauxem.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zdtkfsnf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jjqgdxbc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pivivsez.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eypawjkp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ktgvbdnd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tvwafadj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxlyavkg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgleqgpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvptvupz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qjivyksc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rxqyxkzl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bqzzdkdm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vapkyiwg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vvsbrqhs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fgzzbowx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kkfmaunt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kcwzeuyb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lxnakrat.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lmhldvhw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2qjukxdnx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iojggowo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fsnfkrkr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fdbtqfeg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2otlrohyf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uolwsogw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ajrulgrf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2poppbulr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2avtaaovs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bcxsnvzh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nyhexyfi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrgbvko.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2khecbfle.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aimqoxqv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rptnykws.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tvbqkjqj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xoboocgz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mutqayka.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2iohxdgvi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwchllwi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zcktiyik.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yzjrvnqj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fhftimvn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jzkukbpv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2cbqrdffd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2iwdtwbpn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jjpopbsx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dxwnbwbn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtsdehus.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gcrwhpxk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yxummdrb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ukiyrusp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2glwvudcc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fuqsbpcc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yvvnoovx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzkgymsn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2coaijoro.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dvybqpfi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2iwwregce.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uogwmksi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2blkejgyi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uewaukrs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2puurwzad.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dzlxyuwr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2gyvzukrp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2adtujhyc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2vpilsgxz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dysfroht.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gfvktdhv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdkshmf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eszmwttx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kaduirro.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yqjfhhdb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2glhafvfe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qovkybgc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwavlthy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bjytzirg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xdexcffq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sueckgbe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlkfaij.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2scqgibss.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2efgsvzwf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tozrjnpy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2muzhcqcp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtllrckt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkdujvp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2txixzppb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2niuseyfm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2afbftcwa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kmxuznfb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2otqxdhhr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2puwxusru.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2szjplreg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2umfvqooc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rowgmsux.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2npefimct.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkjndsdr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eymdtyup.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzukhne.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pukycsef.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2elerzcgb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qdfpkzqr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bixktmmr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ajfhqcrp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zhdhduzk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jeqvwrtd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dkbxusol.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mmtundxq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cqwsbzjb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rhjxmsem.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2elzmarkp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2evdjxweq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2msttscfh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vruuhasf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvands.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jdthmhdo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jdbtawra.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hbwerdgy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dzkhjpnw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vfcyttnh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uvqeorrj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zovecjdw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vexgezco.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2stjbmwni.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gommqjvd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vjdmewzo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jnadbkag.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xtdspgom.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2tnliolpu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eoranxyf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2npdysche.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2svkehyow.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nffluxcu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vdxhhemk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2olnyucjg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2czoikiae.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cbwdssyo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hdnfbbje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fnmcdxtf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nxgmnahk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2umkorudj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2flolvmra.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2upejhggg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fdmoevza.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xdhhthaq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjlkjo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kbuemsxg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wdjatyvl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pujeizgc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pzgcnqif.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2caodmnkm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tmmtoidk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2whkdwdlv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cstieezv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jolswskb.html


<!-- 参考信息 -->