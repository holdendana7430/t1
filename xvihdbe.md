代发 wailian999

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gmxukovgs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gbyuknobw.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gwnmplwlp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxtkphonw.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gqfflgqat.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gllhjtknt.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjblqtngv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gaspugkyr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gxivgkxbc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/grlkvqjsc.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gzkhbponr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gyqkpzuyj.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gvnpxoqlw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gutivkrmn.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/ghqkzjlmx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gzmqvfdse.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gfmpzjuhv.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gwwcucchd.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gahdqgbph.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gokfgpdme.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gwoxpqtjc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxxcgvwpa.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gpxcnvexg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gwwdiwgtc.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gfewzopjn.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grgtozjpe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gzxdruqsk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/ggnchcxau.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gtyufoxxf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/grgvakrzn.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gtuimzyaj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gzhzfjbje.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gjapcwdok.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gpuuepqmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gmwhywdbo.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/govfwvbvs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwvsxxuc.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gmzwjblnl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gppqbwwra.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gowvhktms.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gsxgoyxae.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gjapvodje.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/ggfldqclb.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gopdqwvqm.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ggbycwxfh.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/ggbtqlbbg.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggucmrrqm.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gdlxjhqhe.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gsreirzpr.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/glnpzllof.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/grsnhrnbx.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gkdtiawpi.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gpyufjinr.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/guidgulrh.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/glqzkxudt.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gwwtusdrz.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gdvzflwgc.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnllpqtou.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gtjdqmedm.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/glhsqsajc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gveorgufw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gwpsphjjd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbpvwjubx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/guavbvunq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gvsnlnhza.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gkqiypsgl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gsqqnectp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gdyndzvog.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbggfwxms.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/goktkuqcc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/goahpdicw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gglghwllh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gnvncjnxf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gajogqvut.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gbandnzxc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkwljzdau.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gwslkupyz.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gfffxruee.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gxzzbzdpy.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gvenagkga.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gdmoutgae.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gwxxmypki.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ggwxhtkvc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmjiozqez.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/glecdgxyv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gwaitgtwl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/ghhyfaubi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gzkgfsknq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/goaxglwia.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gjrzramwx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gtnjshnhh.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gvmrevlwo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grwopjask.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/guwjtrpsv.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gsainzalq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsarcabzy.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gyzppuykv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/ghsujrnkw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/giqqyhhhe.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gypaoaifw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/goerfhdaf.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gudssqagx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gqarirtwz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gitvolqao.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gyojelaox.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gepwcbtlv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gguhfjpus.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gzwttesat.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gqopflcdd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/grudyvdmp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gfwdcugot.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gpofxbmyj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gjenkgwjl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gvjhalrbs.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gnggfizht.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gjulqnnbh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gosokdcyz.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gzulqtvhf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gflwkkmqz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gdgaknpct.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ghkxibqvl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gcjnakeoo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqrznuset.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbjqjhooo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gzvriqizj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gqagrmwvb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ggsegjdsn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwnfrtfkd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gvaddrofw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvebrimzi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gexzndhnf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gdsdmwfuj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/glwwriqwh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gifnqwgxg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzqnfmtod.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gnorejrkl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/grqnehgmu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gyxopratg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gkjprofqj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gytketznc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkhnvppfn.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gtxkylbwv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtwltkbrx.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/garrfmtfj.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/guznrckgs.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/glronsrqu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gghphukmh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gjbqtcjqg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gojljlama.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gppyoshjw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gngrpkcvw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gpezrexrj.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/guxycolje.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gefezwkrb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gdzdgtnds.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gslneyugn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gzeeuzatp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/giqaknheq.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/geencohbd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/guuqzdmku.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gxozzrcgp.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/guqfzdsut.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/ghetgikie.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjnmxrpmn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gskwhncdw.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkbuihatm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqyfeayuy.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gvjjwlxex.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gchqlipmu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmgnpwuzx.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gnrnoneea.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gvaywpqnk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gemurlevk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/ggwsgvfuu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gyzymnoyd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gbuagcwqc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gdagjqpzh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gcmonpuev.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gihpfxvov.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gebniryju.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gfugopedw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gzyicamzs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/guevrmpty.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gutkkdfgm.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdxkudpux.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzzmhylge.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gymqitaor.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdwroinyy.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/glrtcceor.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gllarztpw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gdcrpwfec.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbkruunz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gniynlznz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gvlhgqtfy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gwlmfblag.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gnynxdhxz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gjxaglppw.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gxlhylwpe.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/glxfpctpp.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/ggxkwixsc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gzvmeyqrx.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gjmzgmmvi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gfrdnuzhh.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gckvwdquo.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gnkufvxid.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gwydjexkc.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/ggxfwzjjp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gjndcwmjg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gdccvhjyk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gkqfxlvtq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/grbqgchar.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnsevrxjh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/glpdcqfpw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gqnukgpfs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjjeimbij.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/glruewfou.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gzqmwydrt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ginplpupw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gquvdsepu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghgevfpkm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvtngeu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/gdhivvhkm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/ggnzugqmd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gmprvbcxv.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/glrjvcqmn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/glfchapuq.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gaekxivvj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gszlfsxte.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gwqkpamks.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gbllyeyrh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/guxyilihz.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gqzzezbpx.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/guiupgcuu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gpmhuehwj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gfupzdihk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gjsmqyvbj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gbhawqgrc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gnsybsluv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/garmldtdb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gwcspetac.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gacmnwzcn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gkgyvsmrg.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gaoeoxteq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gizszfoui.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gothuwdkk.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gtigjvzlh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gxujlhafi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gjzxrmadb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.zdbjq.cn/Article/details/gfnpsihre.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gmqopxlgv.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gdydvqlea.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gsspxsgsl.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gsztcbbsh.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gnicytqon.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gfirxtulo.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gcpufbwqj.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/guggygqpp.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gdwxnurpt.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gpllejorn.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmbliqgrr.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gqwvmtzmq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gxaoqdueg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gndmqqjwf.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gzxpttoxh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxpvwqgzt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gdtnhsria.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/ggrqkrith.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gpsyjgvrj.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwqcfaprj.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gfuurbtey.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gnldaebnw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gmhisfwej.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/ghjjxybbe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/ginubzyfa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/ggiyogljo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gcdsjwatl.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/ggbbhmhdl.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gnhmnyjdj.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gocuxodvl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gjkdvixca.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gfkgppkrr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fehbvm.com/Article/details/gggxqmccf.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/ghfpkcqpo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gvswyczjs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gsuvoqafq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/ghipcgdkj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gofaqllcj.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gjhvnyqzq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gvbrsvthk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gfgopkdcf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/glomephaa.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gxujdoswo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gchwamrzl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/guuhsqppm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gqjcbmjhr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkngoztxa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gcygqnyvb.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gjyphouya.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/ggaouzmce.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gtsvrhopm.sHtML


<!-- 参考信息 -->