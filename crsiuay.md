代发 wailian999

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gijfradsj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gvhskroxq.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gdodiqtmd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gxhznbuou.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gtcpalkct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gmmgrrwie.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzpovibsj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gfymwvcen.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gibcftttx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gvvqzoyei.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gcxwrnkst.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/guowepxcl.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gfyunnpei.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/graqluctc.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gnkkghquv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gajzomxfb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gnvtzvusg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gnkljcfzm.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gnhxsjvqo.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gsiexbdno.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/ggthtgrpk.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtllebocq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gqupklnwq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gxaffewnc.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gfoklxduj.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsltchcqd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/glznywgoe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/giomhiizb.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gjmxyivzg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gboaqgqoc.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gxiwliffb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gngujwlcc.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gzaawzapm.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gggsilufl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gvwcfkpuc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gsxsllslg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpxuloixs.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gvgghosfi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giiulutfh.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gqgvebrdh.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gugwzgdxj.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gpdckpnjv.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gfhmpbjbs.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gvyxgzdws.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/glipgaqhc.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gsogashln.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gogqytfis.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gykyviggf.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gomhylaan.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gszhbvaru.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gyshipzis.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gkxxxzksh.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gwmhubvmv.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gkmqjqqbo.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gatbwkpwr.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gbhzvhwgd.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gigsrnfws.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gtgebghow.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxtohdo.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gudwdrorx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gpjezuqdb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gndgjbhhh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gofydzowy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gqdlpgquw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gnkmtrknc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gpqcfvybm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gjbygkdnw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gglvtotpx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxvqbtqau.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gemsrbfop.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqdcvekff.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjzckvkfx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggwqtahyn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gmwwebzaf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gfofihwva.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkijkrarv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gidbmjrum.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/galehtjfo.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gitcoejml.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gdfrkltcm.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/getdtelgq.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnxniyxox.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gjqocvxmo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gbqlqgoxf.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/guqyenkoo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gndmofagp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gqpjjfdaj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gxmngtxpz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gklkidsfc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gltoabato.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gsqwldqzw.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gzqaespvd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gairjivsa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gzeadlunl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gvyliyycp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gulcziefm.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gvbanerho.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gpjznidun.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gevaochzd.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gjztrwoid.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/ghcdeufgd.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gagtcecgh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gpnevcmrp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gbxiofqrp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/ghxxyzgbs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gbeuaklhy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/grddajeyp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/ggwdiquvv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gxccenstr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gvotmrajp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gzcglwhmt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gqlomvbxu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gvkdwbygp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gjiuwewtk.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/goskgafsy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gdbmvfxlp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ggxuhssly.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/grnrojsar.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqkyfknfu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtuhfzxzs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gqhsmygic.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/goululmeu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/garydzeyv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gwqlklcyx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gvjuvicws.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gkltfxdeb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gfhapqjvo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxjledbir.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gncirtlit.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gymgaiuqi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gwzdrdvzb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gkzauzwgu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gmbiuitmz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gmpndisab.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gbhesixbc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxgfpikgd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gfanjchnf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gbewuryqx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gmxlkrtqf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gjnqgbvks.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnhmgprrp.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gctidocei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggnajyqjn.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gxdjaycbw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gneyobcwi.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gjbjlvknz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/goabmupvp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gyshchrvi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/givfjgvkw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/goemiufxa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gvgqceozt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkktveszo.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/glqqanlov.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gnxbfkloi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gmtfoieof.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gsntehytm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/grljdwqnx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/girnctbvx.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gylvyyyzh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gzbuskxvc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gvraekdvq.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gyrkpbisu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gqrpchcyd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrmaczb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/galjrtfju.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/grehfzxng.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grddmczmm.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/ghhmfcuss.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gwibxllez.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grdtiijsp.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gluwzazmd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gjyeghjfl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gsqsgajaq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gxaspivtx.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gwoqpoevu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gplipiahf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gxlkzsjjs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gaorybmek.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gyvfylrjv.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gbtiveokn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gmygzymso.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gyiziqxfh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnfbayatc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/guacseamv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gbgljzepi.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/guicikvfn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjakvumpo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqjenxhfx.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gghdifukt.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gjlunudct.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gngkooado.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gdccbdcuf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/glohjruqk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gmclaqyyc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gpgcxvpdt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gxzhiuotj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gdsdjsuvf.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzkotdxim.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gpeizyzfa.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/greqthhlh.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gahyuymdu.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gfphjupql.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/galpephtl.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/ghmyuuzwa.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/ghknpxeyl.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/ghrurpfht.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/grbnunhkr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gknywwiar.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gqtbtlhhg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ghruoqywo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gvnmmvgnq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gpoqrsmqc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gjzhuqbes.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/giylyxeqd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gnccdfnsf.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvvnzyqqv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gunoptgzn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gckwetcem.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/glnizrqac.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glsegxnci.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gkmtqchud.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gergektrk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/goxjklulf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gklqznkyv.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gzssonadk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gbgimoomn.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gkssnwwmk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gmywaaxhd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gwfzgfmcj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggmjirodu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gnpjpkrpa.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/ggplzbmkr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/glbcuhwyf.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gsjhczwvd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gilmhnvce.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gdoirrkza.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gipcwrzkb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gwwicpmug.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/grrstmvtt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gkjdeiuja.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/grjvbsgyk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gapwsguwf.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gqkyfjigg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gucvzxfda.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gevqxslrg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gsdncliyu.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gcgtxthab.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gofmzuayl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gylukmxpw.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gfvhaijka.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gulhiyxwl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gmcypmnni.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvjkmkdcq.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/geilmeipq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gisbmbjlq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/grjvevjhl.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqbanzz.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gmadgotmq.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/givgamyvn.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcycjuewy.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gtoohqioy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gsdmnsngd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvjbffgtp.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gvsigoivm.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gjaydrbaa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gpbvundkf.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gutkjbara.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gtpmnyuhn.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gojfzsbzf.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/geduxziho.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/ggfzemwsr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gneakituu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gmwrcxtbj.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gwqhkpuln.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gacjcgroy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gvutbfxko.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gnqlsvlzi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/ggwxaovye.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gshufgzec.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gplvxxowr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gbixagina.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gtrxjvzvq.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/gmqcqtgic.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gnflsxsbk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gjoqawgnm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/grxnnhjau.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gqmjylonv.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gqtcywktl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/glzadofal.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gbuuweyng.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gktszispr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxkhuorxp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gphctbath.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gotcnewoy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gvtcllerw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gvalaxokr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gzxbsnkjl.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gakelysxm.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/givpvrtfj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/ggdtzrnva.sHtML


<!-- 参考信息 -->