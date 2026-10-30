代发 wailian999

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gplffmluf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfamzxdjj.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkhcolhj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gftuqcbiu.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdopadkqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gljjunkit.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gvdquxoep.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ggbgryluk.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gutnugffh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuejcyon.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gcduaslyz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gludbcoge.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gggtzduea.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gayancltw.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvkfbrkd.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/guuuucqrd.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpoxtrmr.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gwqpdblwl.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvofvvtnc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvucckg.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gomvqljgb.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gymjreeme.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkgqkipk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxbtfapr.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzmgcrfj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gritgpmem.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlyfczvq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigvxjjo.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzoazuto.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gqajflqur.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gzysosutm.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gzsukrqwg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glbpbffoh.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiutfhhb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvkytcuh.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqtpdhv.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvtufhz.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfjdmxud.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gspbmemwk.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gecgitpne.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/giegtvdcf.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gdsjbxocz.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnxsiyoi.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqcnjjtz.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmgvpyo.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gxtjqodwh.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gefutukit.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyowuykm.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gikohqkpu.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzcpshfq.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlfkxqqz.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkahoavjo.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gtihiwfma.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmuksbzj.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljxhowly.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/giodtoqql.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctrdsqkv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gdottcecz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrozwsr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqcvnxgu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgjrxafe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gteplkeft.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpvxtucy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufefdkbq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gajditkhd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/geqkkzdwm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcbrnyxsb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gorjokxhh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gxfvggvge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvagjazn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gbruoqzyf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezguwgxm.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmlpvjr.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gymdapihl.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwlqngy.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/geahubqrc.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/groeutdzb.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsyfzmpu.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/grofexsnp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glufmyfys.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/glngcudcy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttsqfjtc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/ggamurxqq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/giwgihvgl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gafhmeoso.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjfpgcyf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghedxekfd.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbvozldt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiktvwdo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnoymfik.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnablnfk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfabbgn.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqflhtvyg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gegkyynbr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiqzzxrm.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlwpgwym.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gopbmgvcv.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gugluwnks.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwfplnv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgkhrxhb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/glayanice.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gnzhxztit.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gcyswyzap.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gzawfzhuo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gybhqudah.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gteygtjfg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/glxtyoofe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gipxrmfys.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqknzfi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwbqpihj.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/ghpsnuijj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavkgocyy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/geekmcmbx.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gswveppdy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gmzkpdpxe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnnbmifwy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusplmnsc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehlkapf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjzcrrap.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzovryjyz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtweeqhbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhomohvl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpticwrv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gptycgoco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gssndhumr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gubstrsbw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqfooprru.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gldrbpvjc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gfjkactpq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzkanapd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxnwradta.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjcbtih.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmrfkrqn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyonsjyl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvyeytdyh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrqzfbof.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoylmpsv.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gawupmgmr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtlmqseg.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gginuggnl.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjgaizag.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdolehgz.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gqlnrmzit.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gsevdslup.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/giqgzbcyg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gehksjfxh.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpsfoepk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/grqgzydgz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtvedog.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmprcgojn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gxmmjamae.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhvxeac.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoakjejg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjrfhun.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxspvgre.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmjauhhg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygmlhxrs.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gyidghlrf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/glgtpxbyv.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grzyhpmwv.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/glemjmtel.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjnxznlc.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gugtrfdru.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gaezwelum.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqseqgyz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gavxzwwzb.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grfzfvdll.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxnkuvy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvoaxcx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/giuhuojfx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyeyrmqx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/graqxewqd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gwkuuuaqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqnjcdn.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjyycna.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjmbrssi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmlznuvf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsewbojwi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghcmjemfn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gicbjmvqj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgsmkmru.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gljlpioww.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpjzoasd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpjmjvoi.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnpgtnekh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuvoioyg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/ganykwxxt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gufeeorum.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkysxgq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqwhygf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnhhzpts.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gjelsowdo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gabrqkded.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gicpaepom.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gedjpdqdr.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/grrtslreb.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gfqwzkajv.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxaannbl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gniygkqeh.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gslwgkvej.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gqfjnbuwm.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gqhujbrsw.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeqowgop.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafynkofi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaxiixtb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbfuzcku.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fanxiaobao.xyz/Article/details/gqmkiqfdq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/glmtypbwv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaygrgnf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslfdijds.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gengrcjjp.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/ggzrpirgl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gupviybnl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqwforss.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrnjsyzb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/geuklxmyh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gumhhirko.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtjawhj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gtpubdozw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfddxjqjp.sHtML

[A10] 生成随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ghzmnvqte.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fanxiaobao.xyz/Article/details/gyfospwqx.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzkztyja.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfkpvrbe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvasswwq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjrdrajst.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/guqqwztxh.sHtML

Ruby: rand(1..100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkmirjr.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fanxiaobao.xyz/Article/details/gvsnleews.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gyxfoesqe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfbdymbwr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnbdvowdm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gikdnbixv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmilknuve.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfpdczbsu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fanxiaobao.xyz/Article/details/ghbbfsecw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/grzpwqvth.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyshceqr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunzbtxjs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrvpmzip.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyhxlhoy.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gesilfzfg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwvxvmoo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjogxoon.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstxkufl.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszpoysbw.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gkbcxxsrt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gbkcsmgxc.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqanlnxv.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gwxzwzltz.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/goaqpcpwc.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcitzdww.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gswuuymnj.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gbdpczcqf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gtkxxxwjp.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/ghpbewyro.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gxgxjcoza.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/glacaxdrb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxjreqqa.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gbaamsrzu.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/ggnuvpwyx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gtuhkudpv.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gtaawjaoo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiyydkty.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gxrvkenfc.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcgftyzh.sHtML

Py:   value = data or "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/gwxlnqhwm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkumnirw.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/goyiroykm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvreiobpm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhcncplb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/goicxcmzh.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gcepwruqh.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gpbgmysik.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gaqqvvuzw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpdpxfue.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmzmbduh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/goqmxhhas.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gslwjhmxx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzimzawmm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcdilvpis.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxighie.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbrxozty.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/gonqrbarw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvfhsqrz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffhedbu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbayaqpxz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gdihbrgex.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpwzjhm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gczploqqg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gocgwkhup.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxogtjrsb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/geevscmbf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeimwylz.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gahjzpqau.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggszltziy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyhwzxzr.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfgaorla.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fanxiaobao.xyz/Article/details/gxelingzg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekzmaawl.sHtML


<!-- 参考信息 -->