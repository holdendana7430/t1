代发 wailian999

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gxjocqaqz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/godyfbtck.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gocptwuki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gkvmlksyd.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/geaswhwoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gzdjlzxas.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwoevhl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gqllxlnnq.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gvyfzyhrz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gptqtnryy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gsihjvnih.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcyhqowed.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/grunnswko.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gnclmsmyc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gkrophvyx.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsbrswhln.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gopjhvtsy.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtcrgxdti.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gkgxeurbx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gxuwwaxjs.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/glfkxltmu.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/guponsuwl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/glvllzkmb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxtjnksmx.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gbwtiybyq.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gmlizdqgy.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gvmwaiicb.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gjkothiko.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gkluhcvgd.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gpzfdweri.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gmsmltapi.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/ghxvimbqw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gumgcmqyw.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gfhasfvgj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/girauytkf.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gzgvhwdrk.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gjegjgpae.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gphyrkcrx.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gsspkdyjk.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/grquohtfo.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/ghuyqcabm.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gmewxsbta.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gtflgkvat.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gzutjlylq.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gvlgmfrfn.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gpkwyatui.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gxsxwxjzs.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gfgkypcrl.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gtwogenrt.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gmatskqsr.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gaatujrvc.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gkbpsbzkf.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gyttacnob.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gaewbfxyu.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gnhiyzzdj.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gucfszemt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gyeqnpcul.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghcrwynye.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gdmvjxnzh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/grmklhrih.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gekqvlyja.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/glrrqurpf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/grgeeaehi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gwkcxzrtk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxyjsytzq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gnwqbisrf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/goowwzcpp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcloakeis.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzjtihdac.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtacqvtly.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/ghprsurhh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gyqziqeco.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gjdmprfkn.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gtdjnpozz.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gzfjyipvg.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gpxbtfitk.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gzqxzniji.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gaehtuvyw.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gturaoknw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gulnwjcxg.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gvycxmudc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gtufigvxq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gzrobokqv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gtycxgitc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gbzjmdlmj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gyitkvcsw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gxzoexhho.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gzjpxyqwh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gytqucwko.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gzznvlqjn.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gpjdurdxy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmrgcruid.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gcapapgxw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/giotrsuxr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gibhsalaq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/grukkgjgg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gilesubqe.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gzwjfjzqv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gliehfmfz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/ggrgvzwmq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gtidebusy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gagurwrma.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gwgakkvce.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/goytmtdma.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gsorbpubx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/grkmowito.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/giscyumui.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gwapposqk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gtluapbme.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/ghcnfmdja.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gimrcxqei.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gmivnelbs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwbqhlvff.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/glkntovjj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gedjwjkdy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gbdspqcyd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gwwwseybz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gpslniqqr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/guargsbhd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gzzydpktz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gbzfqcpxb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdfyyvuro.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gmfeeagbc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/grkojtxbn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmivyxetb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ggfvlalur.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gdoizmzyf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtnvtfggd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gmjrtewni.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gthyzkhnl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/golklfomj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkpfuvbjz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/grvyadckn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqqiakfne.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gjdvsehfa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gbxydwblr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsetolebc.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gadwgbrwi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grggnmseh.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gabzoqfmc.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gzcrzvwex.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gzjlyhjiw.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/ggntistcm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/glmjrdnyi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmyukrf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gacbzdqfd.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gwimjwebl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gqcnhrfur.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/glltyoukn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/ggctpvjay.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjjhbzjco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gxtnbchvo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/ghsexcvuh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/geheoalvv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhmsxwn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gdpprckyu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gtqqvkmea.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gykeccbge.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gqurnkoqq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glaqpjdki.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghhbrkstc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggkcugmfb.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gskafdknf.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gbwfpdvcf.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gxcbkkupl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpqmtlqig.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/giuyoocvg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gyxonnjhw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gdzxcdigz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gubxecvne.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gzqtjgpkd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrwwnny.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gpkqpdtaq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gnavvwjdu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gsrnxmhlc.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gjcavayia.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/giknuqirh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghtbrywth.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdwqehzhr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gyednkxbr.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnyotgxdj.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxsczxoig.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gsnataahi.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvgzfelzv.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghlgauerm.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gtmapxfov.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzbfzsq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gbthlodrg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gdpiiupla.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gnhabkqcs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gjvucnjls.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/glfmoefih.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gkxrucgnm.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gfaecpvvk.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gquchfsyp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gmzhgwvoa.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gocwrkqvj.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gtmvklazp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gdlxktuaa.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghyhapciz.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gphqjxupw.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gnkwrigty.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gsvpxltuh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/grtdcyrmq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/ggqqprcwk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqespgxm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/ggybmhfrl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gzsdjjosz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gdwdetxzr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/geufcosqt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfarnxsdf.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/ggyglgtdf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gkhqxohwc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grxlhsewz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/giyxrttht.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gdusjstwk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcnxzxqij.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gxzglrgxj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/glufhdzsd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqddnhuer.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gloiubcda.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gxmwtwgio.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gmfletryp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gqmdeuqnv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gbhahdrui.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gvfjlfsoc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gyseyelhv.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gtqkxtpvn.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gkajmaiyy.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gxekzwvyl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gwpehrfic.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gubnclsqt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqjbtpjzp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gbkrdowkv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggtzpoynw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gmntuhisz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gpwryhlnk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdxifrdrx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gomyplpux.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/ghrvuydyy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gwzlclkch.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gskyosykc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gfbemfjja.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gvscgtkve.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/ghpezmmxw.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gjrxcieel.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/ggbypxzqv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/guofafsyb.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gekdbruvv.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjooyrbuv.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtpsxzzll.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmaozissm.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvsbhktib.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gwmbqmmhf.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/ggdppfqyl.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqlotmvwb.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gtssavita.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gkngwanfb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gneapmfyx.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/ghsdkcfhf.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gmcsrqjlj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/gghrhrczu.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gafstqwff.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/ggumjbnus.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gjtwvbjap.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/garjnhsgm.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/ggyqnooob.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gxlwlnqvf.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/giqxyptwy.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gfhaamrem.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/goyxtuelv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gkpauhkyj.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gzhjvnldv.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gdkqhbkbl.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/ggvgxplbw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/geobagjdd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gkamzpezx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gxnbgzdsx.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gkovzvptg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gndidsief.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gyknbeejl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gcsqbyulp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/ggcuwadsm.sHtML

[A17] 位运算
来源：http://read.share.fehbvm.com/Article/details/gekjgeqrd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gkjuefrqa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gtpmhsxrt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfdnttops.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gihgekgvp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gcdkrbyne.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gljxssarf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghrruvlrk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gzqpupurh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/glpckyrkv.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/giqsmfnjg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gdabnybqy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gttcojldb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gzpghmacg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gavrascxe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/glvkmcesl.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gyiipdfsx.sHtML


<!-- 参考信息 -->