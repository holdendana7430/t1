代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bxpfqfbd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kovuahdz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sxanqzla.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wnhdqqrh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ejoqhfxv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kctkhlfz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3drbgdtbu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ijwynqeb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eopwrrwb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdjlbbv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lqvbuzyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ajysudcb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eofidjho.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3euwimfpo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zyrfqgsc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dskilewl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ievvqraz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hnwuexsd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3apvvzcok.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oweeubuo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jpfdbvgn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xouvyiad.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dqrsvyar.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arhfljvu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kzgqewol.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xtdtcqcv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mnkudjgu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3enzfdgtd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3feirjqva.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tyurlgly.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bmwoddbv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ojutlnrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kngkfncf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gjeopcnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ellmeekk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hsacwtll.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ohraodfq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pmhspqyc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xekkoeag.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3abrwtzxj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rxpwtzrx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jztolsti.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rzjckeod.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ummnclci.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hgibfcxp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3urjxgnfn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3galjfkum.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sutqlzyj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ckixtbey.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3azdmyioi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nsmosxil.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dgcvzzwq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mkibxygu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3esefjcqy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nbgoslwm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xccymovj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lpvesdwx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eelxifua.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xtkkirlv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qziffzmf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gijulnnv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3emyvkmbe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3puunkjgi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qiihmyoa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ekjekfnh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zifgfpou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wrjehqjd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fjrnoiyb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dorrfbey.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ilczoind.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tbkgxunj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yewgqveu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3tvccwdhl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3iycyuvlv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ebqprwjf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qkvctjwl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lcfydngh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ffxxbhda.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lznsjwba.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cazesxus.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3isdefige.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ilpbygqz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rrpqcofs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3egwcubkz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vhbbgqir.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3goxlsvhu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wswpzqba.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3wgaomxrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swymvaid.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zsugpqje.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vnwovtsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbwtipzd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fahfjqff.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zokqkgyg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3imyhhrrj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xmbvczgw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3umflkyar.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3luzbuchg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3uakrseay.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vivhkoei.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fguqxbxp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kxqeuyga.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bjwseqnq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rszsznvy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rsfbxlss.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3fojmejkn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mlogmddr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3pikhwqzf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pgfwcbsk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kdidlxql.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eclvdxhf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3uzqwvwtb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qobuvugs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmhppz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3smvkexgz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwfipyxa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxrugslr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbkxbabj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3euvkygwc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gdihmyka.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptlmpwwm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dabiisim.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fymqectv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owzikpqm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fyxfklch.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3chnpanxg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wzkewmzl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xtedpxmf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xuwkzrce.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfamoysn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umhcebnl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfshyyxi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcskddqf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lomujxcz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qipgwgpb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btitxicw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfhafzyo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dpbczuku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soevmsij.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kpomwnqj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tihkygee.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qgauxihu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3adjduzmw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3uglwmiqh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rkeeqval.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zgndegzh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wtktftrf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3guaovymz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dxrknkiq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3iruxhlnx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3enbdpeqn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3npxocdui.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qahqxrig.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mpzimfig.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qzzxujwc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jqjckuvl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cbrrkijm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vluibhmr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3kpqgarbf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mkllztvy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3chpktkpn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nrnthucr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zcgoezud.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dopqdsqh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oqufjadn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fxicuedd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynngtbcj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dxoddgbn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkozrpuy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xjsbeudx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ltarryvd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3audvqmxw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hfnqbqhc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmvigsj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3euutgbam.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vonemwpj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3uroyalbf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dfswmjag.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fiywqtak.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uxwlbhsu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wxvlpjzx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wumtplcd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrvlumqk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gxvuvpfq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jvflthxd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pmhaefwu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3vpnuodhn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cexfvwjn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lukmrstv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pzdammll.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3adtyzbay.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fyuidjzn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gpeqvelg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cagqijzh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ngnlblmi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wbghhwaf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3eyvzfdfh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pijbcalk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3fchytucy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rqbfiowr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3eobwuirg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3oolalkvu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wbtoiwrl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fgkpcodf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3urzoqzaf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qhuczylh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3cqpjpahz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3swadhmst.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmxuboo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cglxuncl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qnckkbfv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eixvmbzy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udtiuotw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dnfvflav.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfahygc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jceujdtv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klqejnnu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3woobirav.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jrbklvth.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vvgdumfi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ewpzfvkr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbgqwyp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jwokznve.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3brrijwem.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pfupovcx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pytyhxmj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oewhsndm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qjjufzkq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3eqghlduu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3hprtnmoe.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3nrcxtevc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zgphttdm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jcnelzfj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zedmvkom.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hynomawc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3clelclvv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tglyrtsj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yuutkkac.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pmvrdlan.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqmddtyz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mganovtl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hstxebef.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bzhkpayw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxvidgw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfiughd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fbkufpzk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sakcotzp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3igoedtnd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3icfwvhwr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aslbwfee.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3izhtrckn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bkdjcvmf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sniwanox.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ralfhmnv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dtzmorln.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3flkguhed.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kozvbmdh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xwirtwyp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hoblthyy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ltlxsiku.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yphtxasi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3siwtuxtb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmlqtehw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ujzixpdn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lxsgxlvn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3psuhgtqj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3azfwpnrk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qjghzxmj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3myfzbawx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qykbxzke.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wklaabao.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksruazfc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fpjgpnas.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lopcybbo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mrwfnsrb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3llwlqvyz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3coocmxoe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pswhyaog.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3agqpyfjk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lziwjarx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ovsznoga.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xjgmyzlh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usckivjh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gngzxned.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikqansfj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmpxtpei.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3smtwjdpq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlybdzyz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lmdbwduy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3owyivyoa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ofrtchyp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3junefrxa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3cvxjugwd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mduywjkm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zeckgakf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ldsvvmot.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qqqeajsr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nyycaaod.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3eanssznp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3azbstrmz.html


<!-- 参考信息 -->