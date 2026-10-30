代发 wailian999

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gjlxxupgr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/glxdcmdiv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/geokfitjt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/ghesizuro.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/guicjsmny.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/ghaifyrpo.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gflfhrfhq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gnijkqipp.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gdnudrbqx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gcobonkev.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gznqwnagm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gqrgdhxns.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gygdqwiwz.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gefmqpafq.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/givuwlkvz.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/goiswjodg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gddhskkjd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gznwewtyg.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gzozhfnlp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvcqstdoa.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gyisdtqbe.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gzjygrbjw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gjnrwhapc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjgxfvxui.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gbnpwmwrq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gzthptgva.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gnexdqwvn.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gabfaycvo.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gkqcavcil.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gslevkbis.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gbafvxfks.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gkdqecvff.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbgkzrium.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/geosnnced.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwuoxuqqm.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gxumfchpv.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gkqpuouln.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gqdwxquyd.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gjeumdjqn.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gnzyagbos.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gfpsnsuzz.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gparnigds.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gyxiqzlhx.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/ghrmvkggd.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gyqmfhkgo.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gpvtblrbd.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gbribbria.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/ghdnwwyts.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gcotxlzih.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gqynsztgg.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gmsgdovna.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/goskuhnbc.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gpfaehyid.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzcgpdsok.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gvhxoivai.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gjmzwufom.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gufwwawpz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmkuwfzpc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gogpcmvhv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gcuzocofd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gzpofooqm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ggvxnsnbm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gawfsbpad.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/grdgaukme.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkorzosbm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gskbjauvm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/glxcbtjhq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmrthfzou.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gwapzxwhd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gwvstdrhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gdxmfslbt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gwqrtyucu.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gftcnlwdf.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gvaqfwats.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gxihkybkz.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gvabrroek.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gpxmvuoax.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtunyconk.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gdripgbmj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpvekbfgq.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gqvmgixgk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grlwpythm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/grwybaflw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gupcdjppa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gqomtikje.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gsnbtfmxz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/ghlxpveji.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/grzfsalxi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcsinfhoi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gmdtlqpex.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gbuxhmgtg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdezhwdpk.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gubanfxnk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/grcmswxdp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gwdnnifvc.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gobuqfduv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gzqbkxsqt.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gwuzvmrik.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gdxnfnrzk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/ghpprvokq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gfqgecsjg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gocddcxil.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gyisbceof.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/ggyppvtbm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gwykeybsz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gfkddezto.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/ghdhjevmh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/ghhxvypqp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gysqvaamm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gtmyssorq.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gcnmpkkhx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gvzgavlol.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkdtynajr.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gcyyiwxgo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goxexcfyu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gjwjxdwso.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gpwweqxsq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gcracqwls.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gbxedyyqa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gextnwlfw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gaforweqo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/glbgoysvx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/glewhdkwj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsbqealks.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ghrrjirpw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/genrqgvkn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gzqiuwrem.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwxlnsbam.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gpzqyiiqo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggcekwlyx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gxdirbirq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/glzrubbvv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/galizapdz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gvvnmzqiz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gjlxxewjr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gtbxucpvo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gifcqlnuq.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gnejzyenp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavniyyln.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gaxddrcbv.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gwmnfhzye.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gmqityajl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gaawrntkg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gdoblzybs.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gkruxxuin.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/goczlbmdw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gntgtlbnp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gcydzgnqo.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/guktmnfst.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gjadexcjn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ggoutbpta.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbtsejqqs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gaglgblja.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/grqgmihcc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gedzpecww.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gfvemhhqy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/ghplzzkad.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/grifanuws.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gpmkncmvj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/guaitcymw.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwjzhcmiv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpemvsipo.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkbkumuar.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gqhrnvqad.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gczovwbox.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glqemgwqm.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gslskvvwh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gtxlfmizl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gsbuaqayl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/grldtvoqe.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gdopwdazg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gxnivaqmr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gzniqjugz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gvblfcrwn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/grmjisard.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/galfoxnho.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gyhjgczxb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzjodaoow.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glorjsnro.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvzrokcve.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gqahexsgc.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcjquccoj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwdqqihfr.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/glhdafbkj.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/ghmaytbhk.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gzffghrug.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gtxqbfpvw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gnawjjrbn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gnumgsqcw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gnrxmjbyx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gksjuxvnl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gqaheqrfg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/geddzpqfo.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjfvnaguz.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/gepmqezzl.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/ggdzbsbbo.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gvinuuhil.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gaawnjeek.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/ggejzvwye.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gixlnybmx.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gsifnrfzp.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gddcgwafr.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gdbdofyff.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gthasjmuz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gwtdkumag.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gdmlcjnur.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gmuzyjeeu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gygmcnxxz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gyetjnjfb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gizadqvag.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gmfwlgwzd.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gcslyowza.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gehhiiscn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grbkcwryh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzgusfgtj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfpzmevub.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gtzggtsyg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/gqdtylzdv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gxrtwtvkf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqkwtqapf.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gizvsybop.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gcdhpqhjc.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gwxkrfrvs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/ggdekeqqb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gfultkuqn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/giidohqtg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gevqdtqcl.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gfkqtulfz.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gszfynfuh.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gtopdtuqk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gmmjbicvf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gvhcxamli.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxuxfmvdi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gswolmemh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gibuavbzx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/godxvzpoo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/guesaxtpi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gwoyjajwq.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gckqaqfhk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/geluwmnkz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gwhejwrrb.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gczhzxtax.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gtjafzlpc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/ggpvwsios.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/guypyzwyq.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gbmhofkfq.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/geggmjyud.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gfgjotqsd.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gjrkaylfl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/galsackuq.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gfknpidkx.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gsyjzlpvl.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gndqgiips.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ghffkminx.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gzeagbnej.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdpqvocux.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gsvpwoukm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gtmlkarhw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtdzzmglg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gxbkushgq.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gkglwygfc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gclpuqsrx.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gzfjarhlr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gxwlvkkoc.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gbxmwwfku.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/ggcknicaf.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gwxyixdrw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gemxdauyr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gindmitjq.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gzmfxhdqx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gckbpwgqm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/gitoxahaa.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gtspwgqnd.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gteyxrawc.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gzvsdpbjx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gpmwhpjrj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gpuvxpznf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gcuafhjwr.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmjqvwnzv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gbxtcwtna.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/goscjeqgz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gnpjxihom.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gkgdejgpu.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gkwdyvdbh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gusjsfugj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gnqknwfba.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/grqxeiaup.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gqxahuger.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gfokjprdz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gvmfajxzu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gewqifuup.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnzudndko.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gbhiexkph.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gvoczusfm.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gkbeqsuhx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gkzhjjsuo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gbrzvvwwb.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gbzjbilur.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gkmejoblm.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/glwutmxhg.sHtML


<!-- 参考信息 -->