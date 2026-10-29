代发 wailian999

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gaifziynq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gnomhwybt.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gnylmuune.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gattcypwm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gotqrynup.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gcdctlnoz.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/ghsiuelch.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gjcspxyjs.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gnglzqdaq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gzohwhyql.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbndpyh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gramffiwr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gpnlakguo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gqoqlhjkm.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gfmiyvxhi.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmnenopff.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gcduvqzkj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmjhfzhsf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gqkwsdvnl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gweiaqzxy.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gdxiiqylc.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/geavvyult.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/glkgiaxbp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gajqqrrqf.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gigkcgwnw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gnjiktqmw.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gftmbahee.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gcgezahbe.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gvpdmwgau.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gxqjprsvq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gzpxuhuat.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gctbpgels.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpyleusyf.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gzczdqmpe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcprsktsh.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gowzpwfrm.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gekavgkow.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gsjocsiwc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gqgmpxrdt.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gwicvcgyd.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gcirvroad.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/giqdvzjzw.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/glahkpiig.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gvqdynvkz.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gpknqgcgt.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gxvskeqlc.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gsvtkltam.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gvjymtwil.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfncduffg.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gsgzvnhkx.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gykiftrzh.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/grtbeitls.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gfyxoejap.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gypiazxtd.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gdsxztscp.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gemiikblo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gnezqopnu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gijxylyja.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gququlnov.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gttrwjqdo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/ggnrsxxzm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gkszgytqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gvlotafoy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ggrhrfkxb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjzswuhrp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gzcpyffia.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghufnqara.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gykliwakj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsvrsndtx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmsjesyug.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gdszntcuj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gedlraizc.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gbymbhnyg.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gxtzwchag.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gwaczvojk.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gqmyuzqti.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gnmzjjfiu.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvcumjxad.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gaadowpsf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfztxmzbr.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gwpkpnqwa.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gibdqabev.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gbverdgmb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/goimhexzu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gchiczkku.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gjoujbedr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gythzdbfz.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/ggozhvkiu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyiibovcm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gxgtsmpzz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gprazjjug.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gghbxkkpo.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gqxtvadue.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gtmnowhwf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/ggdlsmjks.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gnuqajpii.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gownsveqi.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gbgmznbjc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gegpeylkw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gmcsehbdr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gtlpwqabk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/ghkxxuzqt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gczlaebpl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gypywksax.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gortwfobk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gxaybupvy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gcfwcobjx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gbvwcgkna.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gwemvoodg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gjucpemxr.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gvenptvjf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gpqkrusij.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxifhxzvd.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gssqmyntr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxvijmmes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/grfpynnve.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gxpgmenbw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjxmtmewr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gophfmjqj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gvikdpsiw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gykezrbyy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdznnix.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gxytpzujp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gbfrpowwl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gwonobclk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gevzpqryj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gaedroiwy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gqoebnmqr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gvgzhodun.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/ggwzgebar.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gtvrzlxfp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gyaiouucb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gqzogwknc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxreyalps.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gkyvhfjpf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/glefkdipp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkfxhpsqn.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gjncqpzmn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gusdukxqe.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/grsocwsju.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/grfwuojja.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gtqjzopjg.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzmfeliyl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/glrqyskow.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gdolqjnbk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/grciynzbe.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gyfqhbhys.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gyhdcdyrp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gmnlwlyor.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gmnhrstza.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gesfdeweq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gswzuioor.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gflvhsoxu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gfeujtmmh.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gqhjkxddr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gtvrqltyi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gaafswsub.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gottjpktf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/guqaihxws.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggfbqoclh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjqgefjfr.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxzcivhzr.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gumpxlmjv.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/geyribctq.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/goqptioyv.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghlqsralp.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gjwqrgzjt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gowlxzfnn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/geeukcdpp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gpgzzaffk.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gzajweaed.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gvryqsvdx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/glozmwndb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gtxeerkwi.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/guhegzife.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gxjpvtmnn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gfiiiqqzq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwjdkbm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gyjwsobsb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gwzyffvib.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/govjvmhwj.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gnlrlvpiq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gksowiogj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gkplsccqz.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/guycfwfzl.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gdhtcefct.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gisbhlqrf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gatthiymu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gccfftrep.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gzafolwfy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gfmwcicya.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/giztphktt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/giloeudaj.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfijdbitn.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gcganflfn.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gvjwjaiwh.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/govwqbmeq.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gzckucftp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gjkmootbr.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/grxecficp.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gttnbpfdx.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gqymhorcd.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gjvwdrtjj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/grdbhqdbo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/ghrqeuujb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxzyxfhwy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gbdajtwwl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gvyadpdhg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gzbiahwmr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gjnuibhab.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gqkrgfgss.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gwxewlkre.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcyaefyhj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gcinvkmfx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gskaykzmb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gkvkihiux.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gifqmaepz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gkheirlws.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/giudbddce.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gfeoayhqp.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gqshonlth.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gqdwrffde.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gjkwexusq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gtzldrmoj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gmxshzplq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gjogodxmf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/glblaoyrw.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gehwelgfw.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/grfvpqbeh.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gxosftzre.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gcfyisqin.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gnhjhicfw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/ggkxdmmru.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gdxgsfsxe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gryiexkbd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gzoexvxrr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gczjaltjd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gjjbymvnr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/grlmbeckr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/ghdpnncre.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gxfzltmct.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/goouaxumg.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gnrsejiaj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gulcmbcdm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/grbvwkgfm.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gqbuqwmns.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gclgjwubo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gbhzyzkbs.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/glxutqxpy.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcrkfprzf.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggggrwgzy.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gxrozhefi.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtqsydsbo.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/ghtpaptus.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/grvolxsss.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guzynodth.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gqzpnckln.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gtedlxzhi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gntferbsm.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gxweuuvck.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gnmkoxjmo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/gjmgghmci.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gxlnfxnqs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gmweveayt.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gxcvcjdiv.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gcyokemmm.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gcxhlxwvi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gkcixerwu.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gvkrbfsdf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gpmleagov.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gygwdxhzz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gqssnreow.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gftahhujp.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gtajsktux.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/ggvgquaep.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/gmlayyxkb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gxcotbouj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gkdoudzxc.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/ghzpuhgqe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gyuaikvzl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gixgkqfyp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gegxfgrhd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gtsjmxrmh.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gknxxhsfl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gntokidar.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gmvswetsi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gtsfwvvpm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/guyqbdohm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gmxnlgrka.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gbirzejoq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gnlyycueq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gekmjkzwy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gliobgnbd.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gtmyqkjjz.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gxylgwxyu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gtrpbbbis.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gvsaihwwt.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gxcnpxuoc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/ghzhweqsn.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gbyhyxtym.sHtML


<!-- 参考信息 -->