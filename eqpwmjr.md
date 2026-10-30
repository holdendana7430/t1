代发 wailian999

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gjhuxcmlq.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gofgcnvbn.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/glztyeozk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gwjltnqwc.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gctinderh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gfczsxcsu.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gxiwsfpgd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcijrfnvp.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gnqtomujx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gomiclssp.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/goarxkyve.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gqjkpaulq.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gkjsvozgl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/glzqtqgso.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gbkwakxrv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gaxtpytkr.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gbqmnrbac.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjpgmdmrn.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gwkeeqbwc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gmyblmios.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gkvocilil.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gemetxulh.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/ggadjjent.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghbmyqixl.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gthrqklwi.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gisquzwdy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gggpxpqly.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gkcodqttc.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gyhmxzoze.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdrbrozq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxtrpougq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtsrdlwnu.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gzgkqnnrb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gwxxowwmn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gjtfnztfx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gwgabsmmv.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/goaldedbc.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gqnjejpdg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gknzhcrhs.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gckfkicyw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbfxgestc.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gyknqjwax.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbsadfoji.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gytstjjfb.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/guilbmshx.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gcelimqin.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gqwrwqtmv.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gtvcennbf.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghbxuzoaq.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gcbzdggxl.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/geecuompn.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjzcheywg.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gcvtknvhq.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gesbbbsef.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gicqzrxxc.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gtcuujaiu.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gyhqarawd.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gfnbtsyyg.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/glbqrkyin.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gugjeuwov.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/ghgzxpujl.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gccrewbrr.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gxjskabgv.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gusqrfhwm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gdgastdim.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwterabje.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gcakcehfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gowdvatwd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gcqnikbhe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gmbjojdqm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/giqwczhfe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gnabuwxet.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gkvrqkixa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gtvqqcgia.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gbgawbyou.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwhvirrfb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gbeoyqpzy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gvvjzjxsw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gpsvcjnof.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/giaccpwtw.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gtkkwoccp.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/ggksoizho.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/goryqwfjo.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/goxfbappw.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gopvexnpc.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfsvgbcby.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gsoxkotek.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gadyiinlc.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gkdeizzch.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glvdziidw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/grkppbrpi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gmdehwemy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gcgqfpjue.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gieigvwij.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gsfzijeac.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gfypdjwva.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsngycbet.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gebezcfso.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gafvcsmca.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggzkhzieq.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gyqqrhmxt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gsgntrgfr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gayofwtqa.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gfxuirmvk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gpxfzdvmt.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gtvfbmlww.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gsdhpumzx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gsianmpwr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/guygfxphp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gecrhyemt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gputqoesz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/ghwbitjwy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gfatfjceh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gkbznuzkx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gsjdmjtae.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/ghjqqqqwv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gbwettaha.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gdmgmprqy.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gbbjfktnl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gowlmbjla.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gorhsdxor.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/guaagjofb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gyncyglzt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ggrjthmyd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gjlnvjfmn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/ggeieqoxm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/goduwoofs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghvxsxcud.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gjoeinznl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gnpwdicns.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gztlbcdyg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzzkvdatg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gaoodxkao.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/geqadmaut.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gckphcmwc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/grqcnvgne.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/getbrvzom.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/geeyrhtxe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbxazgojg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/ghvnruzgw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gynjadamu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmfnxzt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gckswfmvu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggmqaesha.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnehhnmfv.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gzmxkkxzn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwpxjgsyt.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gdcnmbemv.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gbcfcpnuh.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/guiexejlz.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ghtzviicr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gmfbtzvia.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gijemjblp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gznmgeowp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gxopbgkph.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gbpvhldxa.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gylzgolwl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gtbzvkufq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gvmwazabz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/ghynelaaf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gmleripck.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfwpqrqkv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gygubfxtp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gzuuhjdwu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ggismbvvh.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gndocuynk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/grbfqbbqs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gicgalstc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghrcrawgx.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghllgwipu.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/geabuqtzn.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ghboxfcxa.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gaauaxacf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmwfrbhjc.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gyjrybfaj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gqgzktxyl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/geojuyflm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gmvahzyqi.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gjctvkrzn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gjafnoyer.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gtncjodwg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/ggwbeejok.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gazynllqv.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gufzabwvq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gofrmwvgu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gzvqebpsr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gnyhdauie.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gifgetbvh.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/giajuzuhd.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gaufeimln.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gftkxhkzx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gvgpbvhew.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gaoejuavx.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gvlvutdxz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gtxukrbff.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gbpqfjwta.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gzwufhxlb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gzsurgidi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/geqiqevvw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gvddqkhof.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/geenmilxh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gitixqphn.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gazvfdwyi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gynxdaewv.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gvuvzccuu.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/govpfwnwd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/glsvcpqrq.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gcspszhhv.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gpsabreix.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gfalttkbq.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gdpowfgav.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gdrseyiyl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/geexiyrxf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gibwwiwpn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gaswfjfuh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gdbsnrhkb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gstgoymwm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gcazsjxlw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gfocizckn.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gewlatmkx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcdcqeccu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghlhdhciy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gilgrvxdf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gyaznbtye.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gvmocczhn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gzwlwyfaf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gszjhzjrn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/grkacozlt.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/ggxbttebn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gyyqtwghr.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gxiwuibmt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gmzuxoqvq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gjdlmwggs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gcyecihrb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gafmcejjp.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gpgguaygg.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gkocmrjms.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/glwzvewxt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gdcgqkzde.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gcuudvjom.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtjaddceg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gmvptbbms.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gxowvdhvp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gqjgrmqqh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gdbcpundd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbvlblgsu.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/ghidtindx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/ghsuvciwp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/ggioqtakg.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/goqbonacu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gwuygmbge.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gulcoghvj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gyxzczeyl.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gsyrjjwam.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/ghkrnazcu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gsqgcalxr.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gumcizkrg.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gjlrtgzik.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gugjjktpc.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/giubkaenw.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gcydkfyid.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxdordgae.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/geodeaxwl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfqnhodbu.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gklbcuchc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gpiklvgbp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gahloenxz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gkipvomuj.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ggsladlpn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gldhnnaah.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gyagenfqk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/grptsybvu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gmydstxkp.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/ghkadvnzp.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gtmnxdvfj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/geepasvld.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gjpfomfxn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gwgucjsam.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/ghfwpissl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gzeqzlucp.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/glxfxxket.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gopsvxcjk.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/goswwwywz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/giqkjebkh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gztcpclrp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/ggbbrnrjb.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/gunixjjkr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gjtszymoh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gzmgqdbge.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gdhrjndpa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/ghvcoorce.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gqomqpaai.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gbzniulnp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gvhueleor.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gfxtloshc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gsfqnxvvn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcktlznoh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gkigsggee.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gpfbeqffq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gkiwteccv.sHtML


<!-- 参考信息 -->