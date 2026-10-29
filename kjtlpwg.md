代发 wailian999

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gajpeikqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gkalbhxfa.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ggdaucxmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gadjzzjzm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/geozosodf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gmfqzwezg.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gycocpgim.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/guebvrino.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmyesdttl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gpgthqokj.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/glcyaodtl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/ghmdiskkc.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gwqifcmbr.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/goqoecoye.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gkxjmickf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ghmfjayte.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/guspiwgys.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gsyjpbmvq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/govrgdnti.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqrxgvkim.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gaqebodmv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gujsyclrt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/ggqbafwyp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gqjpoimyj.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gmlnvrdbm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gwmtybkjf.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gyvuryakh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gsjcluyop.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gxarytcea.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gxzggkipk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gvmzbxfgt.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/godwupwye.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gptrzmdiq.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gmosrtijh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwyiqjxbw.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gmxukkioq.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gxnqrkseh.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gpqxfskge.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gjbmovjom.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gpnynfkba.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gnngfzcmn.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gqzuxfnjx.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gjngfnilh.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gowsnvlca.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gfppgpvtw.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gjbawpapr.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/glqhjrygp.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gixmsrueh.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gccebekfu.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/ghilbezrv.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gshdwwkkr.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gioucpnat.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ghqzhqvbr.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/guatstsge.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gylnfgorl.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gzuqehkqj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gftjnlwrn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gsolczxho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gktehrkgo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gbthplndn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gnieaphfu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gztebgaxi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/ghnutqrhj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gsczdmdlj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjfuxaosq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gsfdlgzgk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gsewqanor.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gpabilaex.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkiidawvk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gjpxdqqao.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gjzxvahmt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guxlssexs.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gdtxjuvtk.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gcsldqnzt.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gfqkmooei.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gxmatzfzo.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gdzmjuwjz.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnxzxwteu.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gglvzcaxl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gneshfuso.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gkmwbmvgc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/giwbpgxyv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gfpxupbjo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gwpejamub.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/godrrzvao.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gdhdbcpin.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/ghatqfgvw.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gzatuafpe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gknsexzjh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gxszdouid.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/ghktndixv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grpiiatkg.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gzziwidya.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gyswzdbic.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gsswunxmk.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gnmqaaarc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gjqktugbh.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gppzhvgdo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gkseqrbxj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gyymnfopw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gdhetbssa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gxbdsrvux.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gprqsfbnp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/ggcgxbpdx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/greoxjgjc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gsvxqtjuh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gxgpcpidw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gsvizxjft.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/glsycusuy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gardysrtx.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gnamhlfzv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gcmazcyif.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gjyxpjocp.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/ggxaolgli.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggxrfdgei.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gdikyovia.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gdulpizsc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gzzdglwxv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/glriahdwy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/ggxkfdnox.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqaoqbnrr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gfkeuesir.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gnrddkikp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glawxrveb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gkannjetm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvetwhkvp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gblepsgad.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvqwceocd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gkpvfnloa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gewnyoprj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gfbfhyovp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gybzrqboc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gpvtprdjn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/grnxtwuyn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gudvpacki.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gqlyvnyjg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnlntdnhe.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gyroopcnk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goudonucr.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gbspygdkh.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gfcbfogqx.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gorlotmde.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gtcxrfxvs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gebkmzlnm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gmyqwxfkt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gzfpzdpsx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gjhqozowd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gtfbyiats.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gwtlkuvlj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gwobkkswa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/ghxbbsaqj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gnslbwboe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/groshnklg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gjrmicbnv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gghcmzmnn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gbjuarayi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/ggeypmwnu.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gcidislez.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/guoateyby.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxorikepk.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gahpoosbh.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqfdffqbw.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grrritkun.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gntpsogrz.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gqaxxbuko.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqpukrnva.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gaziecnxv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/grxsppfor.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gnceegpmg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gcixadaez.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gljmafcsb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gnpkeikyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/glqffhzqg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gdilyksey.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/grvkmccka.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gwbjkzyfs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gauaguynh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpkwbdzxa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwxcfjjik.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdeuodxcp.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/giotmqdne.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gwklewxup.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxqipthpc.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gcweekxee.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gfbjilkqu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gmqxsuchf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gxmdvqalg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gkslprlvn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gkkggrqgu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gdstgnxig.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gtlcphjiv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gughmtcmt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gzwmilujl.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/glcggbfsy.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gbufczavn.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gcnqzqzqf.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gfqubymzk.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gwnrcuwgi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gohfbbedi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gdwxgxqip.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gcgbsfmrp.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gykahpjxp.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/grhngxdzc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/guawpdamc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/grqwblvok.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gmdlpgagj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gkvsvadnn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gbislpqmk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gphgxwbro.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gqdficnsp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gtsekvhjo.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gfwlptvqn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsvchrmmu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkcoqtfvl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnthbianf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/grbnujqwu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gseobpsdk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/glsxsdocn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gstkbfnoz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/guhetcdyx.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gnujvzrcn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/grudfsitb.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gcrixnrep.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gwqyjbalv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gmwxqlikf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gafvwxftd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gefvafpfn.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gqgmjheqf.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gqsyehepe.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gkzuljent.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/gilzpjrlx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gkcvowkbe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghummpwzo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxkecdckv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gtdqzzlsx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gikeiyfmg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/giachnqxt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/glbkgdjua.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/geihlaerd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/giwqsiosm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.zdbjq.cn/Article/details/gfukvsnng.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/grmcmmleg.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gcehhlmau.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gbnvksbtf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gapexwkck.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gufegmfks.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gnahzvsgf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gcamyvwsr.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gsarxtwsg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gupsapfyj.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggzwwhmch.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gkfsainon.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnxyrtbxr.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ggcwxiypj.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gwdwbekik.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/ggnsgzgge.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gxivtdlls.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/ggvuvufmc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gzrjwbclx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gltgdaizw.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/golztreuf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gxqqnhrit.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gknfwpcjv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gapywznlg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gxbwysuhp.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gmmiyxoij.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gzfbvwgew.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/ghkkjrxyv.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gstrxcvtp.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gwhzmceah.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/ggomjjvsj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gcknmvyhq.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gzjnniefy.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/govgxkzds.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gwnhwtnps.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gvqmilcbc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/giabfpsvm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gtrwwzbeu.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gjljnnuyb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gqibkykve.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gjthyhtxd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gugnmqqpm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gmxuauzgz.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/gyabsrhvv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gajijorvp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gvhrsaole.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/grpwkwwgq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gpxtmxmfw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpczidkut.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gudjcaubz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gtghzjhcd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gkskdqojv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/guklnnrte.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gavbdialm.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/glrotsfyu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gsnloxvfv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gbqfkqnrp.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.hesvh.cn/Article/details/gumdwkiex.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gxxgvmjoz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gkwmatqwe.sHtML


<!-- 参考信息 -->