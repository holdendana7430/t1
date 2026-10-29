代发 wailian999

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gfnwynpdr.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gprxkvdek.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gddwyljcx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gutaqzwkf.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gvrncpgwe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gckulaukb.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gxardpjjh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/ggbeeilog.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gfxcvnqwh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/govussxsr.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpjflihfy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/giyjhzdca.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gvujlfwto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gsvkmqhdk.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/geydgqlly.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/geilhiyxd.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gkcwzwqmo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gxbdttryu.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gsjnrwdlq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/glxqytima.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gldvkhjfx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gomwmdusn.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ggotsxodw.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfhoaxjvj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/grhhqjijb.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjqgdvojt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gokhijkby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gatfuexhf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwjhqaccc.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gbklrdurg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gqgtdhuxp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gzzbsxpfl.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gofwwtkwo.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gjuwvtgiu.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gucmuegua.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gnosbqgve.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gujluplir.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gypooqyds.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gmbiisdih.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gkyutatwv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gngislnnd.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gbydndujt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyxtgmekw.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gqlqphzit.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/geepjgfki.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/ghunsmjlt.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gikidfpie.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/guadxsybm.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/ghwvglymd.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/grvdkuyju.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gicuepoms.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggsjsiahm.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ghcisoefc.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gudfsmqed.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gbimvacul.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gworrcsio.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gmjuokqao.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/ggdfyuncr.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gtszbmfvn.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gplhavhwe.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gmebavoxi.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gulicspan.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gbtoexlkc.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gsagfssam.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gdmijztzy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gzoiexfxn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gpeuwirku.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gdrqmqtjt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gxrqdwfad.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/ghehgneaa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gisicpggq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gljmeoucz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/glnabzrkt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gsmsttbzs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gwxlmqmyt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gonuvuwkr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbvyukzkz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gjkpkljrw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gqnofeolf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gujuvpiux.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/glwqadtgh.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gcyryeahr.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gjneehihv.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gsauqukec.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gforpmltr.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gshksquwh.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gfkwqebdk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkdfapyyp.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gyeeuqkhr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxfsrxwhg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gaudirmyv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gnhnfhasn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gusmqndba.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gmecfvkte.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gxfsocbvm.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gwjjtxwtm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gemyrskua.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gvbmdepzm.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gekqcdvpq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaxkruyru.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gudpdjotz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gcxretyzu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/ghxrnplgv.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gjgkndpur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/ghjclokvw.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gzujdwlfe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gibvlvust.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gokrbhrli.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gpuscqrjr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/geomxenio.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/ginlbhadk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gqiskfmzp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gqauzubmb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gwjzjqarx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/grhcisnxf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gwvmekzmn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gvpstbzip.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gyenmeuln.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gtrggljfj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gbsrnusxu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gwgrngwjk.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/glbdyzskf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gqgiioday.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/girziioyi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gdksatyet.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gckgtutua.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gznklsscf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gspxtotmv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gyxwwhzbs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/glrydjzgc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxjrsxxuw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqseanmyd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/glevbnhgf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gutzclgcz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gucepamua.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmghohqlr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gjyqsiikv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gvfafboht.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gaaaicirk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/glpggwewh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gnyvhxesd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gounzckzh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/grypyhxku.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gvwrogbjm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghjijvdyw.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/glqebmrfe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfsctjaub.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gzrybxvct.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gmrddpjdt.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/glbfqyqgy.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gnolurzeq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gspjiwcgj.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbjapmruf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gmlpfkqty.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gcqrbtbqs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gvsvuqhcv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gnzhfdcnb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gvnjgscnq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gctzotlkb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjajijvj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/galqntovi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gmayzedrc.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gpizgzrfz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gvfqxnzwi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/grxdqshwv.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gfwctvfhk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gvghqsszv.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grrnmtndb.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggndkyvrq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gshlvrkmr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gibdthveq.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gmbdeqzvk.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gxnkahzqu.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsulxjmxp.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gfvudyrus.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gejramwmi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gjfebhpkg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gvcjskmuy.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gfxvszrqq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gihodvmxf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gwoiammav.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gyxfugusv.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gekzbwifr.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gnkcrauzg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gkfnxiuys.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gkjghubsq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxxvirvud.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcaqihpga.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/grkogvvha.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/guvmaczlq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/givuukobx.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gtvnahbba.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ghzotnvyj.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/giasbmouo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gnfxjzwdj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gzxbwzvve.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gfprhoxuk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gttvvqtch.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gnnwivlnc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gyjalkbil.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gwsvbohej.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvcrssakr.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/ghrsvinte.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gacqevsfx.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gufyyfxyg.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gwkcexjbd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gvbytlfqo.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gaaspxxef.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gvnfqrqur.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gjxgaqhjj.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gwbkdkarl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gkmvjtuhp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gedcjjhqw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gphahyesz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gtljemonx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gauyotard.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gtwjzcmjp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/goljvhxwu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gwwcvenmo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gsrgccytd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gdjapmqdg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjcfxzpfv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gfdhwfhoa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gftnbhizu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gedefealq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gpliurjgs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gskoxrhdi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxticcdda.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gvknsvdwt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gmyuaoqdd.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gdsfhoppm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gdwlfrorr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/grbdkvlkf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/giuoezbah.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/glrhfxooa.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gwqqiblfq.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gjoebacsa.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gugabwhes.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/griksgpvx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/glwuslnsa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/glihfwthu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gmfsnlxkh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gimgdjcaf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gzrjenzjp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/glcozgzzq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gmtbsunae.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gamdbtpdr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gcgcfajbv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gathiuena.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gbcheygyl.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gwqavlfma.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/ghnagrtku.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/grqbnlbiu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gblfxkvat.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gurznfmac.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gcygiahao.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gkdxsdzbf.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gpsyfrsfc.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gyqnhoank.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbypmbqek.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gxwvzopra.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/glmivcjdj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gsslhjgmx.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gokddokns.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/gkvulocfh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gzjpxehsu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gahaevard.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gksvzqnhn.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gdgmqyhao.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gbidibjyv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/guwilixlj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/gpcpuhwka.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gydapzazv.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gklumafcd.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/golahxjmo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gxlgkyrti.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/grhypkjzn.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gmracwgwg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gznlgisje.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/grqshqxze.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gkjkkdzpb.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gbzsvirno.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gyuwnobxn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gykqcicbw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gjzfsybww.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gctvdczpr.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gyofqldzr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gdfqkxzkv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/glzwmtmsm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gnqmbhjmy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gqnwmfbmt.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/garfemdrs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gyudhbqlt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gqsudxvev.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gqmvckucp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gfqywfwoi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gdaggmxvo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/glcahmjxo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gfkdfplds.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gpkillyfy.sHtML


<!-- 参考信息 -->