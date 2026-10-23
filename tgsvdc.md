代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lakbvyqh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ykegjtqy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xzsbxmxk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fjpvbjzz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3whunzofe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mshfhfft.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rjehhwup.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3agxwgvym.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dwhbxphq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3oemyjlua.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uwxozpid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ashzaapf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lukejtpb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gilmngep.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bhxxllsl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3sgycqfvf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kvzbeenj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3umegfhos.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3fbstvehw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ukhxijof.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3nppyiurv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3idkledye.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qbsuftwt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ezpzkoqp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3swnhjzjj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vbjsjbfo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3oeuijjtu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvuikeqd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3malxxqjz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qsvnyidb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zbehinsn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3weuncwyc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3obnnsuwu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3trecpprc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vhmhutxk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ftvacecf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uljggjtq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3asprovoy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kklujiqv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3clncnzki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpbggcln.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xbrhcxed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdoilpbg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3djhrfhix.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xwmrfkwj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yerxzsid.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mflojmbd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wqwzhnyn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ukbhbhyv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oszqeymt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3miwtjuuv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3anjvseqv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cpnzphfd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hxjbhkfe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ybwkegxz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hhukexgb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lszxpkfe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3sjkrsnns.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3pzxzyjiv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wcaetqzc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3osdevnyx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3esopqbvc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ogblhuyh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cdjqesqo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lrvnevuf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ctuhlbkb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xxblmokk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lyfnzdbb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mukvtymd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3thethmtv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rwbcsqsi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sfwxwahd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3efvgbbqs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zclwbkqs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fffkbabf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3etbcvijr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jqxauegl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3javukzfh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cqnpvvnr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ltrdwbgq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yaigdifv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jmqoxque.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zrvadixj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3alzrutkc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3vydmgfik.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywnivkdy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3swtqfcjy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dujzmnzs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3llvtgouk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nfkkuaem.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3caijayyr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3swqbwryt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3baviwwjx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mkuhfxdv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3eglslnfx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3yofasdxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mckupnzu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rbrupvor.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3giuptjtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iywlhtfp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ngsgehxg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3etbzxyac.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mypbtvgs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rywkblte.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xipwavsr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ulyzeqhl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3efowhlqs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hblhpyxj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mvgwqcar.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3iuxmxewi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zcemedon.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3inkqqtgm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3iyemubzn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qnyjknrj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gnbchobw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3giwfzhdo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3izpelybz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3abjaukvi.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zsezulsy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3rtwcgybx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ghrlhdky.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3opdcfsvi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3edtlmelh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xqtdmzxm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jdonitqg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nmqhcslu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xaqkyybx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3kvgbtfpb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plvrospg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lstnwpnb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jdktinkx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sltkzlca.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbbvvhml.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vxgdkorz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dabfomhb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hslwqzvf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3chjbzlex.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3atopjzzm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3enfdorlj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ovaexpwb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rdkeugwo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ypubylda.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jadmrvro.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uxnipvzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjxyahsc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3uylwvwzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfklfjkt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pkplewpo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wrvupsyk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3nezwnsiv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ppqjajaf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dailrimt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3prjkmobp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fzqramzt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mpreifbi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yspbanab.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhtrob.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yiejvcoe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bnlqhudv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fwtajdiz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3oherckvq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrpqeoy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hprabizd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3esuhkyrv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jsbkkuoq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yhanueca.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mmmruneq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wpqffugn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fvttmipb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3seymreir.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3srjcorqa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uxrkureo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ukocqshq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3krblofsy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzmmrlcn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3wrlvgcxn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipqmfiif.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ngmpfkir.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3eibynand.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3upcantpa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gxpicdkl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nsodnrak.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ukujhalc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3draitbtv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hkcvjmbu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mydwrflr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3izlopuxf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wxczltdy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pyuzknhk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oihgqqtu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vnaqplkt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nvandgbe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ucgzoqta.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pldicldv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3iwuytjlo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zhbgqpzo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kjacsdyz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3triozbsj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3txjcecbv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3pnlybzsu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3iilokzel.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3mwdfxfzr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqeizzm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3nmklfqxw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tychjawp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3shakhusj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3rvzopkch.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3oifmqijl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zejbhgdr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3jdsoxpqq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zvwyhswa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3smnlqtgd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3odqsgshg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yckmoxah.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fqvguuui.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bllcsjnn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iwpfdake.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hujsyspk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kytjdmjs.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nxahmshv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mdxzoekr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhfjmwt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fchuiuqt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpgucwd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebqbnnfa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3uwjlmnbz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pumboxky.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aqkatpks.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tdjuskdm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xackxilf.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mqyrpyke.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgzebgra.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bonwrrbp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wuntwzvq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yavvihpl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3iuhnrmkg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ixkipzyp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rmwxburl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cqmfyzyw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qtcioxmd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gmhxckvq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ruwtgcld.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qpyuawry.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3djhlnmnr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nzcmvgvz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtpykvtt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3cectbbei.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3vmsopgoh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pmxodbyk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rilfdybv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mzycgoih.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ibrtpaaq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqnbgjz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3aopgvodo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3inqvjwri.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jbiazcck.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xzmbtwaz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zuojjqtq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vmnkkzbh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bzwymtvb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sazlysqc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rniowluc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ojocbowe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3slhhlgwv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rlxdhryl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3jbzewmar.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nzudcwnu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3psavkvsn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgjvje.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3azxsvlmw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pfkcnoak.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ffskhbey.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fzuykmbz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vujjzzgx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ppemuubg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nuveoulh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hpjvhnks.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tbtodqib.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3evhnnecz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zlzjaayz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hrwzvjmk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vtzoowkw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xvkbscfv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zvjtqhrn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3vchroidg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3aeiovinx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ogzcseae.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qhvnkyll.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3goyuzpos.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3botmwxdo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vkielcdt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3bolfvoah.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3igcwoqks.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ceheozem.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lqknfadr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zspmjbuw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnhpkdhq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdlwvwuv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkzkrjna.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnszxjpc.html


<!-- 参考信息 -->