代发 wailian999

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/ggtmluzdr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gbiqzmpwz.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gchhvwxsg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjkoooeig.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gqgoinvtb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gbkmuusev.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/ghlkybdwb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gmdkihjcc.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/ggehafgza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gkvjuxpzj.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gafkswvrm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gmyjtavkh.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gwtttqzpb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcetcqyax.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gwkwmozzn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/ghcadsoxv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gfepldaxa.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/glaskklzl.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gnwechhbl.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gpcfniglj.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gpwjbvxxp.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcchkvuig.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gqblogwzi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gbygbxsev.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gwlcpevms.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grziweipx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gosvlwool.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gfsreuwrs.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gtnnumijc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gjhpxslhd.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/glfiauynn.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gwfnyupls.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/guqbfxsxs.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gorpckmei.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gkxfcvoug.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gkdkuzjgi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geirxbpif.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjztgyi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gakrcediq.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gtcinuqyg.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gwipofqlz.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gmdmrblis.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/ggxuqomaq.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/glmlxxygq.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/ggsojjxrh.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gobvlovlx.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gsjegfanz.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/goqshlklf.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/glnagovwq.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gmvofarkw.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gqdnchfat.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/ggzpcglce.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gvexurmmu.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gsvpdsrex.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gbkhxkaec.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gthnupffu.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gnvwvcsoq.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gedgsqeca.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gocjjelus.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gjmhqotrj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gmhjjujzl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gkjhnwvgt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gnvliusfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gugjgnwqf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gfmmfotup.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gzojvaraj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjvuqitdj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/ggtwvytzw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/grhhuiiwh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gmphsdinp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtczylevo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gaqpgyjaz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gogzheilr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gftrynoaq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gnsmxcqyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gohgkmwze.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gvjlomafg.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gpnuxnixn.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gdyffzkmh.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/geqqkgfrv.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gblyzkqsh.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grkucrmkg.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/glatvbflc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvcaskqig.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gfbhdfaty.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcnhmbzru.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ggmqrvflh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gouqcymff.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gjtyooekt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/glsnlheyf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gcffonwha.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gdfvlcbmp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfelsinmv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gevverjly.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gymkpkrsn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghuzadyyx.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gsctmprbc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/ggkxetwwp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gfgqrsaxx.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gpiswppue.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gnfpupjzb.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gbmpifbqz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gtbcmbacd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gdvawfyjz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gwlzsvrox.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gntgfsync.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gqwsknuef.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gfvuosbbg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gaxhncpzj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gtmfikpgy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gjfgqrteq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gguoxpybo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gfihmcbcd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/glaliocdr.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gfsylipji.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gltadsumf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwrumaqfs.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gmkeqztrt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdztdlgga.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gvhxsvpjg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/guimhheav.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gglaeegjj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxowojwcy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvpjggbrs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/ghzrkuuhv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gymfwtazq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gcqbkfryk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gbtoancgj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gfdzkqgyd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghyxoqeum.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmzdzqonx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvejqwpqk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gjjehuanl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbofuwddu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/geirhgafs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gixhoueir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdqqkltct.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gxkicgrsb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/glmlcubab.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/giksdixps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtrxickwc.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gjwymdwto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqwlpvtst.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqgrwqbjh.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gspdbwwxz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gvujddlkv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gdlbkgxzo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/glifbhqwd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gifjufxre.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gcknkhmqk.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gtckpoolk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gyocypixu.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gafdyznxl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/guxhbmiuw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gpfrfcicv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gnlgeaqfl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/ggqvbwoeq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gnwypxffo.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gicbegvva.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gmoobbeua.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/guyhvgwai.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/glmtusuef.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gokwogmht.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ggpneggga.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggualptkh.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guqusbhya.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggkelydfm.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/giaffavbh.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gqwptwpsa.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/girdiuluw.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gvoijjaux.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gfduunrha.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gbgjlmmez.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gdzuvzygc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gkwtdfksu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gaqcpbmnc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gvpndsljj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gnhiabbed.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gbymjysuj.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/grqauqxgo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gphhccocw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkglmbetw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gsjtaeacz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gycecxtjy.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gcxemyjpa.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqypiyutw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmowthxyy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gggaagtdb.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gmzpvuntl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/glbmlfjrt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gzudoyjrw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gvbuvuyyf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gokhorzkn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gbghhyisy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gnradqswt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gqnlqhmab.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gatyoolda.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gynfslfec.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gibufxilw.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gvhkypijs.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gohifvzrk.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gkuiakpsu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/guomfzmdq.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gkzpyrkgm.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gtownegjv.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gwibqnscz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gmugubykj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gzmygdpvc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gabzpqwcc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gaccdctds.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gnrivoeec.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/guwqxmyuy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghocfyfee.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gjnpzxgto.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gkcswtlco.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gzkgufulv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/giepjgcrc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gosmxxnun.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqydeldtm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glanygvme.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ggrbyasgd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/glybthpch.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/geatpfbfy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gglbjwsgy.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/grquscizx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gspjwgftt.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gmnkvugsu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/glrkevfng.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/glzrhazuz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gmpcpqvzt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/grmentbbi.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gxanagnny.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gethuqrwp.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gotqgszqd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gstiuffdh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gmngbmchn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gkprluson.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gprbstdpa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkgkmgwfm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/geeaqgrqb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ghxobetcy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gtwlxocja.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gazsxxfce.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gkwahftws.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/glteivdck.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/grfmgrqce.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gbzelnefn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gawzxukrk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/guelkjikq.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gejdhfilt.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gxjxtqsvl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gpkswprob.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/geivlvvxd.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/grhgtqnlq.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gbibwbmir.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdlbovstu.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ghbcwkstf.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gfdrmspfp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gstncuopz.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gtosztsga.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gjhoscoir.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gezehgonm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ghpllphsf.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/geifadcwv.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/glcjwukys.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gwwapztgo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gedodakjg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gfnqhtijs.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gbkofnnyl.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/grjorypat.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjfpzbj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gszfimlyn.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gztozzxtn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gzvdotfib.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxdxurj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gvywevzip.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gsytofieg.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/giffhzsfm.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/ggmundret.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/ggjinrhtw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gpwfsuqsm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/ggwiwybfq.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gpahapsyx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gbfzkkone.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/grkucfjeq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/grsaeoawg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/gdrzstzdc.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gvlinyhdl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxnrbkrsk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gkwwfxpvl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/glkobylew.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gnbtkvvpu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gljxpstgt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gstrjtbzs.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gqxtevake.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gumstxpyd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gtapokkwi.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/glvttpgay.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gtdadljbr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gvhgmakpe.sHtML


<!-- 参考信息 -->