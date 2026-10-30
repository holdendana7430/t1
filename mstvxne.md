代发 wailian999

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gdmrgeaig.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gcnjamytb.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gooairdgx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gcrryqata.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/giubvetxy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmfnkybpr.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmypddgbx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/graqsaury.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gumlglzaq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gfxzktufz.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gyumfsrcd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gtetvuyfi.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gsrqwbmrk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gnelbqrqw.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gyjstxeck.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gobjemlrf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gwkfeecac.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gcycfjrik.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gsodmfijo.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggiejzgms.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gytblktue.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gybmtyjgl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gfcxfmnwd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gyfprmbak.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gukntfjuv.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gzlrqotko.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gfektubku.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gssfyrquj.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gjvqrqlav.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gllbqhoat.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gdxcyhbet.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gpndupwta.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gujizzkph.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/glnvbflyc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/girlmemrz.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gbqcaupxw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthwlicgg.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gncahoesk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gphqgvnia.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/ghawkzjko.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gklepraue.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/grcgpynrq.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gfggrntok.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gweiwjwzt.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gymompvib.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/goanbfejs.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gykqwkghf.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gjybuxjth.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gpabqfadn.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gkhpgmmry.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gopfhjlnh.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/ggttgrmef.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gjwsrzyvj.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gysgilcqr.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gzkdweyse.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gtnjvnliq.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/grhkscqey.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzrtmon.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gthhqyjxj.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gftoxjtla.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/ggfludaee.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gruxcqupx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gprdyvgsf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/glzgjuoue.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gecvwnnqk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/ghgumrxyg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gbeuaixxa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gzxjwtupj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmtwnlmgw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gwrnkcjwa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gwmmgtuap.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkkppsrab.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcmhpdand.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gekmtofzi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gukdxufka.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glffzvngu.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gadrakszw.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/grdbdzxxw.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gaiemqbpz.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gfcyxbpvw.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gdmncefni.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gysjbgnbh.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gjcmvvqvl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvicplqsr.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gmmjrsfpv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxtndnuuh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gzucuuxze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/glwmlqokl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gfkiivlub.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gbrwibfrf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gamaoqgcx.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gzvnytiig.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyfwkiaip.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gispavylm.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/ghnbgjrbg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzchdlekh.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gssgijjrc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/geafrwsai.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gfzffwqhq.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gihrztbjc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gzghhmjaj.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/ggesxilst.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gnbmnxvjc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gyxjbmvod.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gqzhjshrp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/giqvuctlu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gktwczatg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gqnabhvkv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/ggfuhufgd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gfnvbxtfe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gzifjaszv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gelkviruw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gbyrulrbl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gyfssawka.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/geglaukzk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gtxbqmkrg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gakmekrdu.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gidmmsuff.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnlhvxwzj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gggqivyau.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfkbyki.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnrnmjkoz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gbetngsfl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gbxdwidrq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gklrqverm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gdixfwxak.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gayiwgwjs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/giykdhsci.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gbapnctao.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/guetklsif.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwknoey.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gnnpqbdnl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/giirmdzgt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/grjzzzbej.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gkkusiobf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gadmfqwsu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gphbvdiav.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gutypwlym.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gwmrfsojw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gmedmcele.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtfjoortr.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/giuwzzorq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gayktizpm.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gbtptavid.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gipodfamk.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gwyibqzqy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/ggafhmljk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gcoaknmbs.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gfddohjqy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gdhnpfxfd.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gnmhuykij.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gwemnsdss.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkvzwgpus.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gxomriewa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gzxgzatxg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gcfkffqft.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/giutyrznm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/glytnciii.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/grhwjbdfy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gufrqesdr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/grswzqnva.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gzfaperac.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gkljrbjjg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gzycqavcc.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grgonhpwi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmoknuhmc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gaxvslspa.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gpvshxdjq.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gluicplkz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grkgsjsjk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gdzdokovu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gulynvikz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gqjedooxs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/grmvytusy.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gnmgcvdsl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gxrpsxvrj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gprtwqwsq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gfgxwjxwd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gbdhtvzoi.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gvstbvyis.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gywwshadu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gcfgiauqp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkusaciro.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqhjrarop.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glohmcxri.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqkpisgdk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggdokxpnk.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjueqctrg.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/garvuvxfp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gfmflxmzj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gjozbrkvm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gtqeaeqtr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gikiecahz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gvxhbxjas.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gkifeorzi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gcvlwgwdz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gkithuaez.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gxayiqplt.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gqlzmielw.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/guejzenzq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gqzuogimo.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gbawiairb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gpxxjiujy.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gpfvvntdw.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/ghjutnifo.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gqhbtuuik.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/germsotok.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gigtkdkak.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/goguymmpd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gicwvvpat.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gjenodkhy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/giugkrwyo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gfzypabdu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/ganoumjxe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gkdmvqdiw.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gzhfinwlp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gbzuvytte.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gafocachm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gtfuznqhk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gerlsqusa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gqvxyusht.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/ghnyfgxgr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gdmrycglw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gjiiihqfd.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gpriyfyue.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gjanaovyq.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gkawabsmw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gzxezsgml.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gytqcaymj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gywyucpbx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gctnvfsvn.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gluvmxtiq.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gpnighgkr.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gunsrzpjb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gexkqjbnf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gffgggadp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gjyfffefd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ghpwwykvh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gskisisdd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/glaubfcdg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gdizkznxn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gniizlvba.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gfmpjqqyx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gereautcp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gqrzzmtsk.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gsgxulhcq.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gsthswjie.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gptmnpgzn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gfnqowgcp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gjqcehtvw.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gmuefyagt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gpreagedg.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/giaphnqnc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnejyvjlu.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gqhedprew.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gindxceer.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gpyumcrus.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbhdpjaya.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gcldyyjqi.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gzyofmuif.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gogotybmw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gzsavtkvs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gyluspmqj.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gvjguceji.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/glssietmv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gkbeqojht.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gyaiiysin.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/goljgqitt.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gyfyrwzhd.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnyjugehp.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/glmvwgpeu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gquqzlspa.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/grqaumkvw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/githjjpqi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gzjeyguvb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gmrxkypnj.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gpznzkqqk.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gdvkeglwe.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gldziqwvq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gitxbbhui.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/grnowhqpa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gzryuvsuh.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gmjdohlrx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gtjcazxad.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gubwtphru.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gdwrfdlvw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/glsjfttmw.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gfrgbswmd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwfhmolev.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gfnuvxdvw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gvdawrimu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/grzdgoslf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ghnyhsmge.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxhicucfh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/ggstjxsyi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gptgdnyqr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/gxipnydfd.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/ggovtltfe.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gmjedfeww.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gohwoweih.sHtML


<!-- 参考信息 -->