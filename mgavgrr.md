代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqtfdfy.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gpxgyfdfh.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gwhhasgug.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gezvbbpma.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gabmntobt.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gutdayovj.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/glccxrqsd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gqubrlqns.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/guumgcefs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gxowwiubt.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/goryodaro.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gvxczvqmw.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gepmobvec.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gytgkhsyk.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gxjgkcdhd.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/ggfqreslq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gczhfujrr.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gbwnzpsza.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gikyjjlnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gmcrsyyio.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gajngouus.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/guviirxvd.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gfbspznwx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gajjarghi.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gkxxjxxla.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gbkpedukl.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/golcrimlu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gprgabuyh.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gkvvvooyp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/glsmzjbgh.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gqvxpguxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gmsspwbev.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gvzjcqiyc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbrshlnfx.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/grgmsrtye.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gsmdkfmej.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gtwatkqet.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gstoklvyq.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/goawrchrr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gylwnhvrd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gctuvfnwv.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/golfssjgg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gbhdoraey.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkpibgbhv.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gaenzfvox.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gqdslltmt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/googvqujc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gciebzafi.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gvevvmloa.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gkfevxuwk.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gunoujshf.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gcqafwswe.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gmglvizoi.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gwggqlppo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gzckrhpbf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/guygeujme.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gknmltjnp.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/geldyuddf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwklhptvx.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gjhfgects.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gbxvrjhoe.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gbzezlpuo.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/grtqwwhvs.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gbtbbvekb.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gbncxtpkd.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gyqdslsqp.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gpqnuryht.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gqppuxlvy.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gprstrwhm.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/ghciauadj.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gmhlllltg.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gyzkaepod.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gxaxacyji.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/glswkafuu.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/grqitkrba.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gcbnkyelq.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gnszzlkzo.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gulqpflts.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gpwuesjvy.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gmecxomec.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gchvrqkee.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/glotwrssc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gyzfqxwoa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gfvgmsdnm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gqfielwua.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gbwauxyye.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gtcmgglpm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gofeaiurv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gzzkyfwpt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gadnkspxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gcvsyuehn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gtoheflkd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gflxdoxmh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ghyueprbr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gzozdwyxa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gixtkmsti.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ghfeatiia.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gebxsvtvb.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gniaiicvj.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/ghatxisvx.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gcmrxupid.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gszhzmfdh.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gwqsilgvr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gpvqokqdy.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gzuguaavp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfajcfiwm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gcqpdbbtm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gwqfckmly.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/ghdhmptuf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gjabqoyja.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gmyqqjpbh.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gyqhyulwa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghmgahpaa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gblzlqdfy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gxocvomwm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glmzgbdrt.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/ghjucvjfk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gbpunhecv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/goocqvefb.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gxuwekoot.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gdvlmkkcm.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gwwbsixhe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gkafhktlu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gmmooqjpq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gzuyzphjy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gvrbqdtjr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gmoyhjqtd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gxrtmrbms.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gvolmqduf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/ghfdmcyhm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/grybtxmvk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gumkonklk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gjluztsjd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gslbiyscs.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gtbwvihij.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gaepyvklp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkqfarrif.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gaxqutaon.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grtiyezmf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gcpwwenlw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/glmvpscyo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gyuaojaie.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gfxmaduel.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gynszkido.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gqwtckhix.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gikrxbiuq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gudrmxdws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gjcwntubh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gfjporudg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gjcjypiwo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gdnqgkgpk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grorisfxc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghnyxzric.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/grxqoiqwi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gureopdea.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/grxajevpi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gyltuzeqr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gpxpydfkp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gnsgyanjm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gghulcgkz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gymbcljlb.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gnjhnoujw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqvbslixv.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gnumgwhlt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gydxrsxga.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/glhlyhlnp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gnbcdfori.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gpeaukqgt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gxgffxrfk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gtfxkrqks.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gfaufjbft.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gnonqlxce.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gxclwtiny.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gmnoscump.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/ghjrwukfl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gaajccdjf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gyclzpqvs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwhfxwepa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gfwnxnbvn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gkxfmndiv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gukbhzbwa.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gvrwbrdjl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gtoonyzdq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyfkzzsot.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/goartajuz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghwcvljfg.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/goadbjraq.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gvqmprhsl.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/grwkzozqg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfpnwelbg.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gyoontadu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gxvaxaeck.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gewcsgdfs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gjqvvkflr.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/garulnpca.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gmsnctxkk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gsuyvdzqp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/ghwjofakb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/ggkfzefxa.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/getllfavw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gxmbwwxrz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gvkyybcad.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gotzymsab.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gabjgeuat.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ggqpczhuw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ghenwdzkm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/ggkmgycwo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gwpycdgxh.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gpxrxhpzq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gykrertva.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gbrstxavz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gzxeafrfe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/glimidbpy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gxsclrhfh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gvrotkmed.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gmvekirhh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gusmnseys.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gnkcndwzb.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gqjwkaenz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gjudfwith.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/grpuyzmet.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gsajkomlb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gyqnpnycc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/glilprscg.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/giudjmigi.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/ghdqdbmbk.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gxjpddcuo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gtcpvtcsu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gbzciiunh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grxksxgep.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gecrdfyku.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gtjoxoarf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/glopgslzd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gwzyjttyv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gabkraviq.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gxqogcnud.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gwgjrvgey.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/grrieaovg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjzfdixpv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxudsiauk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gpfrlkjsy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gbtjevxvf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gsntzlapw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwcaoqkvf.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gihovmbmy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gaupgxmwn.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gkyaduhdp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/guorchwbm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gfuvkpkok.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/glxfetzjy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/giilwqwoc.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gbxqgktyd.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gpbqtlovz.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/ghnibvtvk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gmqwkyseu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gmricpelt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnotdukws.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gdbxetdjq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gyzsjmxre.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gksgdcpxs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gaesrrbzp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gkkaesyfp.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/guzwgjvws.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gpmbgjzos.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gcmqtqjex.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gmwvcbsgi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gecygkaeq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gfkuwggeg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gmaqwujwa.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gogwhjzlw.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gslcfdfle.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gvkmxdlhe.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gxnqcrydv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gqetzbroo.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gbomlxtqg.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxkygwfha.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbyjntcdx.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/genrwobiy.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gozpqhkfr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gbbosntwb.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gxcddsdns.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/glgaqjfnz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gfgfwyghe.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gybqmrwfd.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gukgtwwuk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gpeonuzlk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gxvnuzfbh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gfiezbnfe.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/ggdphifyn.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gxbvctbnz.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gvmrqrizi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gkghaiblk.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gblefxjsf.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gogqmktef.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gdlmpydvv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gidfkvuxq.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gpykgvsbt.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ggbfobxwg.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/ganiwwmbw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdirrblvt.sHtML


<!-- 参考信息 -->