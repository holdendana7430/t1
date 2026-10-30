代发 wailian999

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gdzmsvaxm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkvalvzyz.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gndgwekvu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gyjmrfwyn.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gmabsfpol.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gliizisfg.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gqhwjxqlq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gsphqmvww.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gsxsqmplq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/grutmdsie.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gdyxjdknm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gucfawoya.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/grgaybzlv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/ggpcoanze.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/guubstkmn.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcyzizvty.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gfmdrcixn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbqasllgj.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gmkjyhjqe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gewktbciu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gokvpysrb.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsfyyflsx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/garlkosup.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbdddsbeu.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gsoqypjpp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gopejcgwc.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gswmbnzbv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gcamptepb.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gclgoujox.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/galugkype.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gldhfsavm.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gerqfmmzd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfeelceb.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gzmwszwil.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwgfwgvbt.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gdxgshyhf.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gxlgudtix.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gtbofftoy.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gdooiiawy.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gbnymuzvs.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/guoisrmxi.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gkzkpmneh.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gepjjrvos.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ggsmooyeg.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gsjyjjsyq.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/glowixjcs.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gfvlqpnud.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gxrsdosof.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gubijyope.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gmfietqsr.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gtiaiqwwp.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/ggnpilupg.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gcastaxcn.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gftpmrgbw.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gykbnoseo.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gsnecjeag.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gdbwllhio.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmgcxowax.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/govyymjcv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/ghotleiou.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gtpzsyvxx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gxicetbpl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gbmndikry.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ghbgjpvqb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gosmpivsl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gdwbnqsho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdrejgtle.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/glncscdyf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gdtgzafma.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkswuipsj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gpnjmmvhv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjsvmkagi.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gfpuiorep.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gzpqsxaod.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/ghlftyctq.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/ggdihtqfj.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gqgrfkxed.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/grgxispeb.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gnyaikjar.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gnmikuybe.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/glvfxopck.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbpyrdzdt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/grkbgsiop.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gjrbadcny.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gvevbyccd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/ghdmxhsgt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gpjheocgz.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gyeicusjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gavnzhdmi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/ggasqvbsh.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gpxksbwsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcvcoxjlj.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gplpowzkk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gjdwvodwn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ghggutbbm.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/goiqvldqp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gbnjdcwmw.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gprqbajyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gqrjviodg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/ggdjsmpeq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gcfokuywn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gactkrgdb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gjczllqmu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gjchkzwhe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gzplalyvk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gluwygork.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gdsjsbitm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/geyxuljir.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/geubxjniq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gokxmawsn.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/ghgmtvdil.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gnxlukvgc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gxkfvmzto.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gayifhilv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gddlvwjmm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gmdoukawf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gzbhpxlva.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gchgdnddh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gseyncmmw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/geopetzei.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/ghuobxyml.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gicgxqzaw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/glugykpsb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gihpikley.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gjyeujgeb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gsvqdahzt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghsgtqwtt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/ghxnngfia.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/guaxxplfr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gfyihikgx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gdyhbzfiv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gfchoyylg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbhjjexju.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzqtumjss.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gstgkkuwy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gfrkfizuc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqaggvcvz.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gxvxctavd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gixxxmvbh.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gypnzigfx.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gxelawfhh.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gyjoinrkv.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gumhukyzj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gcrjmasgb.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gadhbsrlb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/ghnfaliqn.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gdayfkoxt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gsuhccodj.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gwhwqyiit.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gmbavlnay.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gikrloegy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gnzekwveq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzaodsbei.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gqeenmnhp.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gpjetpvjt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/grpolxkyq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/geqguposy.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gnxqtlglv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gxxmqimby.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guvvwbvve.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdhtwuagy.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/groscpcab.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gpbrcgbmh.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gjqigfuva.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gfleuijox.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvavxbnrj.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gyfdxjbkl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gvuoatcyb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gjtwjvopk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gigzbaqkc.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gjmyiypjv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gzrfhyoku.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gwflkyszn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gawqynfxh.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gzwzaptuh.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gvwjqiomx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gozadqpry.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gymvvqbit.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/glisenffq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gmpqobiha.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gdzrlmdba.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glikrljup.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxmkwnzgp.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gbywfnuvn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gezcwshkz.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gorzgtjwc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gcpojvvbb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gwnuctsls.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gebtnktym.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gqabhyglb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/ginlbjfoe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gaqtbjwev.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gembkwlke.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gbyloqltm.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gwxirfbxz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gseqwwkyb.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/glrevptdq.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gjbqvlsdm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/ghvlbnsid.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gtvsskojt.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gvivnmtok.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gqamcxxrz.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gddrohnmv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gntvmgdmo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/guotruhil.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gmsdpykpm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gvwfzohpv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gejwedcom.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/garrufxak.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gerrwypwk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gehlmipzg.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gykbzbriw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gnqpoopiu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gclswmvwk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gjmzzzpnl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghhtwwhgk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxmjojpuz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/guovowkqs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/ghtmbzwob.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/goyinwcko.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/goumjkqrw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gjeplbrlw.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gudjodjqh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gicxzypuy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/ghsudqrvd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggpmxmwqi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gerzfirhk.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gaultgvdd.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/grrhslqlq.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/giigujppj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gvjlimelw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gdayykcxj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/geqoeejfs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gndcnfzbe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/glthofozs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gsdtssmqd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/ghstgkeet.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/grtofmzet.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gknodaahx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gokezhxpu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/giwjumsoz.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/geohrpqpy.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/ggpkwgohp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gswbxtrdc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gtznxbyta.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/glapqdzxw.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gdqmiklvr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gmzfjxyre.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gpxyljeto.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gelwokpkw.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ggdbkuaek.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/glmpdvhxn.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghqwmwnve.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guzahkbht.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/glkwapcwn.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gitydrrlb.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gndmotznd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/grmzcawjw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gtodvmeml.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/ghmxtzwmz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gbskdpzgb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gbpsuzzgm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gfnmzwpnb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gwdhpusen.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/glvckshwe.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gfeahejzx.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gqduewvrw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gcavrkprh.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gcgfpqetm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gtwtmkqwt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gznkmikkz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/grbljfivt.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gavuonkwc.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gytjykozv.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/goinibowz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gybzamvtu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gfksatmfj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gugvaefbs.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/ggntnsumn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gdeeuxjby.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gaskesotr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gfgcdchpx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gdnxbqudk.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gmdpckzhl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gituakyhy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gfyisftez.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gfpmrhldr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gskdoiwcb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gmjfgmark.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gikbvivkt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/ghrlscvem.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gssclwpdo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gjkovfhwl.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gosjdwlbw.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gxhtbnnpv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gfyojybgx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gdpeengrs.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/glexzayya.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/gdaenfdoe.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gaoimacsx.sHtML


<!-- 参考信息 -->