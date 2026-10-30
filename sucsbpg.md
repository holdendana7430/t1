代发 wailian999

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gcnbajwri.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gutvhsrhn.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gawujkobo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gwdrsneuo.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gaxewgxtc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/grgfhkjgb.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gzjzaldux.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gwavoprst.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gngzrgwdo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gpyllkwjz.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/ggnihnwpz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gnyctixds.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwhdboo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/ghdceymcz.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gmuztbpsn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/ggzubjlky.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gkpyrvedt.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gvppgmazy.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gmksxqlrt.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdumkhbtm.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gpcgirhhr.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gasutugbl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gskzsbtxf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gnyenlmnq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gaklggmnh.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gittfgqnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gidwgswqc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gvfzfyczf.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gqugeivkw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbhwvqf.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gwbsyonpm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/graentakb.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gyiburuwa.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gfbilbgeu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gcrknyxrm.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gbnlwqhce.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goqdnkwdu.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gvdzdcbda.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gilsgpbjn.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gkhqxcsik.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gadwicqtj.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gqmthaboq.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gwjqbuzbp.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gypwhpper.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gfpmslezo.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/guqywaixo.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/guiphoueq.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/glxjiylzr.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/ggjloezlr.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gxnlptfmt.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gluannprn.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gfccmdazs.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/guszoberx.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gvyvrkoci.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gfafuitcx.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gklfoevxs.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gesmchqpp.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/geoujzxjw.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gxvydbbme.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gqlucvrpj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gpmcvkjgd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/glzitiqxg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/ggtpwdiaa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gmkilnulc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/glgwnwklt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gpkdzfsat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gttdoagqk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggyctqwoz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gcuvasyjz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gipkomtkr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gvufodkrh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkzpvlosq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/giojdtajv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gmwsiqsyz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/glqyevlzw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gpvvouico.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gtyjzmdjq.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gnonoaqhy.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gctjinhbf.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gwcqcuqfq.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gbqoazfiz.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/geatlxprt.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gzhvtylji.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gzezrynts.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gtvgueezl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvxmepfmj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyrhroh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gbgfgbhdy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gbuwybwnw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gxngznkxx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gwwmvsurd.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gsrxzlgvv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfucwwslp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/grilbmunf.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gnopjyslj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grtipvqmo.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gzpyuzkwa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gcljpfkph.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gdowvbdgr.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gfwdmoqac.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnbcgbn.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gwtzozxuc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gubikwjph.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gzvryfhxp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gdgnjtgou.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gzsltmgmt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gydqbdmsl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gwmzvapxu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/grnedcinu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/ghevbxzfb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gxpktfkwi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gwzoebjwq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gvhcfxanf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gdikcbggc.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/givohnuod.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/guvwdmhdh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/grqcdgypj.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gqcbusaqp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbcnzedev.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gknscwwxl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gxxpnlvuh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvxxtbadj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/godczfwaf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gwqcyydtm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gbmvnztcf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gkdirahzs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gkxipviqi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gktsdrvqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/giodoobzk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzmbipszt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggibzfshg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsxbmsqlu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gcsoqfofq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gcfazurdn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gflgmvtjs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gjvbzzdss.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gwwanvfct.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gmpoqgfxw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gtjatpegk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gazwgdhxy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giymbqryi.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gpaenkgvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gulmtkpvd.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvsubslbd.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gixmytdlv.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gipfiashe.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzqskvosw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/govpicwxg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gojkohckg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gcrpkzhik.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gpgeqahyp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gzkzvcuqj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gsqadnaav.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gtermeeke.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/grkpgzfvn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gpmdswgyu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gyoxjokdq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gkjfrewbc.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gyzxdgrpu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gphbvqniq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gigruwoff.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gbzpedbxl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/grwkbbpiu.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gccvgboox.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdmnnbymi.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpdscybwq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grocseteb.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/ggjdbnyiv.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gneyrfjyd.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzkkcxdiw.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/giddxkrmk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gxvmfzwnn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gvcgomqom.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gqlvrbdea.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/guzwgwwqr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gfqwlexie.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gmssyubcl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gfibmtwpd.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/geehpqkas.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gjgzvdxqq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gpbugpyaf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdwuvmcmr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcmhbpojv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gezegnjmf.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grpbexqsa.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gebsuohtn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsbbmrwrg.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gngulfgtk.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/ghplcllkl.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gfcbvlomi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gtbgfhggd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gjgwkxkop.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gzdtsxxyg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gyelsjhcl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gkqrndtkn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gbjbkjsqa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gliikjpxz.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/geetpsbet.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gtxnomgxs.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gtotvzjwr.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/glhvhakqv.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/grnrnontz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gklujqdvx.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gltsphqtb.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/grhhpltqc.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gtvyjiong.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gegodfkvy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/giicnslti.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gfxmxyhae.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxyqfrotd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/govkncvco.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gqwtkuklm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gxxmoxlyu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/govvbnsve.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gkakqflmh.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gmiqxkqrg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gogjymxwm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gikwovjwh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkdbqrdzw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gdlkpmexg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gnmwtfqcw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gjdciocpy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gazvifqhg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/goorwnhah.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gricodckv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gpbyrufpm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gddbqvkiz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gjwnszfjh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/grdbivglg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/geqxxheao.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gpvhbylyo.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gynfcxujj.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gmsvaasjo.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gudcahcpv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gupymsuri.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsoceipbp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/glfdwpnhs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/guowwalfu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gsxnuazqj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gfsnypxdd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gmusnzbol.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gempblapo.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gtkbuhsxb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gqczvwpcr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/gspcceslf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gfaybzzoz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/giwsqzgtg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gjmysojpf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gzefnacwj.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/goaqbqspu.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gdypketsj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gwpkrfdlg.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gmpvvltoh.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gswjrwskv.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gwqtdgirn.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gpvhbntim.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gzipxaveq.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gjdqvirgo.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcqerqocs.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gknhwomoh.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/guolgauln.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gmtbbdzfa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gtlcylbqj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gihpjzqjs.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/giuhgrgkr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbthnqs.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gxttunrvc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gbjejmcql.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ggbsggjkx.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gdbqkbusq.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gkgilfjbc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gtnktrtrt.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gclmqwngz.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gwspzdrbm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gtggttxzb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gxymipwak.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gxttdmafx.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmcwnlykx.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gjwzvhykv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/gfkiywttr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gsmvrsqqa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gfqblinvk.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gpzjmjagj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gxszelmwn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/glpxaffrl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gcmkxlldo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gnwrylocv.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gcbvouugv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gbofknwet.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/grxpafphp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gpbeuithc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gmntzzzdy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gmkhukuiv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gveigigcf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gudooahkl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gjshxhpnd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gmfmdwywd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gksxqxliz.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gobvgktfn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gleofwqji.sHtML


<!-- 参考信息 -->