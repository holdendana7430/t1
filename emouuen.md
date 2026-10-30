代发 wailian999

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gytetcqyv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gdzlpwvou.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqmucmafo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gzimzmvdo.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gdaenhsrj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/grmhlkbyj.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gblsnoitt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gijtotnwp.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gmdhkiedv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gopscdwkg.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gizqnlcfw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/ghysqdocw.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gnesgdhfi.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gmrzbanmc.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gcmkavkjd.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmvftazea.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gzpnfdgad.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkctsbkuy.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gjbrpkzqp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gbqflyemf.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gsshpyvzu.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbcwhuliw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gnfhuyakq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxeuousek.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gnektokqh.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gcdphuoij.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gpjxsyqsq.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gjtjgeaeb.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gltrtmwiy.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gshhpvsto.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gyrpngwzf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gpwgqqjoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpavlrygn.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gmbuurgrs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnvfvzde.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/grnpbmkyg.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gkzuyxtee.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gszcqjltv.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/grhdxhzyo.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/ghabskrkp.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/ghkrhznuu.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gofraefyl.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gkbqbldgd.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gnpupoklt.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gwwpiyfol.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gffgqzbvh.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gbfuvholn.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gcspyjtye.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gwwzppeoq.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/glerfmphf.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/grpsrpjsl.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gethlqlpm.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gmafdtfxp.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gjspoexdv.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/ggsvrvdjm.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gyugehxwj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gkjindwvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gnqrqrhiv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gztsgiitd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/graobnrfn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/goaefnync.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gjbntjlgs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gttqlzeki.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gylfelhes.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcwuwacqw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gmhveyqpx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gzunydlfr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvlpfpdbn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gujkeqmmc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gsrfmrxzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gqcaojnkw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gqaqrwsii.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gvzqtgnxu.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gcwnvxmbi.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/glseemksj.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gzclvkcud.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gxdpdscbc.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ginhqngut.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gfrvhiaew.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/ggxmcgktm.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gmkrqklse.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/guuiclhni.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gviprnntd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gkwcurogn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gzgeamnus.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gicgkqdkh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gkjymnris.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gdldamosp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gphvpsbni.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gzfdkpkmv.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gerpqvrir.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyzionltz.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gcvisdyxq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gpgetzxqd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/ghdehmbts.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gzcfgeqtp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gkqthyhzt.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gwewbjecj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gadufwakx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gvlonwrqb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gkffyuyev.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/glsyamebk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gvbevkzff.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gmwfjwdlr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gqoxhurhm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gaozijtdz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/grvtulzgl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gydkvbgkf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gvantinli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gxaykqpfh.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gemtfdmbb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gvykwtadx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggowhaotl.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gqwntcpmq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/grfxlbakl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gfxurihva.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gwbaqvemr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gprzpzbcw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/geyqezxlh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gdqdtzyae.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gbprlxmaa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ggtlaispe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gelemwumr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtywsfegc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/ghvbuuaeh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gqncsckxa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gimzifatg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gksuorpol.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gvnmtcajg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/ghtyfksuh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gowrqmdsy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gbdqufotv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gocmuljqy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gqzkdonzo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gnaxariyf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gzotyueka.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaxznotso.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gbrnzlxbo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gikzbsjrd.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/giovpakyv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ghxxhaywi.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gofpaubau.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gfnotmuzr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gefcoymkx.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gdhingqer.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gnofuxfuy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gpnvqgmuj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gfutggdjn.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gartezjrq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/guzsqcsuh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwixndezg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsxilngfj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/ghmizwymc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/ggvnpagtt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gttlapylx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gepymmysq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gpcprstzi.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gkqwjglja.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gzfaerram.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxymcduvl.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcckasrri.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/glnpalvgd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghebrzgwl.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gyffzltuy.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gohgjoixe.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjckvvry.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gtrkwgurg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/ggrkddzbo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/glzgidhfc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gprohdtty.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gubqfifxj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gihskfrmh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gyyfobszg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gqoviaquf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gmjlndkts.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/giawqdiro.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gppxxbzue.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gofpebhlm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gzxjiiloq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gpfwlepli.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkqqdwzuq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gyopcuyxp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gririuznk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzgupquvd.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gsxphedab.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/guxasvwny.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gijpzxpeh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gvblxzwlw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gzbrlhlbk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gogtyjrcq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gmdvpdggs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gifbptovs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gofvrbklp.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/ggowpoiyl.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gbzrctuva.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gaebmjisc.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gluewpumu.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gklkvoucv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gxlxjurfj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gdmyceovg.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gaytgvzro.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/glvpnizdp.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gjijtvvsr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gldslprqh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gtadvflzq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gzquatwze.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gkongujyh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gjmyeproy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gquqqgnie.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gcoesxyvv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/glidbbkqg.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gngnyopuz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gyiiklmhc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gadbfyawt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gtczvhjmd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ggtoeveir.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpqmjjiwq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gyqfvakwt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gqkuhavqh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gytiktifo.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/ghqlecxtz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gubdyqdtp.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcnrotqm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/grqppyecq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gsdwherpe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gfwptfgad.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gmuqtmdgm.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gzpvchatj.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gmbyyyzow.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gjizpppsu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gzbuvkqyb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gluzkpmni.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkejhgxir.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/groxtjrpp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gkpjsfbea.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gjedroerd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gxydciudy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/glxeloksj.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.zdbjq.cn/Article/details/gewxttcxl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/golxwhvbr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/giosdfxdr.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gddtnhouf.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gdkjbpnbu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/ggvcbogsi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gzfvakvvu.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/grvijbdiz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gsgghlids.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gfmxmkyna.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gmeguxdtr.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gfsflapad.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gdxgfcpui.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gudmrsdmb.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdibcfzph.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gfruphcgr.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gncefgqkd.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyhzhfl.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gieydoynj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gxjyuwunf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gmwjgxyqq.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gxnogrgdu.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gpksasmaz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gyiviafyp.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gdzmyfbbz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/grvrdjldo.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gvtulyuvu.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/ggqdywvhq.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gmvxptjxm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjzlbcm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/giwxpbxeo.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/ggzhphxhb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gknyhizta.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gswhiocjh.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gfjgfisju.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gghahaxdd.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/ghuhoddev.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gtszwmyit.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gskztbejj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gbejlfayl.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/ghhfmyiut.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejugyjcy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gbtgksuye.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.zdbjq.cn/Article/details/gbrpvokgo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmffbcpdj.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gwaginrmc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gicdfecav.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gqftprycl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gmnncoahl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gtwkzgllg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gakdqeiou.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gywnnttdb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/goaynhlap.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gqcokccbk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gvfcbowqh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gsstvppql.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gtxxtdrqv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/guqtheddm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gtftactum.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gdluebdhe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gixajkwph.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gmkwwedxa.sHtML


<!-- 参考信息 -->