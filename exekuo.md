代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2avwfpkyg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2urrcldjh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fmrsnwmz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kfrwthyb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kbhxuqak.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wlruqfnb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nnxsrzqh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pxcpmret.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwncdkcq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2udpgrviy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bjuccmql.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pubaryaf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xzenqqyq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2alvgbqub.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xltstymh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mxffwaiv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2frcjyinj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nnighhwd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2euinbjjo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zogaeydn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ekjrcpij.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bctfvjom.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fweittoj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmuaddre.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qefsynrx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rqdjfrxc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fyyacjez.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2tvuwkafa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jvvtihxb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cjqjbjzy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vtptfeea.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2izarffue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqfevhpx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zqcqlkkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqdsewku.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vepfbuqo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lqimajti.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wuegxccz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oomnpyvm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2exqkxtdv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nuirsgks.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gpducuqj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ofpzxmtd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zltbjtzm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qwpvbkhf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wlgkzdkn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lbfyeqwz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wthdtnby.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2psrcmcfx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2anookoyr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vfxfragf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ldjrjhsl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dtfvveyr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mbobimiq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bfhdcmlo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2aryhcgkg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ioligcxy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xccmudyp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xyjmybdu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2olrwnshk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kfltqjxy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ywxkmcua.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xpxdfmhq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2prvatvvs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dmhdwlyd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2giwjafkr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xhiipgdk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cchvgppt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2byptgdvn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2axgzxivm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2btewuocc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dhfkiabt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmeodv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2suqhbwrd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qfcwzsjj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2czbeypaq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xnzqxzfl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lrwllhrl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2smqfhbiq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gspylboh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2epxizuvj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qzrjsquw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2idmpepct.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2agilyxfk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2urpdrpqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ritryuky.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kwlxwica.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2utnkcmjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziixjwwy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vidwruns.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zffcrmue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivhnmzqq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ofzxmujl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rrqcngdf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sqycglqs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2heppkbob.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pkwknaed.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2yaoikspb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lqabdjjp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2pmxxwezn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ryhevcdt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2sagydfzv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gfndxdwn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2juhfuntz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2oaewuucl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2biccdhya.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2sexxjmmn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2dsolorjx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jqenqxxa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mesksspp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2cdetuneh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tkqgixjy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gwxrfhyn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ydfiwxsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2etkdhxge.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgyvvuyl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyavgzrq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tkdsgfht.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kxblxwkc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxqlqhqm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocjnublu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ugwirnxt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hguqsxsf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yboovqqp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ortcyowt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zldlnbdm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2doihygjs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fksxhcoy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykelzgik.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkikxc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dawkbzxf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xvixkvax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsbndtmn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eziirhbt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fdgcrmbe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2glestdtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvykjsev.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ftbbkams.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbgkhkwz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qtigkghb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ijfgzsgs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qxoxaoqa.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jdmdvoud.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ywtivoqs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2etjtgled.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2emzsdqhr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2dgdvwopq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zklhpdlp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ypagremp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2sahrcayw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qbcrwqaj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ehvcvkps.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jjfiifre.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uyoziolb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2venzmvud.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2fcoarfnc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kvemgfbe.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2iuqzqktu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vukofvbp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rcyctnri.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehjhhaqm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ebkuovwl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2trxgvmhw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dxtclger.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ftznigmr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fzfvipit.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2znzfhpwb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2itrywwlu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2erryuync.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bowwileg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2snlekoiv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ltaclbfa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dzsnkxlt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wcntkjaf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qfdqmwcg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tyqsixvi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dolxilkb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqvvhokv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hbthjqkb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwwgsntj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmrtslcl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ttcamjvk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zysezypz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lqygikiw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hcqsstrf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ryyxergt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2japybcof.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dvskifat.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qvuyunzr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bosupdpl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2klbdllgu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2prnsnyhb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2asdlsnjo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fichuarf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2blkzmujk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zrqnsakt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kdvkgeow.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lpzabesa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kddjzfio.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzvzvkd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2aafpalud.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdxuxnet.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zyrhiufp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bxuyaqaz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bhaklanf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2svhsepbp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2soylpolz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gldntwau.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkblztn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2itgicvef.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eebapjjg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wswwkrub.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2imnztsam.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2baxkhfgp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zccqgsdi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtrnzemb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zbmxegbj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2szwiejst.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tnkvztub.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odvjzhzh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qlfdzlwn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2yckvuesy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhjojx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2swuhgyyw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2btvbmtqs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvpecgwy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2pwlilrmg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2lpetwvbc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zfpcpgac.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2lpdmogdm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2umcpaqxg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pgbuzsjv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mlnrlyok.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wyohvwzj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jcamsqbn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kpfingty.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dixdmhai.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sfzzdvhm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2tpfaqtep.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rebjacjb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2uzzqjlnj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lphkuyba.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2drccnrjo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdtgden.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2gfbmfziv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fblrrklp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fzqxogqy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zgbtdijx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jkbjmjlq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2baivinzf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bekamcku.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hqepqsdu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zrkxyunv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tuwhjnkq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uajagziw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dgjtmnsn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sdoytlro.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2aermxzre.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mofwomii.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jcacknim.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2plbgyxbe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ycfewtxb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cozvhnth.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kygklfmg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jboylhkn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ipmhfrbe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2czxzaiex.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nmwtkbkz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cgravbkm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2codyclvr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2orqwdgwg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gihjsplk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jhbxadls.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sekcplkb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ylraypjt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mohwadkm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zeomkkvo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2csdnpwso.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enaiqmjj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tabqkeyb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kcnapdbe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2izdfxsrn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nszxwvsm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ydgoltjm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ftlvkcga.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2guznvosw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cmhzrzwt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ikmhymin.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jciazmwy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2unpucida.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azrkrwkz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eyenptaa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2kayxidrl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hysrvrgv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nuiwzrcc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uklbyrpl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2maamymrw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2odvtgcoh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2khuegvji.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfrxay.html


<!-- 参考信息 -->