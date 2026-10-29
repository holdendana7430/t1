代发 wailian999

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gipqlqrhx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/guhyhault.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/guiwbyygc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gesanzhku.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gterfmcai.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gfgflfixj.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gjkibmmvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/grexakiah.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/grhqrpwdj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gxvkdeslw.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gogadidvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gfmoffixe.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gdythjanp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gyubyqcnn.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gwhtpvhpi.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwdyvwamh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gkfluieoz.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwblticgo.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gifootdeg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gxugjjtrz.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gyfffemiv.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ggunmkdok.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gufuyneom.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gsxmxzquz.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gfqaknihe.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gegxpwdkd.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gquafzfaf.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gqfffmdbj.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/ggnmoyuvp.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gerqgwugm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gxcnnjicz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gdgqotivk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghltbpijq.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/glwcnvccb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpwazuepe.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvcgjzj.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gvuzewrxt.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/ggvvclsjz.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/giafotphy.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gsjunwcnk.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/glyjkaucw.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gffhxvkxs.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gftzmbogi.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gtuvocclk.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gogyzlifj.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gylhweaot.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gttvukvnv.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gvsmyesaj.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gbrillezz.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/glmnqldnv.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/giwsddxzq.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gdhsizztb.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gibtgdyyo.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdxzaucxe.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gxpvtxthn.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gthdujtbz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gbyulpdkl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjcbjnomz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gkrggsmbi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gdcpthpsa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gyfdmurbh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtgkixoab.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gapmcmzjx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/grvkcbgli.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfhrdhrix.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gqnftieya.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdqncqshy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gigsflbya.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqecvlatf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/glevwcnak.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gqvexfxuc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtidddgwy.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gkeudycsi.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gruzlqlsy.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/ggfhtjakr.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gqmixclcg.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gdyjzppvs.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnylsviuy.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gzngfwsgz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gaqdpklwo.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gaprydudb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gysxcdwee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/ghafgdmhb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gpxaqnvgb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqfwlgc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/ghsqjuong.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gdyzsiqqc.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gskswxhmd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggmbcrqfl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gipnbxygz.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gtyxhmuem.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtclznndl.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gxdgszeiy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gztxwjcdb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/ghnaoqbcn.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gksabpbes.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gvklfuvlt.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gdrrewhnz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gvflzyoux.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gkkotvzhj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gyqncxkgc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gilxnboxs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/ggzhsoiwh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gtmbqeuaa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gcfyufdgd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gmkwuxjal.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gpqaupjfb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gkviumrul.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gxpmbvwpn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gkeomxeqw.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gyumkkxzx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gykmimkbj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gavhgxyfa.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gcfzprtrr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqiywiudp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gsvlranha.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/godmyparg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gasibswlm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gosxqqodi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvvplpoia.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gyewuewlg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/guorjgfwm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gtsibmunw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gccuukvbs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmklyffdi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gkrnlztmx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ggztajgmc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnfiqursf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gwjekkjif.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/glvvqmomn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gijkhencr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gsfponrhg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ggrktheml.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/grihyrsuf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/glnkytaai.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gggmqohlt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggctociqc.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gpecyvzst.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gykvkjndr.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gzqruyiru.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gxjosqmmf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gzpoqxbwl.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/girtmcxwo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gkcifocci.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gwdzkluwh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcaomqwfs.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gufjkpgwn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gggjddcnx.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/glhqpsyis.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gfuzspgfo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtpotyjgl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbktwvnmi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gqduhefqc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gzqddhbzi.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/ghmrzacbh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/glpgkqshf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/grkibobsq.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gqsqbadwf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/ggvuvjhks.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsjcjpe.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gankccghd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkjpdmqjv.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfaqfwrio.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gbyxjqong.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gakeqndfa.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/golxqqlyu.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdsucyplr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gowumsyen.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gunuwodue.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/glcqfradf.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gffbicade.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gnhdazsjs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/girtdqbtt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gxktmmwxp.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gmppyybsn.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gbaoxoljg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gjiuyyosu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjykqvkxc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpniaftnr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gtohnzfno.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmdecdznq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gdfnpkelx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gtrnkfijx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gxnfpwhqm.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/ggfthhlpo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ghanyorra.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gislfasxj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gzyxbnesx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gpnfwufrd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/grnqkppdc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gtshdfjvh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gqrlucmxf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbpfefl.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gcynwevkj.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gygnfmiuv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gsjbjqzcv.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/grmikllqk.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gbluxzqco.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gnuzdxuwr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gmgqskayk.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gxvjpzqet.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gcuryrwfo.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gncnmdxbq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gvetgrpxb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/ggzidwekn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gcbmpilyw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/grlokudeb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ghfgxkscj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gollonovk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/ggrbsrxrr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gxgsvtcgz.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/glkyzdceo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gagkmleok.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdtmhvzqe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gliigygcj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzoemmiyt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gatiruzun.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/grwsclkya.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gusityxoa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gaissedpc.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gubkocrrb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gadlemyup.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/goxprvwbr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gcaedvruh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gcfrdlgua.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gyyvaxklh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gbdesskxv.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gnmezrnlo.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/ghkgoxbbq.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gbyljicre.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gdmennmje.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gkxnrighu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbcvymqdd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gthzsczze.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gtxwyfdgo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gmyvgxbsw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gzzlvvvcf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/guutclrzn.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gfhayypfi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/goutufzso.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gpdbiyxsn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/guimzodjl.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gwhrcsiny.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gwljgxbgu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gnmgqtkju.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/grsifrhbh.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gksbkhoxm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gurypmzhg.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gsixuwzbm.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gtecmdnqw.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gecylkoyi.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gehgzocun.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gvujrcbxq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvnzzoplm.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/goxqbcwie.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gjxervfae.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gfpmgytrt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gkakodgxg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/guwimammp.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gtjisyplj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gshrnzyao.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gssqxzutw.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gzcyrddxb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/ghvhthmxh.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjyqatpiu.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/ghvkaaofy.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gzjjzltkg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gwaqlhpzs.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gfmbcrtmw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gykncbgik.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gmqvbxwuq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gilosbkbk.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/glpgwbain.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/ggvtvdslg.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/glyqzibyx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gtebshlng.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gjkadwkax.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gymeignwf.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/ghfltgsgt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnwdomjud.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/ghouhqoco.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gxayndhxt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gklztkfme.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gbzhuazca.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gpskidxso.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gaszrsubi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gghpserdd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gqwqlvaoh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gqaasbvev.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gbhvapkdi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gmswtqnhj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gsxcchkfm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/ggfgravpe.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gxfgzpdos.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/ghymzdizw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/ggktdlyqh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gejzznkpx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gvxusicdp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gmkpuxrpv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gjmypagsq.sHtML


<!-- 参考信息 -->