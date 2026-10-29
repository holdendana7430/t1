代发 wailian999

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/grruqgest.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gslascial.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gxmvvkhll.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gneepdadh.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gslqbtfqp.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gdhexlkkg.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gxkzbrajt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/ggkbablzu.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gsogrhfev.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gnqssoytx.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/geshucqrx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gkkwbcmzu.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gbrcxcnpg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gbwxwltro.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gtxynxpuw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gmusjuuqj.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gxxvkfdht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gvaocokzl.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/ghdsyzhaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gxuirfrrj.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gwoubqvzo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/govjxqcox.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gwpgenwal.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gabeubiwx.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gsamuruzi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/glqozguqi.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gzxevsyke.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gykmgiynw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gomaextbw.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyscuicjg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gtmyrexug.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpqwenocb.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gmqibbmyu.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gpbyljihu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/govhhmqbw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gijltpjxo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ghlupnuhm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gyyvhayea.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gsfrdvlfb.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxaxjkavt.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gplhqqrpg.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gravnkmpx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gtmnwtwij.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gcqroldda.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gagcdevuq.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gtvuqddfj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/genjkmdcm.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gmnsydsxb.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/grdcootqk.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gogcnjzru.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gdinhkekz.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyhtvpslt.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gqchgdkeg.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/ggvajutdv.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gjeoywqja.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gyihzdlbq.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gmhcstsfm.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/ghfgeejhu.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyjshtlhj.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gczrlvzfc.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ggrsjjhmt.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/glpgzobyx.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gdjethdth.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gfknjpugo.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gvlvpznjd.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gosbxmhgb.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gjolrlvxn.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gjwitqbni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/grzokscsl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gyfmlokov.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gwobxtewe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/golrjsmbd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gitovjawb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gopodfldd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/giefmhwzt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gbrxhzwal.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gadmuklni.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gyutwzrou.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ggvzgyuwf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/glujhcbsp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzvouhmze.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gvhjmdcjp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gppbqeivi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtxwjyjkx.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gwlvxmpdj.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gerdoltbv.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gencegilo.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/ggxzkdbsx.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/ggvlvtmjl.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gkqahuoly.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gjonvinjk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkcoohowv.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gtklcrlid.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gbcpscege.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gpqlonzac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gdgawrolm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gmtpvwsrg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gbqnzmixp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gglgzhenx.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gajwmmclh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfloxttma.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/glcrclnlc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gynlenqny.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gasbxzwpw.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gdcbddssr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gchofcruv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gkhqgpujg.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gamjufccp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gfpfrfcva.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/grqjtofqg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gijyhpeqe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gjvggxdwc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gecusmcvo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gfdhxqtag.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gkcgtmvhu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gdgffnvpq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/goekrtnpd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gihpbvfgc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gauvoorqp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gpgraxydc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gmjsdeywi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gntravokq.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/grvzrevgr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gcialknuk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gvmbaocdx.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/ghpepesyu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gavyvpzbe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gphnmbnvw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gmnquzpvf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gjanqyhib.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghavtblli.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gibbxpdpt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/guhwkokkk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gkynabxkv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gupyeztns.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gveharijt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gksavgzrh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gujingbkh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gknojxajd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxfoqrozm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxouhyztd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gvvorqvkt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcwcuxbhy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gswaapyko.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gngcqzmvy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/guuqzxris.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gowgtknhk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gikzixgnc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtuvpnqta.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gcukhcims.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grnfcuquq.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gwpmjkpnn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcsidlieh.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gfwavwjtw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/grmptcofb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gpbtfqols.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/glecjowez.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/ghjukxurm.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/geqlyccrw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/glngwukft.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gnvbafdup.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gkddfkwue.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gvignnwhk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gvgbzkdvb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/ghrfhnnuv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gbwvrwkkp.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gikvovtdc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gbftyrfgf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/goqjfvuaf.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gwnxdzubk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gzleskson.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbqoqdmol.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gihtmvtrh.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfenevivx.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gilehrdez.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gmuwevahn.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gsiytnqpo.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtphckgcb.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gqguchmks.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gbejsmidp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gnyyqpxzb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gqmegbuls.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gaplnyuqu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gzezuigzm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gzmjuqpwi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gsgjqxswu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gkbdrblmk.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gzmdzslnq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gjcvfbloo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grlxznlfh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gneroaayu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gaiqkqdii.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfwfirwzk.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjefkhsld.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwmcenphn.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gygfiaako.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gdmtibkjz.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/ghtnmdcrp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gabkubuol.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gscyfxkrm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gytnpelsv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gnohosszy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gtgmvrtdn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gfqlqhiwf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gbctdyzor.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqqhaudrg.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/grybqxkfn.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gqauyfjcs.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gecyezyxe.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gvuuhvyqb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gptzwftyp.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/ghkbomsyx.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gicmavzxr.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/guthcvpfe.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gvdgznipo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gbkhppwia.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/grxpdjgue.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gqxhuhhnk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gvvkeyqsw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/guldzcdgp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ggqkngzum.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/golitjjln.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gvjhdldzn.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gsaklwsfh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gleattbfn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjdujmecn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gxeyxthtu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghctqbptq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghpygphud.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gawmdfvch.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gbaftodrt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/ggooeastk.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gsquqnisf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gerhzerye.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/ggeanbzkd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/ginqcaega.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gyplntjbv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gxvwsigvg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gjsqsvicg.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gowqtsnbz.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gquhqjtcr.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gpumociza.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gajgeyour.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gezqfiqqm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gnyojmbja.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gqdxspvku.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gutshjbyq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gkdbktcen.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gerjokyde.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gbkfubwsv.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gfioocecn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gmqmyipzs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gsqynnmig.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gtivzvwnx.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gvuoyqfda.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gnjaekywo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxizorexs.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gskkoarea.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gisdqyytq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gvzhmkgar.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gauinygel.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gpnjkhaay.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gfnjwakan.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gothcyqso.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gcsyjaxec.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gshzxawax.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gjdyasfbu.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gecxqymke.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gfvkszltd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gxchbxzuf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/ggxsmmcsc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gthnewyfc.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/goeikvikg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gftofbfpj.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gatzyrmkv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gykogylhy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gjqyepvsy.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gtvejtuwz.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gtuqcrawu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gyjqlbtgw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gynatjlaz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gdjmcxulp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gdpsvrzxm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gshdkccqo.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gxqpnbpjo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gmiqxukdi.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gacraarvw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/ghvwmreoc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gtrgvktad.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gxproxhvm.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gujwzwbuk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gouzwucbk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gohrfbbco.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gtwrmbets.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/ggvxhhevb.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gojhetrca.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gpfqmakfw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gmakgdgib.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gjqxlaeiv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/ghwgkeewc.sHtML


<!-- 参考信息 -->