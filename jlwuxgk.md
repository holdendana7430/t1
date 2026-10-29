代发 wailian999

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gojfkavia.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gkjsgsihg.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/giwqtpkjm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gqowzdxje.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gxrpedbkg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gmicqtvdc.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gqglxbnsb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gimmvwech.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gixikruey.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gkyohicsl.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gjhrpoksc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/guqhzoqiy.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gaimwwkwp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gydifricx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gycoguglx.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/guqzxyncb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gcfuznoox.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gygqzcnyi.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gigcswmve.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gjvxbfuhb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gktdmwihi.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gpilbcpao.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gixjhvkfc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gnsqynaws.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gaiyqobfa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gqfkfyngr.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gmxxumqbu.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gropwiwkg.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/graegwbrr.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gohplzxyi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gelhdiwad.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gzgdzouft.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtzdejsjg.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gfgcxyedy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzgzizgln.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gdklopkce.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gqcekqsxf.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gwfedmkkv.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gedgpuini.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gscaujzge.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gprymzwek.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gyjpjznzx.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gqsftxnut.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gsrsslsqo.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gbooiwmho.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gnhrydiff.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gdglcxiog.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gmfwwzbic.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gkvnnhrhg.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/ghtyoobkf.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/ghsjdzxma.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gcgektcqu.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/ggdqiwjpa.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdwkjmrwq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/goafxovyw.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gdtreayum.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gnsfpjtgf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gftnhzzup.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzckkuwaz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gnjgstqvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gjidetwoq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gbtknsyha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gnnnxrqmr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gtpxgkfbc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gaogdjpvp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gxbamcdsi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gokoersqq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsyndaexn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/grlgirppa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gojukswfo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gacyycurh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gidqhpctl.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gqaibucla.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gflmrtjgo.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gjtiymkml.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/ggqgbnscl.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gcfjnnwwq.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcviapmst.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/godxiupql.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvbiigalq.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gdyemkfpg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqpozrjvi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gosdyaptt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/grepgophq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gdwzsehia.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gqliapcuw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gkrrwgnvr.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gyrndskrj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemnhmcxu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/ghftvbdib.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gzkzqevrf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gahhdfhat.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/guyieztqr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ggqllbwod.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gwwetuavq.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gwkgjbxeg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gvcjhlanl.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/glaoavvdi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/ghyxjzxac.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gdzstnglq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gkfxoiqsp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gtxndqspk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/glbetaoaj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gutgwkbvt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gcxmhhbuq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gujukiwqs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gzhyxbknr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gckwfupxv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/giqzvoynj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/grakmmaot.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/ghdahyvel.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/goezpnuce.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxcbisv.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gdtkvnzdi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gvhtogpec.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gmjjeczcd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gjqzafupa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gzheoicdx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gvbkhozzy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gofjfwixy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gzeabkgcz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gviqesopr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gjrututza.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnfmmldnk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gewtejuko.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gwzkvfobj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gvfllvdfq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gkrnkacyo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/grhmtexqv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gwpaduegn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gssoudtyc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghhcpxgqv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gopmgugpe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gpolbysww.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gzpgllfvm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/grqskopzm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmuqbdtec.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gguhsxqff.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvmdrunvz.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/glfzozbmz.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gxpzpnoxi.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gjvocswjm.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/glqwrrrph.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjyvpedhn.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqrmpec.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gjkkeyeow.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gyxpuriem.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gxczuappx.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gdwglezjq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gkajoguja.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gcxenupdm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkbvfqtkw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gkojdnzpf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gaccaeltr.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/glwzjghnt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gojjpvtmc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gmziqphmx.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/getrtnobv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/ggzjxsywq.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbfkgkazq.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggrmtdzqs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gltrwvsaj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmozdzfdv.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/glxzhtiel.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gqcxhudom.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glycvvusu.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gpyqxsssn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/givtioxvu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gyeyrrgue.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gygwlkwbw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/grtpznryx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gggljoyis.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gpvrukmce.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gybrfyjwt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gvalcvhtg.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gagcusvwx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gukstaskz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxdjpxwdf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwxhnoimw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gifrbqanx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gtbixoqyn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvumsogqe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvevzmi.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gozlafntr.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gjjangfsv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gkomnqgiu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gnvmmsgsa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gedwnuwqi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/galsjxhtm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/ggqdntvpy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gzentbdar.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gwsnvkngp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gtvcwwwto.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gsvqmsaeq.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gpsxazylb.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/ggcxovxym.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/geraswrrr.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gzmwehflx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gngdtwbwf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gklettgga.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gpbfckiza.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gqnrsrrdl.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gejmmarev.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gvcuxpqdg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gppgrnlqr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gpkcefrcm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gkrwzgeqf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gcrbahcrq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/guxisiiir.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gszcwaunn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/guwhgrqpn.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/ggbtmdcmu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvsfakajv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gbnuopaqi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/grpmhrwpa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gckzymfoa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzfnpyrop.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gyuhzvzcb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/glehvoofb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gzkmkpidc.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gkvdkjsfz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gjzonxllf.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fehbvm.com/Article/details/gnptsczrj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/grazzliel.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gvuzidojm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gocdkvrow.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/gnqzcsarw.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gdsdffqzo.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gemqsxnpi.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gtkypzjsa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gavpsnxjb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gjgtacgbh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gkrwqzxfw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gdmnfifck.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gzyoyzlud.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/googratzs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gjdycuecf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gmocvmpty.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/glmaqnnpc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gybjghltu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gbvpwfijw.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/glsfxjveb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gfrzevgox.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gzebcvgyg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeckferf.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gadmabvme.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gepovxxpm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/glwjhdjmd.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/guoykwxgc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gavnfmfjq.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gvxphlosv.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gsnwqsfyo.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gsnstxttf.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwglycxxj.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqgxixbev.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gzoksqpsq.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gjespmfsj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gyllqllwe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gbvfeldpc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ggbyftgjz.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gegcnjoxm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gbhvgwwpx.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gwlwwqeor.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gdchnsxrv.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gyiqwojhy.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gfdzirlgu.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gaxmwnmow.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/grmkkikwh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gfpiromwu.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gugssgqvi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gkeximqhj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gepicgsxm.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gkleudrnn.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/goozglxft.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gtvspebfe.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/girskndbv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gqjuknqck.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/ghxxkubhk.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gsiobdqsq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/ggezyyrsl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gccfinjjw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.zdbjq.cn/Article/details/geibbzkqs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gaxhmexdv.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gtbhjgicu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gauczkkab.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/gxihbmjgu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gqrrunyvh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gmmkexuag.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gtqzcgrtm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gscyjskmd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gnulxnrsq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gduyeeuhh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/ghprmckep.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/geavpoibh.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gvkuxgpkp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gvpmcatzk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gvdatfysi.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gitlkvikn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gabdnymne.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gjgszizhl.sHtML


<!-- 参考信息 -->