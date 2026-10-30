代发 wailian999

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjctawi.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnubtsanv.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxslpoxnb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmgshmyn.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gikciacgv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwafkdzza.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gehlgvwad.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gwwyfoftr.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/ghimkkxwe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggixwibua.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrxbucyb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/goedzhzlt.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmdqyfh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxivbdz.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gltsvllnf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiesoqeh.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gbkfxayim.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkntqimi.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gdpbhqzqr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gduwdeydo.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gyjwfqptf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuacteem.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/guygpbaoc.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfybqhzt.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gaktnxubp.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/grsuzndjy.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqwfcwbu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdmchqnsa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtjpwkl.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gytvdluww.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gejtlcqqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdnoyvimp.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gnjzvjyth.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhavtvjv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnweoprhd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gntmlsgzx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glulvbznm.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnxwcfy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glufheekq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gojpgdeht.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/girofgogj.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gnvwmicpm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghiwlzpvn.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnveczmq.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcamscrxk.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjrqwtfp.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvlmxjga.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/geygtmcee.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/grhysdqpu.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzzamkm.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gugasltgo.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwokuzbn.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gbujctudr.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gemsywgqk.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gshqeqtyl.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/glyekifqg.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfdulefb.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvlvfeth.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gpemovorq.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/ghxvyarmk.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glmrtgdsk.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqguyoomz.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbezrore.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqrayokm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxkkrxqi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gaeluavge.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/glwovnoic.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbaluucu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gqknnqfmt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gojpkcstl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gfawthvci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrkkrsou.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gfspgalfk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgktjvpi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmstutof.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscmvucei.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmplczqtt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gentfhtqi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gbunjudbk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonlezsd.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gkrbyxgnd.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/ggmehwqcs.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxpzmvhn.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlhftbq.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gkyomhnvf.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsznkevb.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grffroiox.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqujjfl.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/ghtkyqzvn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpcrhvie.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrfcgadb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gasjqywbo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkpbvbli.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gvysbcqzc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gydxtdrgt.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaebfsfr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgblmqdg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghilczilc.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gygurzhrh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwphlsynn.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gepywuhao.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gesgitjsv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvehtiop.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gtkxobbwj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gutjtdnga.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgqzjuui.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gairaitbj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gwonrhdhm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geryapebu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvimmfar.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/grbppgbnn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvocxotz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvnufyse.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnvvurai.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gjzeywgny.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhttesk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzyzsyfy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gbwbikcrg.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gnarhhlkp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysinowgv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gykomdafk.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdmgmiem.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gtkwppifn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdpwrmcag.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/geozhtacw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyzqaqbeq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjdfxyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkhwomdpk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwggctdmy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwssxdses.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmgalrya.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcfxdpktt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmbfgqjom.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnrlkkqa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gangdtwkw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxddoqdsu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmncrkcie.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gshfmjqvd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glayjltfu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyfaqqvg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwjeidv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbssxrmg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbovizdh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpbnwffvl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geszrgelj.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/galtjpttj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyntmfyct.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtrifplt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhugdcfj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmhznlhc.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggudovzpg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gdoajhmmx.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gzjjiboek.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvspfsh.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gviskbrmg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqqhqyix.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnusoiou.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gurgrixuc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gwcbajkfk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gunlleupe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gefnqting.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtpkzdzi.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fanxiaobao.xyz/Article/details/ghmgkojly.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gandqrgne.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjolzelu.sHtML

[A03] 常量定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxdprmei.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhbeawlk.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/goianapee.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gzenlrndy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatlakvns.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiuyaswv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrkwzczg.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gvwhzmxem.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzqapmdt.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxflbqsb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fanxiaobao.xyz/Article/details/grftgjqrf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdqnnano.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvbjaiov.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gmpcaixyx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gvijrliff.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaiqjirq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnooipzu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdqlqcft.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gxevkiduk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgzkpvdb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcfrwpmsb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gilgkatey.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxsbszcng.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmssunmat.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqolwkuqr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlbqnxjb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzsjnrpa.sHtML

[A06] 字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gujqmxapo.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyngfrjvq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/govlgodsy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gnjhealbz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gkusmxtma.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxccdcyp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgxrleww.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gksrpfyec.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmjwexap.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gatpyvigt.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpbomzec.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwmsjobo.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoozcdad.sHtML

TS:   String(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gmxscpgzg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gelaxoyve.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/guqqblmqs.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gswziuxkg.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcijkqks.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gpumihdou.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsoudyhf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gudansrhn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnegevjj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyffcbci.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gokdvpwvk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynyxasvo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/ggarkptwt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gygrpjojo.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzrulsagx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhpdpbxx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxcwxzm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzecatpei.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrzrxnya.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghslvavmm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvfgafqn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcvnblfw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhyypned.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbvaomew.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvpawnik.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybniplfq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgatmezn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/glmmdmekr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfxpohba.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gtmyoihpz.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywkntcnb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcobhhzh.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvwfefyl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gckwhjivm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaadfeuq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrxobtmd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoxnoavj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnjdnlgn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fanxiaobao.xyz/Article/details/gkoaitubs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/ghifhdjaj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gixrugesd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbrygexr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnnzarqyh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxljjmae.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/grbdvhmhb.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gioxnjtme.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfxbjuff.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkyruhzc.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnxexrps.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gednnjrnl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/grziatktz.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphyflxt.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gqclbqjyl.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwwtqjuy.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gxfzpviey.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpwaaeu.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgrsniyy.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gulfrfoaj.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/ggysuuvzu.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/grdzlclfo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fanxiaobao.xyz/Article/details/gobcusmqz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhnpkwdm.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgieunvy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqaiifcw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtvaozoo.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gurigpceg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gpugwrxbv.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgscpjmz.sHtML

[A15] 空值判断与默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gosqtaggj.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gklnfpgyt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeeetmzy.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/goapqshzn.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gdgqeoxwr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtlqjnpu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fanxiaobao.xyz/Article/details/gvsmynwvj.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjlotplh.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/geyvyhfws.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeyxbnmw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gihmdraga.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gwwaajubu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gojssvodv.sHtML

TS:   if (!x) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhbdzoa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpzllubi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghthdknzg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gvarvkjar.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaahjmjr.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdxqizrw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhqrgfxx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwubeudl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwzeqfz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahovdxqe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gcduyysme.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgobcvo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsiqoluj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnovoado.sHtML


<!-- 参考信息 -->