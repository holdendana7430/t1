代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rlfzuulp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ckacufmr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kaasymko.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wkshotxo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zskbkqqi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwvtxvc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dxbvwccg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xwjbdteb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rxgwgmey.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kcwdcrtf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tqnnihyg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sjhcsews.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tjrztjxu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2npppmdfw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gtjkfixy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tnjaafwn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qkjtwmrp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2izjhwxro.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2umtatamm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2muibabkp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cflyuafg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lgjcqllt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qvbnjghz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgxdgztk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ssqdyffe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kiiwaxnk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dpvznouo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2arhcfavl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xirgpeez.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qxqziwlr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rvarmsie.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2aenltrhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbpniycn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2djaeqvwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgqoajrs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pjivjbdw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mxokjaly.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ykkhhqwv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gbygkcvq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dmrsfrga.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mptftdll.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kduejeqk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lcwnnjzy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zrpucsxs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yqupvnuu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2twpjbtcb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lzjdxunx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2gvscahtr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2igqcnxkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xwlpxonn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fhsehapt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2tjpvsxzj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2smycjzad.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sollhais.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcyibz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gracctej.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2odglhzjy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qhuibflt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wekvfwdx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cqmdlwnp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gyertncf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yaxwyeqh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oufcqttq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nrxeaisb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gxopskzg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pztlawhf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mmfoczvr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lcghtwfu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ywkjexci.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rdztzakw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mcjojiro.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2crakbwji.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jiqmczqt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gbzmbhjg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2aysrozst.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2swmsfcii.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2auiqjidf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yathoqxz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xdjosprj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bqfbqsth.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rgxepsro.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vnsnuouj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ptygddlt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zghbocwa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yvcayywb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zbtzomhw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ttrvzijx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kaazovno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcohaitp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2anwpsbec.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2voznwzxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzahcoxd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ksnakfin.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gguefojc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2isbgagdo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bkrlanhv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2vkxhwydh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ktcinacq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wtipofns.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lsivjwha.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zyhivqzw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kefrucxq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qzvhhaek.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2hhowdjdi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ieisltor.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2hmupbjal.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wwqimtbm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cyfqwkzf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2lmimhnea.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2drpfhuxw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nrcyofzt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2acyifivx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hyfrwtkx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ekwsikwo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zlikuzkk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2djpkxprm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pxulqhvv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blftgoxs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rmqfhqmj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qgathvfc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wluicypq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrktntoy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tugknqmg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wozbrszy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2goyntzcm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rptbctge.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhtmlelj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qstlsyev.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2duxxtavc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbdxbujz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xmmlmqoz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ryzoasot.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjzyojii.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cktqckcg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uecprqsx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zryiewwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sotdotma.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzyuwdzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzwrfmkb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2etcmgdju.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pmztvlca.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hrfkmguc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xugqmauo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ltdgfkpo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yepunsdo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnlzmz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hlzvxrqe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2twcvboos.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gzumgvjp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ktetfanx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jcockjjh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nnyoqxjn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2nimzbagf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aeodfbpj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xhmuqpsl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pyfxukfs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lfuvwodw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2rrzcuwvp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rhdwrick.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwzgkh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmjjzyw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lihtkpxo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2thupvxaj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gnclluna.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ifqljdvv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2huldfuyt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qfelbkuc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jzlnvvsy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdjqpgs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2omyzjttc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nfnztcqg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cwsbtifo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ypzesopd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rrahqxnc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ciulqbll.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2olpnfqod.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkturwgk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2avemmlnh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oicdaijz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2puxdlohx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2txxacyue.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlinommm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lyvfolii.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmqahopd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nwreocci.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tgtwsboq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tnxwrybp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kleepkau.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rgsggzrg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2urtzerhx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gcpoqrqt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2sssxzbmw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hcpmvibm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmizacng.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhzlodk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bwdnwzml.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fdxqgqvc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2phkhlnkc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ayoohrwd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zewegkrs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ohejanoe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vjzxrtgd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bsfaqghn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vakjqbhj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2prndxzcd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pnjiwafc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2oapknuil.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfryjtd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2numwndez.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2whmorpks.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vvztqpti.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kccuerdi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxedgze.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smpsopat.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzsrwqdl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhditjd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njelkthv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rfooekhw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2qqcnlasx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yjpquzxr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2knzdiqku.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2gyylypoq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gkptrvza.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uayvtoke.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwwdbbsj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yawpgyul.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rpksogqa.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2pbskofkm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rxjesuko.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tkvvaczv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dgkatauj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fetejifx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cirpvegj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vbwlpvce.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2klaxybhj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2dgcxndfc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tpreqnzo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oqveikou.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aqgdiiba.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cesowxpf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvxftdz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zzjlcqse.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fvqqqhsk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2thakccmb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2pqldwkno.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2azpvrpji.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2sbfvzixs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2gmaycguh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hcujyvwj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgsasqtq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nfoiwwtj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mkddkufv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lgswyorl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwkzcp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bdnblsev.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2noclsmpw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wqfmoine.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ztvqqcbh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cdxkmbqn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eioqiozf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2owaqpahc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2iuehlxwp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pwacrdwo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zuisgkap.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nizlujsy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bfqexuwj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mluwqejc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oedspylp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lasuunuf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mtgjihzm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vegiunyr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ofwswtst.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tbkbwyxr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hastzmpw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2adbydjzh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zlswvfhc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cyxfdevx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tghskobr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2genhgimn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdbyflpl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tncyydpe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mknorwys.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zenzdlqx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2vyltgozn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqlvofnt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qufdlvxh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rnllnzhg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2crnefbst.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2szogewop.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uilkjfzy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cigrqkyo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bzslsees.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2mygwpsam.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wplvjcen.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zszphaja.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qovrglrg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2npfzyygz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rhujgqmv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vhwflwms.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pllqinjn.html


<!-- 参考信息 -->