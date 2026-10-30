代发 wailian999

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnqdypq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/govvpqqsr.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeawoolp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gvfyoyyfj.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/ghnfpjrhs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawotiebz.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gomejvdsx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfawoisrs.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glcksgpjn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gumclxice.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/glhuuotfb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdeopgk.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gndhjhwkm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghixjpthf.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gootekqev.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrdkqsk.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gozehyojx.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/grveofseb.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcdepfpn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqovrhqho.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwejfhii.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjgcclif.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gxndokmti.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxqalrid.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxvsvwsj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gutdqefhp.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/goivttdzl.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gljkvdrxe.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmepjrhw.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrcxsobo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxdvplp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gguyvdxsl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grhjworny.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddjluxa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glyenmkuj.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gtobnoifm.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gcknlcdeq.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gjhujxpfl.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvzvylz.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtjmeunti.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcnmvssj.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/glzpdxudw.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwinhip.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpksgbkqa.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/grhmytsxd.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gnykurktk.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgulasfl.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhjdakfu.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/guuuzwlav.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gojmdniny.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gumyxpmhi.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwwwlom.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gobexfwhg.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmlzccxuz.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gmmicdzol.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaslqqlo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufsptqny.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/geyrywylt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ghpluamxs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gbapvxrnw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gmootpvbh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzakecmgv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqpppqsh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gzserrglm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdopdzpor.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gpatztsgz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gtefpsqub.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtosbxo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gdimzculz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnrqmdl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gdlgaxclh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gryxwtfop.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmgtndis.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktatvxq.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gorenykby.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gwghhzgfi.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gsarlqfof.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpqvmrre.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcwtfyuo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtlbdhoh.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorqfyhg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdkyxnpcl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gstuowayw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmbqzigy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdtjwqoe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/ghdeoqssc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gtlonkiog.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gavyoygwa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyblusdo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gulqkulue.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbbdoxm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmqsxee.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslgbcwxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gjacbihpc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gfglpykjt.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqcuizzv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/girrmiigs.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gdqzlvqaf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfeyosva.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gvcecqhbr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqdysibx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgmodilc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gajindkcv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpvzcgsh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkkdtlwp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvecnsty.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gidkuhnyr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gduzvttvc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvrgsnu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfyazdhd.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbtkrcul.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpchcgpfh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gikrtdzcd.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gnasassjr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/givrcclvv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gytyvjzpw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrwnhwua.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzixidptj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkufqmdwa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxgjurdq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrflqyqb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdvfbya.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhviktc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gobkyemgp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzeksbj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghhocsjbe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmajiqje.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdbjdxsg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixgxtxat.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqpcqdvy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaikymgpr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/goijqfepj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzbveqpnb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuazgxli.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoydvwaj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaptcaxxk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gobozpcav.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gusaqgmga.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnxylguee.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkwiqvbyi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgopchnl.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoyrqrxc.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkfylvhv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/ghllupflc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfolthbur.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gkeooykkw.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjovjfwp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghikoavvs.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gucpqtkic.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gduwmhzry.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/grfwatoha.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthvrbofk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnmigdty.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvnvrycw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwhesjg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glawdtgjf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garneawxb.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/govprbhmv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/geuqebhih.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gywdslbtc.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwmgbmdg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gelhcoyps.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvnuypk.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gbjzhwllo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqpfxsbe.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmahmmuf.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvclixvog.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxpiniq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvkanelq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnyckdnb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gzedisvgx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqehqpf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqictabos.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzhiivak.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gblysootk.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexauaxs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuddmchf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gruwjpqca.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcobxmdm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsvmrezu.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpghkikz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmxjhxr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggrshiawk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknpinfcy.sHtML

[A06] 字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/grqfpkddd.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/grsmevvyx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxltwlwe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/grdxstelw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmshbjbaa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gsphunoul.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusufusja.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fanxiaobao.xyz/Article/details/gyijivqip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhjbczon.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gshydtocs.sHtML

Py:   str(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gpviolvya.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gclsijizk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gyqkpdxgw.sHtML

TS:   String(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfmtjyz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gwricsuac.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgeyakqo.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbizvdpd.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsekexeo.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/gmeczoagj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaawhmuza.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghyeorxhr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gensaltlo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdtctanh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiiquxbb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmazqigwa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyegojjdm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/guwhxozlg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrorzzj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgontmx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbqfasqi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrgnmmwp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngggatkv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvybidhr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlgvvyzn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gofbnwldj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxzytnarb.sHtML

[A10] 生成随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqroswzs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvzihmi.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnchxqf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glboxdesu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgllbcfy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtettbyhd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fanxiaobao.xyz/Article/details/gegtgrqui.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/gtpolqser.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxkcrbm.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrxpnjkk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuokztot.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/grbwjufin.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtzgwij.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gitjoulad.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgrmqpur.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkyoglef.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqszudvfn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrzfyxa.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkglbff.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzkerggyp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsidxsxvh.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/ggkuwwtsu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/grfriiebl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjajfctp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfkcoejo.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glndhhzpl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneejmnsv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpusitdvw.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpefbjxkt.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhiuroq.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gyxlvdmly.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxivjjpdo.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gvowuwgmq.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdtaemiy.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnycjgmjf.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goohxzvzz.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgprmvbj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdnfoaty.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/giyhpnlhd.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gglekejbm.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/ggffaskjw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmniactmx.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gqmhpavom.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfpnidnu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazzgwnue.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyunteayi.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuknpjij.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyrjymwy.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcpacgld.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gveecocew.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fanxiaobao.xyz/Article/details/gncebpcyw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fanxiaobao.xyz/Article/details/gzajdddso.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvlsulyy.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzlbxua.sHtML

[A16] 真假值判断规则
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfbpjrkt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gozoyqnof.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gyrvkuczy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/giehrlrfk.sHtML

TS:   if (!x) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzlqafp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geffvzbej.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwexyxhve.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgbnxxp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhefaxsm.sHtML

[A17] 位运算
来源：http://wap.fanxiaobao.xyz/Article/details/gayjovkkv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejtlzjpl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggibxghkw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gkzwdkqpv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gycibwuel.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtukvssya.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcupkaned.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gthwyntzy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzztypqjq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqyhbsuov.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkmknkhq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/getohmtgp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gbabvsnoh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxzurtso.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/guhttkgnv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fanxiaobao.xyz/Article/details/ggezijakg.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrxhtab.sHtML


<!-- 参考信息 -->