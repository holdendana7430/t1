代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rlbwudgg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dqyzcdov.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tmyedagf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3imuoqzre.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3krmtzdxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mtiaszzh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aqvtyope.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sghbuill.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vgmudpgq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3giokontr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3saoqufnz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3drofhhqu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zapiclgx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3spzovxnp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vbjrypnt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xswkooap.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dmwqnmih.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xdrhuajd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xdbmfnty.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fvsdqnsd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3asxaxfuq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pvnokywe.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3idhgudqb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xvcotfmv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kxvxicag.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ymfqqqud.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3oiupikwg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ngmqwtvl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tvzbkehc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3eyunjzht.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uzarbrhd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zmuhibji.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lzghjtbn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ftbeknmo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fwfibqeb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yrlfghqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akvjtgbg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mrotpmic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmgfieen.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uggjjdjn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jpsqsugm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3iqypfwll.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ugrdowrg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uympxnin.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jsrjijma.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qkeablft.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qrvvwmiu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ceqklfzm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ffmcdcct.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zarnxnkl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hxiafkdw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dgmiwbhw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3opuuatmt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3adfbjkga.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lwdgtvoc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tuykztck.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tbuvrnoq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ipatcfyn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gfzzbmud.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qzicjedh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3drgrpils.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uacazzlu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rsakbsoc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ydryximy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yfnjsnix.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hmxdnevu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uebrdaok.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ilssnxgj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3houyodns.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3knbpibxi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eblxdoei.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hlfraqme.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rjduhira.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ytznmskh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3tsehdszq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cbfvsloa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rilrrucs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3rhrqntqq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vlkxuitx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wlcwspcp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3xbhgicru.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3edzrmqjk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3eckrtlxp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ktpopcdw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hnscddpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gntbilrg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3byfzmfss.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gfnjsrty.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hzmshorf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kgjisvgq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nwsqgscv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3neuczxvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyohznjc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ubvazfzv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lcfyfdtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neqjhppp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wskczgkj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hoomgjgw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nactcqhe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3aylvqoow.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3saveppjd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fakftora.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pzndvodc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3rcjvxwuq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gmclnyhg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wvynpmht.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3maooenew.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gefpzyhn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3plvnzhll.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qmgekosi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rdkhlmor.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zocsfsuk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3yrhjjicw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dvmhfdrc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zdydhbzz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tbuprlgm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dcghfkxm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qvgupqwz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrthyt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ypcwnicq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ypsaevwu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fcpnqvti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pznnqxtx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryeayrou.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kjxsbrrz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3adaskdty.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uqinlxhd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jcozxegg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3poopzler.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3leqsfybk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exctqkfe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrlfvoan.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xovxflor.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fpvchatm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivblpgwl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3krvfbbgk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axvfshlw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yicvlkei.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fnitbnzr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3alioeakq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icxkbtgg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rmgwzizl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szyhcoig.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gedvnlra.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nysymwtz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hxsnqxga.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zpjjvkwa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3zqnxxjeu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3eopowetg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mrgqgyyr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hqzetakq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nvvezhzk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ulskqimj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qybahqwt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oefshkyz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kyeghrby.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ybtikzut.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zsalfycf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3nktyivyw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3urssnkwh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nontuyjg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tfrxgzwt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3uaggnvnq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkyywwm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xkrrntex.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3msaygnkg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nwlnixit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vouhfgtt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gxbrhcxd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iqqzyoly.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vpouskix.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ydultzms.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jkaxisqy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yveeiwyy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xbtxgrhm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bijongjy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3qtnlcgyz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lamztogd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3olvbpfqs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3inijtbqj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3aljwwunf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bvfpfxyu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gxxyguam.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3baaafhsy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wdegmmhc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tzreehqv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qsicokpa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqmezmgc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zylgaoio.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3blgglgse.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3yztpaoxx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rkgnnrrl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tycmfhui.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ksgrzhak.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3piagmvkr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qdcifsrj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dsjelecr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bqjdxwzn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nxevofcp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ygxkgxkl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jlerjwdz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rgyrrxip.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3psbreikb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nfpgcfkg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3glqdoddy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lrvaywru.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3jvusoedc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ftohdhdv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3aelczpic.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qzuvduox.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bqpqztkv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qgvxnecx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ynsbfnpb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3dgfbugxa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yetmodov.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3orkkbwcg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbliwbh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3asfbijcw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dbhacaqz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lvbtluvx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zmgyjygx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vgguchjs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bwgznnks.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oygaowmy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xhovsodk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hytnkrlm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhabpc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jerjtdah.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pzlhudze.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3icsugcfg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ragqygke.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3imbajfba.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fmtkugbb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3copxfsnj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mlmdaras.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gfolcbrd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kfkohccy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ufkseomu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wnzjbmpf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nlsljsuu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ucwyuerk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kjhtnswo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dvmuzhnr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvdqmvkp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hnqqhgue.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3unxbzjwg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gvpcxnfb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qejuyewg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fcxjuzle.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xaannxfq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bzquotwb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ngddqkbi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vlsllpsa.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zofsakei.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fqgzacsz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uccurjmf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xztcjxzj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sbxankza.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nmwlcazw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3slkymsdb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ncnsnlgn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3uvxprvpk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rxjftlro.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3swaxrpwq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jooyasjw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hqwyscif.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ljjsdamx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cydddkmo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3itrdxpkh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kfxtwgqa.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvyihs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uzkwjqgb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ourgffqm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ndowbauv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3cexyfdrp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rdgptkoy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uhnutgpl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3irgbchjr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3naticypv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3isqfsmyl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ekohvobn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dcuecsjt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rpienoes.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3atrlxncf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nhudgmwf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zhyhbzxy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pskhbuva.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ruviduzf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlegidvx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ohpdntwn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzbdstid.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xfwneveq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdzujqfm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3afzpditw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iiwlhsge.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3btxxwnlj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ialyynkp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eykajplp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gixspxow.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3staimdhm.html


<!-- 参考信息 -->