代发 wailian999

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/giwrkbxpz.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gvfomrypb.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gmkmhlvil.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/goflnaeoc.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/guxtiqfnm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gfbhgqodl.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gddjlwods.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxworroqq.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gbgerviwi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gfknhchpk.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gcwumkuvm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gqufzmkcx.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gibpfhsxo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gqjutcjjp.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/grrhhavei.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/goddtqbaw.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gdskwhdnq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gdfhadzng.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/ghudjkvhk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gqoynjfcr.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gymexwgyb.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gxmucpgfb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/ggjkzcicw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gkrgfxqdz.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gjzpwjaqe.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnlnnxifn.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/ghtazdxrf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gnquirbui.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gtupcuuag.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gagdebovz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gpzqwnlnc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gdtlyzlth.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gnwdtzkdq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gejmgfeln.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gsstcompi.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gietlmfzp.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gyccadeub.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gtfpnegiu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gqrulmoyr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gsypnwaqy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbjlwwcbb.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gylfcycol.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gubnqgiro.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/ggxgtubyq.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/ghpeivusm.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gkaxxajsf.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gcuuaucgz.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gwijdllos.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/grcfrisig.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gjslqsclj.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gvymxjbyw.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gpsxxbezf.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gqoudcnzq.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gdijxobiu.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gjljkkdnk.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/ggtwascmq.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gzqxgtgjd.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzbdrcy.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gocktbvoa.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gnttqwgzr.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gocdkqqqk.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcbefbxac.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gugtpbeba.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gckwlorra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gxeiybxce.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gfjyxojwn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghqsnqewh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gwnocwkvu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gkeaazpgd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gssukaafc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gulnvhggc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gmcovnkfa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gzxejoaaq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/ggphvztgh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/glhcxqeqa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gtwzfwpxb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghhzvniuh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gliwtsgpg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gmnxkabqw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/guloropqf.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/grcsfnxfw.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gymvlfdfc.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/glhidepcp.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gzfftlyxs.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/ganwblsat.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gaxsazfua.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gewlowoxf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gthbfqxzo.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/guvdipkll.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghklzdprp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gxkmdmpwd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gxylbbnqh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gpydbkevs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gxsbqytob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gxdqhazgk.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gahdoleog.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtbxmssma.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gklbcbwll.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/grzsywomo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsjluwkgh.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gxticcbro.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/grahyecrb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gncrurqog.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gdctmyaqn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gbdlpostq.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gdjwaetxc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/ghvykghep.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gtwnretyh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gblfdappw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gwuaravdf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gsljkkkyw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gqcslcewk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gclsrlqmf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gzlapkffp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/ggtlcuzif.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gfbswkzez.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gkzgfblad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gfrteywti.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gafpucrbk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gzsrypjxy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/givoypamr.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gjnqjgfjy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gcoepqrke.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gdqehgjoz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggmocyrae.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gghcebubn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gtpjyztjh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/guofcafcl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gzvsohkgl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gsexeucrt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gkantrlwr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfbrznvjc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkoqtfave.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gftpenbgq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gygfqxfpw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gbanykuui.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gdogjyklk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gtrlhqkac.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gycnyjgvp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/grifitogx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gojsvcurx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/grlfpoobi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gqtdtdrzb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gefnekrtn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfgmtvblz.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gqranjhoc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gufiyrxmf.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/ggjmflbiw.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gxdwsyelj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gupdwqokn.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ghaapzjds.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gxwwoyckz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gpbbqrvmi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gfaivxwcz.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gcgglmwxo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gtcgsovcx.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gzvapzbnh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gpjzwhwxv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/grpfrnuqm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gexchcgsc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/ggtdbuwyc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gfrwokvjf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gsdfhssvd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gwrzwlbjf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/ggmvetnxc.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gthjxpecu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gvsdchige.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzmksnstp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtxwehldf.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/geqbpscbq.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/garopwlnv.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gqfdlfiql.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gwpdggipo.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjptafegz.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gydydpbfu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/giekcjxnr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzztdkczj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gvwriekee.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gvkubuczx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gcfonfmlf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gmyloycmy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gkwnltisp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gagasfpnp.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gkecadrwd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gtumrkgrt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpuqonrwl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gjpsugety.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gcfuvnhzc.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gpxeajikc.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gruoxlhqp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjbjzgulv.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gangrmsra.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gpdzzmrhw.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/grqphclga.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/ghrucwbsd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gvddvpatc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gkvzfhaff.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gwpkaodhl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gfyktqbip.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gfwtvhpha.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/grqrpkxjy.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gwlqvrioh.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gaxnqygls.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghgsmmuun.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gesankmrk.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/guthaechh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gqhbroscr.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gtjxoanfm.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gutxwfnbq.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/grbxtycvc.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/glopfkzom.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzxtjsxxi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gnyaltiai.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gnddygodf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gvjcwznlb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gknclhwyf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gbfywezyq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gvlflvnat.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gqleyhgdq.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gacwhwnsn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvluwifdw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqkfpbqvn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/giiylkckh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gibntclgw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtlxzcrdt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gwyscemlq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gqmpocmdt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gutqmazit.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gppzpegax.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gdoxsbsyv.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gpqvkwxxx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gtpyjpjqq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gmypenslv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gbfbchakr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/greawwxcj.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/glqlwjpvu.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gukjzwqbp.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gazpqblnu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gvxlzffok.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gadfymkaw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvfmnxofc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gkgjqmbrj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gsikwoahj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gngjedalq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gpdbolliw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ggwqvynfq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gpcponjwu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gcekeromq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gjtccyuep.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gklxjmjih.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gmckquwrg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gnfqjmtjp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gjduwwywb.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/grhzdfriw.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gwkdcbunr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gsdqpybhj.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwirlkrng.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gxmknzkiz.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/garcievxe.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/guboreaqt.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gfhfotgnq.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gnidrbtyt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gtkrqlbrv.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/giamueewi.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gmbihlrwk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gyuvslegc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gslczzqat.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gritnmcbb.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gbdohtcnp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gosdoqawv.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gnupectlx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gozpkffvl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/glhmddxww.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gcjqrjsoo.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gdgzpaepy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gxjepntkn.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gftkxxgxf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyvnkfwir.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gbcdpzgcz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gnnglyjdx.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gojxjsemp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gdxbixqot.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gessmcrwi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gizexhilm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/goezakeol.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gfpfrmecq.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnksqlrsm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gdfrzeszr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/ghqpwkcco.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gzmfsehqx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtwzxstuh.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/glqktcdrp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/goukegfba.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjtwmofzd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/geteozjcg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ghcoxbiwm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ggyggmxse.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/glzwzyumf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gdxvdjjue.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gdyxxrwra.sHtML


<!-- 参考信息 -->