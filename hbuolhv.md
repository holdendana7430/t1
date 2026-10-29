代发 wailian999

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gapeskhwz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gqrwucrzk.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gwvdlpgnp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gshidteqz.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gymtpcois.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gnsvswbyq.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gvasmyqks.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gmhycrgsm.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/grhfxayfy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ghdgeuzqb.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gmzwwrmhs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/ggjyehrfn.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/glnikpfoz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gnvcpqlsm.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gtgylbpnc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/ggoqxenxg.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gaavtxmvi.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggzjsllye.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gzelpcjfd.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gscdircpy.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gtpisymvk.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grlcjrywd.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/giypbqhbj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gnrbnomhy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gtooyidos.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzpzusfgn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyoiewhky.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gyzqvxgvq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/guhwkazgq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gdmvbdgqb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gkfpfusgb.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/geabfzofp.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gxqvcuqco.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gbvaawifj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gwnjqmlqk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gjehntyys.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggverbday.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gywijuolk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gakjmbifo.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gddtovhjz.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gsabadtfo.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gbfeuonrj.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/guqhuxqau.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gplfhxtsz.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gvhtgryec.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gqdcfzvti.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gdaxmgdgt.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gprhkkyvi.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/ggslonkvs.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gkowssnlq.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gtiyhzxsi.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gfjgnchzr.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gkylchqpf.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gfwyhoqpu.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gijqtrvpu.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gnxhhewvr.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gjbhjphqd.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtrmaazxq.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gigpaozyx.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/ghgmzfexq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gbzwssmwz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/giburfzqx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gjbigmfeh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gevpilpct.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gzuxzeeme.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gfvbhcvuk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gkluhpuji.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gwofcpneg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggrycvded.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjlsaspmb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gsbkkqxej.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gwirnloce.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gnzpjqpdq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/grrmtbpqy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gvqtihawj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/grdymdssu.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/goqkyaymx.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gbpdtnrei.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gcbdzqtie.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gbicxyuyw.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gowsrkeir.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkoimelpy.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gvprepjfk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grisbjqpj.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gxwdxifvy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gdkrpaesu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/ghmwtggcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/grpmzqsvt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gdxkteqpw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gxlgcpxef.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gchmtewwg.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/grwyygcod.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzzzogjuw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gtahckarw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gkzqgduid.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpwuuhoge.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gaftqwlva.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gwvomlvzh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/grwhetifn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gjgbgcrmj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gtxdrgjuh.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gcdqshufu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gahfqjcri.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gjyogqlzm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gydqymvux.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gruylxhjc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gxziibhos.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gafvprlhr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gewyyeucd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gpebcinrm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/grzkcbote.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gjvviudiv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gnrdzpgzf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gprzglboy.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gndprwazr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gafuiirig.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gojjxqgmc.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gguobczwm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfrsizcob.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gafrbmuen.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ghovkitit.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gcuunoivr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gwzquynyg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gchjoyzvw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwjopiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gcagrthfd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/glmlrboyf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gponripmb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gmryjoznd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnlvjbxyi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/griemeael.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gwsdrrgrp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/glgvgqebh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gesqvkcur.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/glxutaglh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glxpyuzzj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gcoqyttrd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gguzdvoyd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gofkncdjf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gunlgorxa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtkmqvkxx.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gevjssjne.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gukckzrky.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghphavzpn.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/ggjsmlwsq.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/glgvtxzth.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gpmyzbuwd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gickckpzv.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gvyimdmam.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gnlebejil.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gnjnxxmng.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gmwyoievj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/geixcvojw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/ggdpclxnm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gosvfqmkp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gizuroirx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/grotuinlo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gfwmpxbwv.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gseqpnbsq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gmorshixy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/giodgbnbo.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gijkdtcom.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gvcyaoaly.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gucevebvf.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkbsusixp.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfpihaiyt.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghwkuhlag.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/ghyjnsnea.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gcxpdwzuq.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbpnyrxwv.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gjanfnwpn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gzgqkyguu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/galfahqpe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gukystlvy.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/geoihfsum.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/grbheqfbh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gbasvxlkr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gkvfaluad.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gagoulxex.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gnapcyzsp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gnvpuqhuw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gdnfkwkho.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/glfijywlz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gucucqeth.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gybxcwxex.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gnevlotsa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gxdwibast.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ggraptenb.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gpragmhkt.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gcrkswdlw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gjpfopevm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/grfimvrpv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gocnoosmx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/ghuxxzelh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gldearqlv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gvvpoigeb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbawjielg.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gruhhumec.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gshqmvggm.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gjexpacpp.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gagmwxvrb.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gtuxqglpz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnkhyhe.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/gncmbaohm.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gfqvusbwk.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gjhbmpuvh.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gjusavohg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gdlenwnak.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gxrbhzrbm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gkhpejdnr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gdijumsxx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/guxzosfeg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gaqnnydrc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gzgkrsaeq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gomytsdpp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gicnvsimf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gokyuivgg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glwdxsjie.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwujcjmic.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/govwjneqi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/glntgsrla.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/ggifxakqr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gtnoipuok.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfvagzruj.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gptwbeybq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gyqhngleh.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gsviljzfb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gcbxqanzw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gtlskvkax.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gpfiftwhc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gxqzgbwot.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gyuutlpht.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gtvdskrlu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gneiyuewo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gvuwlqzjx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/griehyxcr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gqxkfcvvd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gmuiwtxhq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gpzuwehkn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gnsserwwg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gsflqawty.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gchntbbqp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/ghusjfovm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gxbteurkp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/gkgqjuxab.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gqaeucaao.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdslhuqdd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gqhiqzigy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gjlxphxit.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gfuvhtdua.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gvczxlyiv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gdhuakfqi.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gvyjbrxtz.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gedqmpihl.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gflglvdwh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ggxslyasn.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gqhmitmxb.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqpxsszvi.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gqideixyv.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gwpcmnthq.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gqdwthyvl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gkmrydshz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcvtfbuys.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmltbmhip.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gpmbzxuqq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gxstiqqsq.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gujivouqc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gcpueyrzf.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gtayxrpll.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gzyrrlxau.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gmokryoce.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gphctvtyr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gxtvgywpj.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gezvivvjw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gsajqrrig.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gfbkmexeo.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/ggtwtvmpl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gvvguzeba.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gndiohges.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gnkihkpmr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/ghgjjwvma.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gtvcesyjt.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gwwaegeim.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gorcldtzf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gbjprbgoj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gqbzsskws.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gtkdsqyts.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gsjlenkjh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzpmxmgfj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gwdqrvdus.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/ghylpuqnk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gcetoyisj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gvjfhddws.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gggjocxpg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpcyvnbcf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gcpsdqhnh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gzfrxyndb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gttfajmbi.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/guuuxdcsk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gbfsrytfi.sHtML


<!-- 参考信息 -->