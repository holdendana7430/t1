代发 wailian999

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/grirlgpad.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gtuijngdl.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnwradwpd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gyfltjkyg.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gcsxgqaxq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ghtlkxhzq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/ggkcmsrvo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/guvsmnowa.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/ggwwuihbg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwewhbxp.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gbaebrlkp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gsrblpzrp.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/ghzxtvpxq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gcnqwifnd.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gipktszjx.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvutgdivx.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/guapfbknv.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnialacfe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ginpffctp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gkhcwryyd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmcogmzec.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gopabcnpq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gagvoyrcl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gqhddtanz.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gkcqblyth.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gvqixszvd.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gugwwauxn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gowpjgauc.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/goskslary.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gfmxuwhrc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gzpjdteoz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gumvcwftr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghreextkf.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gyirfrevw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geanugcqm.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gozwdvydt.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/geklzubbi.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gluvqqwrd.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/giajldklr.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gdovuqvcy.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/guigjgqye.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gigunzdga.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gaiwzuftc.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/guinquvjj.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gmfauoydo.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gksbjqhkt.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gdkqpkfbz.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gsohylpwo.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/guhwvqzxz.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gzzktkbfz.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gwpfyiqsa.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/guoypvtrn.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gqngsvwyk.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gozzjwfqe.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gjtbvokdp.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gmqneyfqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gazuqjviw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grtehfocb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gojquuyel.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gzgzgcaca.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gjnhmfkcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gduxrnjfr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxhdqdrcu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gstbhjmra.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/goddapjar.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gwgbqpfez.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfuclptjb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/geaqdsxzz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gkslrjlpp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gfxlqdpgg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gkadzmvnb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ghorlmeqg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gtdqbjbtt.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gmwclcprt.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gbexhqiqu.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gcullghqg.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gmyyhtjmf.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gknbcqjis.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gnniydpzh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqdpmmvad.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gltidntyn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfqrzbcka.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gdfynwcch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gyigaqofl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gqekxqbgh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gczbukfse.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gdwtbizmt.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gsjhrlmrx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gshxmrfwe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/ghznainvy.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gfcmlfmem.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gynhkmppp.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gygxubrua.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gvcnjbxyt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gkwoqffad.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gyvvcrnkm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/guhtqstay.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gyofhaskw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gevfceopr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gsngsngpl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gshfeethn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/geqtxpnme.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gzfnaephk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gxthkicgy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gewayfhfw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/guratgwkp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/guyryngkk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gnnerafhf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gsemcwesa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gqraawutt.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gqcwvemos.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gbjbyoghy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gogkauqiy.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gfqmfokec.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gemtvnjug.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gktvppflw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gzarqnjtu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdkndzuo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gfbzwftud.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gppjfdaal.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/guwvwuhjy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gcvjuokkd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmiscqrzb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/goykkpucz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gysxkxxla.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/goncxeayw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gcphblwwv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gycszfvtc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/geiiqbkeg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gcngkhbng.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggsaershj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gslkslkkg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gnysbvpoz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gybufzymt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gdzozxzhg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbwryxwwi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gekzxiuco.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gdluaoanu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gelqxbcts.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxsguxpjg.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gxtayrqlz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gwzvtqpaw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gvintjqth.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gkwyempsv.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gvovmbbps.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gpysyjavn.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gqbqwcycj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gblpbnmzx.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/grkxrwaet.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/guunzbfxz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gsasvjqnb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/goyvfdotm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gniyqqypz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gueaqorji.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gnfuuxgox.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gasfkdiyi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkalqprgv.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gyvqbgwrs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gpzrzxdxr.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzienzrvu.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvehxycbr.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggnvgmaek.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grdxzubqc.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gjfblwhow.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gxpmvrbnb.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxiffadha.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gpoptujeg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/guxfismub.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gxsmjjavs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gytxoknrs.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gcmbfequy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gbxhyazdd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gsydnewmg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gnqmpkqkd.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gtfnlyojc.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gfsgmufts.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gjiplvdmn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gztnbzgxv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gzjvufotp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gonpgfpfb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gujbjwppn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/geommtqvo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gebomfbct.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gekiwaprv.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gtavlurvy.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/guboebezf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gfwzibpte.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gislzuand.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gkkyriyol.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqxmyvgk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/grbckazkg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gzzabgdts.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/grdygnodf.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gvgwixkni.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gzwhthvfl.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/ghldzmwxp.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gnwrzuucc.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gbnzxczsj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gkcwsarmy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gaopnwzbt.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gfwqhpugf.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/geouyofsa.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gewwamest.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/giuatkgvp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/ggplnizyy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gjqvwvlgw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/glyqeltpy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/grsoqnokj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gbbdsgewo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/goxmvtaus.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/goxljsqgz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdklburbu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glhsuwegt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbeymfrrm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvbfzjkrm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnjynhnuk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyazozavn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gjgbuhiis.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gwpbavgfp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gunllexcn.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gbldgsgrn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gkinlaqmy.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gqsopirdf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gqwyclbah.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gxcljgdaz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gbbmweewq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gjncmnryu.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gideltdvl.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/grmmhqbra.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gudzdzjrp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gdfhxjauj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gyjrjkpjk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsckgxmsm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gztaghsyd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ggcvuiwot.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gvttweqfb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gbvnyundq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gkvtbtaoh.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/glahkoyfw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gokbqkszt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gqgrixxjt.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gapkfxxbi.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gscciilve.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gaiiqbhtl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gkzbectcy.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/ggsuoherr.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gwhweiyql.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gemmwlftt.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdolfzluf.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbedcpjfc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghpqjlclh.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/grbbbamag.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ghxxlsmlq.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/getqovqgi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gekdjafbf.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gkdiqmjkt.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gzluwsakk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gnbyxbzsb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/getefdvwu.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gykfpocbz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gugaceckn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gjxdpxmhy.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gzadxalja.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/ghuqqxcvn.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gxpiwpjba.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/ggatznjjc.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/geodxltvq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gwjiyegfw.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gccptpeon.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gxacbuufh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gyoxkijfa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gznmrgery.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gdmjxdrvm.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ghjsiydpy.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gpdfyqwxz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/glbjzvpzc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gdgrpicdc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gakihtzkf.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gxzhsebjw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gaxbupczt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gpwqqavpv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gogauhccu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcumvctsm.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gezabxkwf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/ggvdmxamg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gencxpehr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvaihtysb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gammyacuj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfjadytva.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gikpednwg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gypexyepc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/garoirxue.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gzvecgwfp.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gfaeivqil.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gywugzbwk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/ghvupzlrz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gqwzwdxaw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gxvqyetny.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/ghklmtmyz.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gjdtmfjbm.sHtML


<!-- 参考信息 -->