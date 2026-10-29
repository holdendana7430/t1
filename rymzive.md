代发 wailian999

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gyqjkikcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gwxtsyvwz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gfphdokzt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/guysrrvfb.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfxfwotsd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gevsujrmx.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/guwmanxcb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gxatwblhq.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/ghopyvtbm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gyshmeqmg.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gspevhjql.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gupmyfcde.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gwzzxavfk.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gzepowtbd.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gcwcectiu.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxlwogaps.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/goaukqkvs.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmtlgkmer.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gisfiawvy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gfjntalit.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gvtvwbzdc.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqjutaqwz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gczguftdd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gyyxybdcr.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gslbhlkao.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/ggdlztalc.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gixuutjrd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gcidmwzfu.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/glnoinsgm.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/giebjumuu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gpsxqhqaf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/ggmtqldly.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqohbusbp.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/ghoeswtwk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grjbjvrkw.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gicvbkrit.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gddogfqfv.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/ggmfyjexl.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzgqgqrhd.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gnqmzdbsy.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/ggmkuatni.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gaetwvgpl.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gdwiosydk.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdoxhubdx.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gpqkppauq.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gxgppvfan.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gqnexengm.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gwluqrrbq.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gycddemly.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gmbefibbt.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gqvuupely.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gnqchshgq.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gosyvvjvj.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/glyqbuonn.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gtqzethuu.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gimjdefia.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gtrazjzsh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzivixs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/goxocxvey.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/glklvabyl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gipczuydv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/ghhjhytwz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gsqwrqtbn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gppkotceo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtczibcgy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gfuqkotfp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjtnaxpvh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gaumfmxcg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmzdcqnsc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gldczvwib.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gmywsjlzn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gtfzyjfpq.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gmlkbowff.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gwhjlphfx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gkawptarv.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gsnsqvcio.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gsdaadact.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/giagphckr.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/ggurbusao.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxzrqchjv.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gbaxoxdob.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmyofcgew.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gwramfxoq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gfzbxhiij.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gujbhkiyy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/grceqvwhb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gvrrbsvmo.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gutyxstfh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnjrbiucu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/ggzjttzwd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gpyytbola.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glpjkbujw.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gzjsdobaa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/glrmqpgth.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gjiwfmvke.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gixkxsjyi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/glrmuwgon.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/ggulnyfyv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/grifkpcdo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/goyprnxxo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gvymwkqut.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/genhoulko.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gweiocelk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/giziccquv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/giognbbdz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gwnpdqxim.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/glekcetiw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gpeipcdda.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gmkyzvmxv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gimuyscbl.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gfjctaiwx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gyirsrekf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggegzbstj.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gwrszmvxy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmrbirybg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gttwgaidm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/ggkrvghbj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjhqyby.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghsyoffzb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gazfajzrs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/guslrwzxh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggooeptuj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gvbdpwhgg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyqxchwxq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbqayyygy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gcqcavpix.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdajawsrq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdipztuk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gamveaocl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gzstymuul.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gwnbpaabu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gqepzkrkk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gmhdeuyau.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gagldtwtc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gaetvcuyy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gejdkarcd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdmwzxml.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gqtdyyzvb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcdrmtcir.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/geghqybby.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gbxhtzpjt.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/geeceoxcm.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/glhcixsuv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gkfvwwzjv.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gdsmuobtl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gnsycwttl.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gqahvtvxa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gdrvfsnmx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gzivrubhe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gvuvvskdi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gjkzummhk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjblwzwct.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gmjpfmcuh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gphtnlkoy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/ghlunfvmp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/giwlpadlm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/glllldvdb.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gxcumbfcw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gomgvesmb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcbpljejn.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdplwocye.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gsspzllgl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glfhsbrho.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gntmiagbs.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gdfsyvvfc.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggxukkeyt.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/guexulmyr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gdpsytnye.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gyodsveww.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gbrookqqv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gxneqoseb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gozakwgvr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gtmbgsyrg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gvdaqybbg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/ghrxzsrtx.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gjwyndmrv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gurzvtqyq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gpdokedlu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmiwepjmo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnhwmgsmx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gddjnaxxt.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gftvpiozc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjrkzohvq.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guntqaopi.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gcmenfhuv.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gynjqvqwa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gakqzkexo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gaukmjbyw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gwvcqgzfh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gglyvotkb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gogxamapd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gdosahzea.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gybllmmxx.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gepjuurnp.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gfsiqluhz.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gxbeltnlf.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/ggpbwgvfn.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gbezqljmw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gphrosaks.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gxplwrehd.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gygzeiqcb.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gkxtvultd.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/ggdsbgjtg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gwlxvokwl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gccyvlfla.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gskigowij.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gbnkfhwyi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gkytscasl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ghwwlzbvp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gjxobuiqz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggtjbimmy.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/guxlsdsib.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpjxstmkk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjqssumes.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gianjvgzo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/ggfgnbrck.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfmxiridq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gffoghhat.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gisutmbcx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/goawlfxjb.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gxdjinoea.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gntnuxjsv.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gpmlnsngb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/grsvjiirv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gxeprdsmz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gvjkphwnx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gdlspladb.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gfiuzkefm.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gjcuitxvo.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gxsybgzpt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gyljrbwpr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gfoghjtdq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gsqhiodjq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gnwxxhris.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gqeornbgj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gfehdzvjl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ggvlokdav.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gyiaykian.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/grtyjesmw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gochckzfl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/getzldxri.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gbksngizf.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gkernfpoc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gyoojfqlk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gguywgacv.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/ggoyvokia.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxsyddlhb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gfsrypchu.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/grzvhdbam.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcovuqnyc.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gifdvzfon.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gtbubnxyz.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gvxyeytin.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxvgnuuzq.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvrbeqrxe.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/godscsdfm.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gwgjnkiqr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gxhcntowt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/ghouelozl.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gujfwkukz.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gogoezcyx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gygycndgw.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ggylkptts.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/gehecrnen.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/geysfxezn.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/glavbmapx.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gxtctjgha.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gexsrjiue.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gknznrxxk.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/geporztqk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/ggtosscvo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/geomhdlvq.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gxbcoatrp.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gspocmwhp.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/grjldhuaf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/guslzdqjq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gakgnpltt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gcbfxctwk.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gjzvmbmuw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gosxfrqwq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzijmtxvb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gcxxmbnjs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/grdmludxz.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gjpasoslt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gaaxagocw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gwhbeveew.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbomnwozz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gxfbdwesl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gyisncrdk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gsicrleuo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gqbjdnspe.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gqeiiuooo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gxopxdhmk.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/givcctofe.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gynalvwxt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfxpnakl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gkvlsffwb.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gjjwxdpwf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gysyjnnne.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gbbhkfamm.sHtML


<!-- 参考信息 -->