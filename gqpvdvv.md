代发 wailian999

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gdcsniqvu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/govkzgodd.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gbcvdrkae.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gyniqlohh.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gjlhcpedu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/giqntnqxi.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtzeocsyj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gajetldet.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gxeiebgvv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gcasvtuqv.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gjqemirsf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gtsswesfp.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/grawgxerp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/ginuulzwa.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gpjjsrwuc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfeknpped.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gnkbiyavj.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gmapfkrvj.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gjyxvtgxe.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gjmtzkhhj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gfewrtfdt.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcfeqbodl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gshwyatbk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gdwgxkell.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gphyfinhk.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/glyyceagl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/grjgwatls.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxlriaxuz.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gekdedgyt.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/grraokjzy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gonrsvjhi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gbijmacxt.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gpaaksoub.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gztfhixci.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gynsjputw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gilejflli.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gweogomyp.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/grqaqgtfe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjteonzzh.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gmayevptm.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/guxyggyyn.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gozqdmxvo.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gvtfefjxr.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gjvkhjoqx.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gkboshrtp.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gofhhjkzv.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gwmrjoeye.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gedwzwayv.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gxlfmcofn.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gwqjjizsg.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gzgwrosux.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gmbxyljvm.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gpchcbwxl.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gmljinjso.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/grrfjmhvd.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gjxrpdpqt.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gsvhpbbbi.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gawydrivy.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/glztuyzgu.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gjsdxnjms.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gytocblzt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/guppbuzhp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/grgsebjkn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/glesinwyh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gqdlprvmd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gbiyevpwp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxkcidzup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gcvooteqt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqjnkesti.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gfipfrmrt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gnnabwfko.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/grwljsdfi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/guajeraqm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzscrmqfx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gskkltojb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtxablctq.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gxbazhxvk.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gwldalzit.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhqekms.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gelhqvhxa.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gepsrtjmb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/giuadqsan.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gkallifdf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gbxejemjf.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gdqqkaaor.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/goqrbbeht.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gimyhkbms.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gfoxbmxvi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gfhnntapm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gsbnzihdd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gvrmoozoi.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gwlyoqqof.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtshflde.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gclccuann.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/ggpjdzpgv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsmdezpii.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gdtmibgsn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gyredhywv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/goukalpgu.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gzdphylyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gjdmkgcgb.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gzubfdbwi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/ghunpzptm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gqmjwranw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gxeodplmf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/grorukcax.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gubmrdlau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gfhrpicgw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gdqktlvze.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/ggcmhpxdo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/givnvxfxh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gmrqhzinm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gnjjttuas.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gbfyohjjm.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/geesuecnj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gxvnopems.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gfnjvokkr.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gnmhvikro.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gqyzhnizi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gckqgjywm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gdvduxutm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gtavjvcsk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gbddivphu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/ggcjnkaac.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdmshurrg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxzhaeyuv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/goxjldksx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjkmjfgmb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggxyhutmw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gfnwgwnes.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gnbknkvqz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gymwivldd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gaafgzgwv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gtwsuufib.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gbrnjoalz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gymixowyz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpofvioei.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gphqmoeey.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gltmyhtba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gqxgookxg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxfwlpnxy.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gcseqgjng.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkeetfdsv.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gpchvpyna.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/ggmlpvpsc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gefwthsts.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gpchnxxir.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gwofkygph.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gmxdagxhl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gylwbvyzo.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gqfesjtgs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/goqcifwyt.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gxmopvusu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gkvomrfit.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gfrnrgkjj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbwwojlmd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gkilktmad.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gwomnbbuc.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gmlycondl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gdiljktsa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtcvitusy.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gonfueiiu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gzzoxfarf.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjcqekmxa.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkmndin.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtpyefbtv.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdmmxijak.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gddwdgglb.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gywptyfjy.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gpchwbcjw.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gyvcazxwl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gidemixds.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gbszdzhve.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/ghlecnuvf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gispkwgbh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/ghdkmkase.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/ggqglwvrp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gxyxevjze.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gsmatctlz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/glevucrhh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gbivgizyo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gbocnxnri.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gftvunuik.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gibxvtosy.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjrgmtaav.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzjpmnbzg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gtdximqws.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnjnmxino.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjxmgpjtm.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfqzaywju.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gjxjgzmdq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/grwipteyl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gxsfksiuq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gznakkgnf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/goohmtmbc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gisvwykee.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/guydmhsam.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gonjgubjr.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gfjfbldic.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gmxdwejdf.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/ggcabiqvm.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/ggxxljmvy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gyavmnlsg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gnaoymyho.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gdqzshodi.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gcexunvfn.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gjluyyywj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gvsdohgsf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gbqftaihw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gitbbsihl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gnntuytal.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gioqxmpci.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gyjekwbss.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gmrpfpfpr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gzoqcovkp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gmpdkpfcy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwyuscnnb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gorebuiyc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyhmvufmz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/geyartvut.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gouwslbnr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gqdbrwxqi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gxyhqgodz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gzopgfdpi.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gbfvnpnqe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/gpjvkfkuv.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gmkwrnndm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gcngtxkcx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/grudzzxht.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gannrywqx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gomhftmew.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gpwdoucyh.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gqpvgpptm.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gkfnftxzy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/giyarxudo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gatulkitq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gcvjhpecw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gjxcoldoy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbgainfci.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/grbnpfpjh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gqywpwlhp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gzlbhnxbr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghvxoiqkw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gxkucxktw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gdtyxhzbx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/genmsqvbu.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gmlskjjck.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gyplcejzp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gonhjhyhz.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/grlydbqrb.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/glbkhbpqu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gywbikaie.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gcrlhaspz.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gipydyedt.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/grmnogfgu.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvtbvabxh.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gknfcfnqk.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gyzdxshyr.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gxyhhjjsp.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gqtiezkho.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gxcvrrluk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gxgfberrw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gsttidifd.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gfajqwcvz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/grtcjbdqo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gpojjuowh.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/ggdtytysr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gdlcepiot.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/glbycloai.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gmfchdkzt.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvqoibo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/grauqakxd.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gidyvqxfi.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gagvwvotd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/grypszmqe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/ghjzwlbkj.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/grzcnovyp.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gxonzvnso.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gydgwvupj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gmiapbmpv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gstguwjns.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gsthsjjma.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gynhzqqbd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/ggojviyja.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gijjhjccc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gpfzohzey.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gqhvwzbil.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gslycjvxg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gwxloakdg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvtphkd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gmhyykdso.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gohkigdmx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gczjqknpj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjthqqfug.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gkjxmpeco.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gkycmnkrq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/grsttdqhn.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gnlhomfun.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gfatidodv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gwtkkkbjz.sHtML


<!-- 参考信息 -->