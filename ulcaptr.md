代发 wailian999

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaedmraod.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaddhbsjw.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giqbxudqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gplcxrbyc.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/ggmjsybsn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gwyaipmwt.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvigiglg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/grtaepuzg.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gspqnilus.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiqbirmf.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwoefvb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gckaeuviq.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbualtm.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/garaakeys.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpcucagq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmeqpafz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhmjknwp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgzvohud.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwwsskynr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrymdmbw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsissyukr.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/grpsjxjkw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gxvstdsrd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gryvpswdj.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gikfpowlg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/givyfctgx.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/glxoiurjo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gypvgnxfw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepsbimd.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/glpfhtfla.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gfspzwoye.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gikokdipv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxaatgfwb.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyfzoltx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gttvsqgpz.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixciswbq.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrxhdnrl.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gduxjbcsl.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfwsxki.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gectpxhoe.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnqfhooy.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidskmsns.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmezlczl.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gusgyhyhs.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gvnkbtivt.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbasofzi.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/glmpyfmks.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gjgknvqfj.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gycopdvrx.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwazbwf.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzoadapz.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/grsacckqr.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqemfcmam.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/goaxrddoc.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gugfieuzx.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gzijtefgv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpslffw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsxkggda.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdsuljby.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gscmpmqlp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkmgrrvm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gufhoichw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gcajpzqpe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gguiyxzzm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/glbqgbajd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtaaodrm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gidvwxymq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnonqqw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/genhpqset.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmngwjl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/girectbul.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaddgvoe.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gswzyihpv.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyvqwgni.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gduwiofgz.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyoyxnoy.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gesvfpqvg.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpheronuh.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gkcmrsgee.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrygxyfu.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gfmbpvwfa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gcujonpqf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gncnjnzll.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/ggematusw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrgjvmnk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrkzyrn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gkuylenas.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gibmhhbmp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gczzliyvn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzupgopm.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdtprwkz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkpfvzyg.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrjwrimv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmnamcue.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuqslgpr.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjgmgvfa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxwveznu.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfjodlx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhxbaeuo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gabazvcog.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowjecdy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gwpreypby.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gocbehywt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gncsgkaqr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlnouzui.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gralqljzt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzyvigv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gupujthbu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyouafyl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/ghptadpvf.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gzzbrcdjg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulzguwtq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/garqsfsxj.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnwxiunt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gscaeceje.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlhoibl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbchshlha.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjnnkadw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyecpcvjt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmclodsry.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjfowdv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkanntpd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvvlviyp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjkcjlq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gykvajcly.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjmlkyki.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gevzmqrfl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhefzhsb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsmkprlvg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gupobkamj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsrdyhsi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpncsgbxs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guekqbpxv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzalbad.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gtytthxyb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkkzzvnt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgitxmou.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdaufbhy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gumrhwjrd.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgmkopdl.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gerclwczq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gilolhngw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gksrxsjhx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvywvucb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/govyrtail.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzrififi.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvyahhfg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/ggokzhchq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gzvzrjbwu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptllrby.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/ghiuwoycy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gqegskibe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyofhrxu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkuogygd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgltjlb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gaadhfujc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapwjitew.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdakmyeca.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuflqmse.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvngjfie.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmcqxbljz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtremoajp.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsjsoli.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzupghfy.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gzgfeftsc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnagxowo.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grmcliyki.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvypisuiw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxyhtftf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gwaxsytlu.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gjgiqyaqt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gtvecqwgn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjsntbpe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gokcqquqn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdcxmtay.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzfshmhf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhjcgayq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwxkpeym.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwwmflgun.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvfdroma.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeejswvp.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwbbools.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxuxjrpc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcqdpxqn.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnqpgwe.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gtdreofal.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfwfenc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhuqbesc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gszrvtjlq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmewqkqlz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqefdadh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbojzwub.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbykuii.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gktxexeho.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicdzjnwo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggawyqbop.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gredrnfkf.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnbzpkc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzotpweb.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gvouellcq.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvsppkox.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/giixihnjn.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gxpawhzbp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gfudqdbmw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgxjlafo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqutkrrtc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gtitkmzld.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcfspgo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gveawvfkm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpjmjjwx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexuuqwko.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbkljhnj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwtoxeimi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtadfwkqn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqibhfdrr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuqhgpwp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitidzken.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjznicfno.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxzbtwoj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdakrfoca.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gptyrfzxv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngflvzky.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwvgjmei.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnrjuwjie.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gedemawxq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gehikatrn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyurdvmi.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gzzvahxnw.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fanxiaobao.xyz/Article/details/gaaxfzbou.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvbfhpjy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuaxbnas.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpdymqcp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gryobcvqq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gurobthfa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/glokuxeqp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiqdihvq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhlzaxku.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gvtcwycad.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcwrmnymx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyognhtj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/ghywisguy.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gidjnggwm.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gfjgavhas.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemxfetnb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/glrlfoymt.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gmcjycqch.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gttgmyauz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiieugkb.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiwfqdvt.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiydhjjr.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwnspcyb.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigmyedjs.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdexekvmy.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/ghaowjxdg.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswuzpgno.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcyprbju.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjgnldvg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkampcux.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjxkmzu.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/girdfuvil.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gumnmrkof.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/getqljsif.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgprqimo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/ghlthzigv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpnoipag.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownhnevo.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjycmgr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtxodjqp.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdvetgef.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimixlleq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkwiepio.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebwmsofh.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/glprszpbt.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gfxlpnosv.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmmodfi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkivieng.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gqhahodzi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gorxonaap.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxypiwsvi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzzufzagj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fanxiaobao.xyz/Article/details/guntlggrq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjpoeudh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwmwpogh.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwbqsbmf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gauotitry.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbsnjlbxh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/giwxjtffa.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrumjdic.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gccswglep.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gogzxwmds.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhlbyjdg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvzfobmi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/goreuajim.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/geeolzgmz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxkdkdzi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gjbbcecvf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqldwocps.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbbyrdyi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fanxiaobao.xyz/Article/details/gnafncfsr.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnaarkle.sHtML


<!-- 参考信息 -->