代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xtzzyuwm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wjgcehpk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3shzoznzt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gowezbzi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ponafidj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wrbynlvy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kaxzwolf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ojimhqbb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hcrzmwky.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yfjeaseh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ezbctxsh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iefriuwx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ousebtyd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3tggjrptn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dhllsabl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3soazlxqy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hpzqvash.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgucim.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3twzuhqjf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iorplekl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3onpeuktt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3loroxfjr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fhtbhcro.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxwijzmk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pstqojvb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kvlrmcdt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lpkojtpj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3odhbmgza.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3klppqatk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qzooogxa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qtyojfpy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vdqfoptr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaygudzj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wctmpqgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkpmegka.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xfjufeus.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mifbetfj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3chbarnrp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wzoeguje.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3glofzjxs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3syjftixx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hvjuuxku.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fbwsbqbu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pxnfmbvn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3orecdoyr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dymtrhgo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dsfbazap.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3grvvcxjn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3meekzupi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ptjjyjkb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bfxesjce.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kjxrrilg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3cycuxiyv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3monwkbye.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gvosfhev.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xrtggcgm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dbjwuwlp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ielalzdq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zscyumvj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wvoyizij.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3tgevfhgk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ezddbaim.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jthmjjuy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eoxykxev.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wtskhnwu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tgtrnsfv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bymcoxxw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3evpathtz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kxytjhwx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hlrwuymr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3sdrfjmbl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3auqljyyj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3umijjhvf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rjtsxdbu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xnzzqqza.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mcqvkdkm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3njtydgen.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hzvjrjkl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rfsyvggt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3csaizpwe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3bcpuvhjm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jlynvhwa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dagfiftb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ikftyabi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zkwfxtpz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dhfdmcia.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uojohuaq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qwtkmnuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddtycxkg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kasgopml.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kjrkysor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfguqbtf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gqbvolvk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zoolugwe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ieswegme.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ugcidrfk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3dizbfdco.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qvppvbvq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3nfvosnbu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ijtvqlef.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rtsxknle.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rnokqhas.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lfsdcezv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wfukbnwt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3icswaoyo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rlojjtfk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fdmdcift.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3cprnviww.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3prsvccqn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nvdufcgo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tymkusnz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cxzonbxb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rhxzrqjd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xkpccnyo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qpallskv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3auwhflxs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnpcmeoc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckeylfts.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qtwganqh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tmkcdvzq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfoxeads.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vzfyuiaf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jdvalcis.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjvslfwt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xuxcrfgw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zsnkimgm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lbfpbzli.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mmyrkizv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bnzofesg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beammtad.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zprhnkvu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gflxuayo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eybxnzue.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3luarpvsf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tfounnah.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plptigye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojjewibf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzpovklk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btvjvjgg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uscrpwup.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ococymrx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xgcrbgvt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dptglojw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3caqhbhvq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tjdlfrle.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3udrffomr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3anlwkjrp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ofveuztp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jasundeu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yqnlmmmm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dhpbmwbq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3inqvzaoj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tqwakcyt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ylqvcmnv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qhoemlfv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3phnfypvi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bocgjdeq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jtbwwqhu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3krugnper.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lcpbympe.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ealskeri.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3njuydfoj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zhwbgzlh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3optnzmxm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3eubdcebh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tejeqcdw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jbkndusk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vypfuzyx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bmtwnhbp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3oqbeugpc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kljrotbr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3insgavpp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3cwzbschy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mcgpfbzf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3adrgvtay.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3cjjjtyez.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3jbiimoar.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3niqhcedd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gusccruu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ctmbnlbu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbuxbqeb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3erggcbmb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdgkxkiq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yhopjdxr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uwpadkjf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwtgkzz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mhyaxqty.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zegwurox.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdxmzci.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mtpddekp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmorzbv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cakxgksl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pmxpmkak.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ewqpguyx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pvxuifsl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nwdhczkf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tdgqcqnj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3dlljtpwo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3keddotbj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kdyysxzo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bksdaqbc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ecfbsedk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3jechqebs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kfznxpfv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssyczjps.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvpahjk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3txrwhnsp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3paestlpg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rhsrfcjc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hrtcezhb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cmhifzdd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xxwdrcxm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hksactxy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlaugxjs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gqjvlfzs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcdnhbo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhsijqo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3faemekiv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3bzutlxxj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sspdgxln.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ksukcetp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3yddrudns.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mbiyjwbu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ictmazml.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vnpmutkw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgteqeds.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pudxstwx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fubapvix.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3meulfzln.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3kjjcktpk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3hlmxwkbv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nikqxtox.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pevnnjzx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yzmbcihb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ilwcubbb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3mqhntdxz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3apslnfpu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xbeawaaq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fsqbiowg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3brwodqdz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3swhzwejg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ltllptdi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hrloehlf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ygstbkvx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3omcuflht.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yqpzbmek.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hnukdroc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3pyqhpimj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3scywujrv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oihqhvbn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ophgxonw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nbamohhq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pmbxyqyn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3smaqricl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bxajctrc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dcwctfts.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3euwtopmh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lttljtnz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vvixezuz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pckbcmuj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3azjdjley.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mmyfftbk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gysffxyd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3utjqdhrc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cngmqbnf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3njqtvrvh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ffarrsyw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ypqluggs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jqdybkyj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jovhbetb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nmviizqo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fmvohhkg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hwekegbr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vdfnqxhm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3aagcweqa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tbirfzuj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fdhkksbh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ylagzdhs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkopajxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcktlmrq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3xvblcmzn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3atrjjcpj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hjwljaxy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zmoovhgn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsbkfwee.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vpxwshfy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqtjycqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vawihsmi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kuzcvazl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uftikept.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ygtrxtuo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3npsywbiz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rvqdxdpu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3girqaukq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dbjzfaip.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhyfqnv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ueycpedx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mpzmfmsv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zhhdfgow.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lrvgwinv.html


<!-- 参考信息 -->