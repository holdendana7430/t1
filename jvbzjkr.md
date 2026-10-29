代发 wailian999

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gpdvqybjk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gegegupul.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwqzsghbx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/garhmvztx.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gpmrqozav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gzlmdtpzt.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gubievqbf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gdsuqhqmo.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gjxjbggbm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gsoluqfly.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gmmrrtedo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gjxhtbest.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gxmmdgudg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gowdibgku.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gqrlccroz.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnxyjcvbt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gujvtnfyn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnxkrytxb.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gcqkrifxk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/grqsptkht.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gvesqwpmd.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gamdhqnyo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gumlvzqac.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gwejpqsmt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/ghvncttqc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/giydzwmuq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/glngushmx.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gxmilylwt.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gakoivuym.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gvfbavmqb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gqiwvlxsf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gaooewqoz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grqbyrcyw.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gimfjftsh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfjkannhe.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gacztjyee.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/ganlrpylf.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gvbtflzlm.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gmwletdvv.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gbvbjqswo.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gkfpimwle.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gnibizppi.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gkutoihrk.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/ggrmdlkdy.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gprriigbe.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gvfgwogxp.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gfoewcshl.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/glwdykofs.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/guqczavqd.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gqwwaytmq.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gzcnuprwk.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gyeymxllp.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gcowerkxr.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gkrocdefq.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gwtrdyuvu.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gahhxjacg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/glvxfxzht.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gxzwwzjgh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ggdcjkzhu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwqdzqtlg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gggofasev.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gzvqogozp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gdokmwhrd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gizcxivzf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbbezjbxi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/giasmqhas.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/goselgcbw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjtngeepo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdemcwnqn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gmwhmxesm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gtkkwobjg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/guhrbnjsj.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gnfhnbuey.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gltfablxj.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gjyzmertg.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/guomcxuak.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gynvmmthl.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdwltivnl.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gdbyaaubl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gebuxneks.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gfhxplrsn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gczkdaass.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/ggclokras.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gxjpwsiel.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gbixmgtgu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gxebnqhhk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/grftklowt.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gyksotfvt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giokelxww.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gcpawmeka.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gxmitkhyr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvzibuirr.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gzustajqo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gsbedonib.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gdtsmbajv.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/ghfvkoptz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gelbtlfaw.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gzcpdplyz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/ghkjcbiym.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gyjpftjbb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/grjuxgdbl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gecycsrvm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gejgjbedq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gvrelzykz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gsrenmnlo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/glhpcagdf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gulxqingh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gpqtqfhcg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gljhujkps.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gitfemuux.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gijthsues.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gegvnxbes.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghimfmtmv.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/ghgpbwnyx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gswteufxk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gmxtpgwfs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gegpiyzox.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gpthlkuvb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gmtiesufv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gvehlzmyz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ggvdilxyb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gadscauki.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gekdhjany.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gtdunafmz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gfkxhhqfb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyupcjind.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gzcngxisp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glfhaeadv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gikskupmm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gcllubcbh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gqpaloirf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gdclwjhet.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gphkoecfg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gfgukinsi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/glijknuye.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/glupjnuli.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghkfmdfpr.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gaxwglzsg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmpntyyvo.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gdvumpadj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gfuftoldq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gfkorabpn.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/goxfncxio.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gbnrqfvqi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gghvjgzwc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gikbflnlq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gvrggreet.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gtlxhlhfz.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gzluacwaz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/girymorfg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gbelzfyqo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/ggacuomrh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gucrccuue.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/giqykhuun.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gyzosddxi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/geoyacrqj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gtleauiso.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/ghvkvnkmq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gwhgqjsad.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gdaogmjhd.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gaaiaqssr.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/giqoqvnbr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuxvfss.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gxqanxsis.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gsdtrteig.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkfcwafvp.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gsxavqxkh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/grjrmqebi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gslzajjbt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gojkprnyf.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gezbiluxg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gjpxtdfwp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gzevezmzl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gfvxtecal.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gnljgiifg.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gdyxjudpa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/geiyapaye.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gzbvebhry.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzioxlcgl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gvfhmyygq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdluzgtbu.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gwnvoshko.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gryjrypri.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqxloevqg.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/glicwxuzr.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/godvhdimz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gtzuhpqnu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gnlagtfts.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gttqnadfi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/ggftxgvki.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gjuopswlr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/grblwwojx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/giwibqoid.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gxqinujqu.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gpdfllaah.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gprcayclg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gnsnqrken.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/graqihwfu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gpniksvhm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gateuemkq.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gankxgcuq.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/ghmtqhzvu.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gveabjdux.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gepnglvqb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gtcqkoysi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gekcwvppp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gtaepiwcw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gjynmmmpw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gnuzqrsmf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gvqcqfurk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gqowvsswc.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gelzyexxo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gboqmivoa.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/glahfbeze.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gkcearaux.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gvtwhdliu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glprgtzdp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gubvjvkdv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gltglfdkd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gewtglfki.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gjvyozorn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gaayzqewh.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gkjgemmcc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gopglccyt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gmkhozokm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gpgcfbyuc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gcohwfnxy.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gqkzpsznm.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gutvhurti.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gcqibhaus.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gbgtcicbz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gadpkqefl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gcxchpbku.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gnrijypzv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gbimyrsna.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gmtcorlyx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gqdavkift.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/guocssgrq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjyiykmkk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gjvnphuge.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gxnbbuhdy.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/ggifbsueh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gwaqmyjox.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gneheivfm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gkfsxgjwc.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gwkrlqmob.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gvnpfqbxz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gbnowihlv.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/golmlpizc.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/glfgdapwu.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gjqcnoerj.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gqgmiihxe.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gcrckrieo.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gtuzplnfk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjvtsxhmz.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gvqdgwyiy.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gaeghnrqi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gxdqrgjtc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gihhyfxqk.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gnouqpvqr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gheouyvva.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/giovahmct.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gscoiaqub.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gtzumfzbi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gdafyqgmc.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gyskzmzhe.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gcrgvfnlq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/glrzabzxn.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gggaodebl.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gywihgtcr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gpgcotnqj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gmtbqlwyi.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gaynmnvos.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gvwsauvve.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gyhqjailu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gybssziqk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gzvrfslqg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gaqyumorw.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gnfsniejl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/glwxdrkdz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gfrevpdkr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gklzciykc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gongqrdhf.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gktvjpsiv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ggpryieez.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/gcmmwivfi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvvcfrxhn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gjlqbgfcs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gyhohessa.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/giyfcstie.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzfawwkol.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gstsdifsp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gvibatjen.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gnvxktzon.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gyripbxfe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gzqnjjscm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gpbjikofi.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gbgqcauzn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/gynphtdaq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/geuwomjlc.sHtML


<!-- 参考信息 -->