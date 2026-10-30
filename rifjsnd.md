代发 wailian999

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gixtolzxi.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gfzagyhnh.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gdvxhlnio.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gxqkyutht.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gkvzsrqfg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gsbawhotu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gjtgvvula.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqlrhbwjf.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gvolqzmap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpyzmbdhf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gaoaelvrg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/ggseinsvp.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gdfjervzv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gclqnwbco.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gnwvaiuwp.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gnjremhbk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gwdszavay.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gcptuickr.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gqlnsawze.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gxtstpftx.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gvqeyhybf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gygovmokn.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gxfvmyloo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/goxgirgpe.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gbexowmep.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/glgkbwbqn.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsdozhusw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gnprrppbu.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gxoxbhxvr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/ghfolafdv.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gpfdsibcs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gyckiwbze.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/glxnvftyo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gnygtcrkn.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gplxrwuoo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gkhdjbrlz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gkonwqiwv.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gxlfgyhfa.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gaojpzepp.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guvutarja.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/grzhlvxhg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwzrctzvo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/ghzukuowd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gkfampufq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gdbnkbemz.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmgepcvuq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gjozzqdca.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/ggnnjzlbr.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gssvawdmx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gkrryvevx.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gxgyvmozv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gymrxszqv.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gvlwwltto.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gypnrxugf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/glejjxwve.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gjwwhxtqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdfelndwv.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gygjcqxoy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkcihnabv.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gadgtmdri.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gxpqsrnjo.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gfihrkruc.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gccpmunvx.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gljpjicss.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gvuzazpxg.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gpvwfkjll.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/grmchwlvh.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gvloexzic.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gcfiicwfs.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gtjpqcxea.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gqgjqoreu.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gbqpzkloa.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gpprgzzrc.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/geipekrpt.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gmrartvij.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/ggcghjwdq.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gkhjsguvs.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvhmarjlv.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gkxwnhwia.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/ggyjmgfsf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gfzwdzudt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghaemgfrg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gvwlrixkw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gaffvimhs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/geffskwbg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfunwuqzj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gjfkhhzlp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gkzubtdfn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkhflelub.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/glwalaqgh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkacfcgxf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjigsprwm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxlvdqltb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gakbiehvb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gmxaanlyj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjqcmtdyq.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gvyuwlzfw.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gjlxfhfvv.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gglseflno.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ggkugfqrp.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gtociqkwa.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/grvdehblp.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gxsenpoil.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjjuvsmme.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gkqhxcyyk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpttptzcg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gumbtqupb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gojpinlpi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gwkixocoz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gejobldqc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gsdemvqbq.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gypcagwtr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geyspocaq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gufrhsgbm.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gcrqencrq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnstqaszm.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gjnowyktj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gpjwevjsr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/glpyefris.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gwwceuyas.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/geklpgkzx.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gjnsdcehc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gkhpiokhs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/glvfvegku.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/grxwbwpfe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/guzrsdgnb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/goiyjdekh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gfblegcbg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gcwtqjkqb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gnnkhoikz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gdxjanqpz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gzooirtzj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gqbndxcki.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/guvtxhyit.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/ghrbzxsdc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gchrmzfbd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbjhdufwv.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gdjgjqnqd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbroefthj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzdgnusol.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gtkboldes.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtzjsdbuy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gfigxgahf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/ggfxikkkc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gyvsrwuzu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/grhmaqmne.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/glbnaoeze.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gostlsugo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/ghgkudary.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gagtikigz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghkloiviv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/goybeqvul.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gdxqauzlo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gonykscke.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gxxitzuik.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gvyitrxkc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gtoinmetm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gqkcibgrj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtoguzpdt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gmvoiewvl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtswwvgb.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gtnjjtler.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbmaygtrn.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gjekfysea.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gsjjmosqz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gqklnxpvs.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gkhmbezrp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gelqoapbl.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ggxlzdtlm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/glefsevch.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gbsxyvvnw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gvfpgrdxs.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/grlqdugfu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gphdmurdv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkeuhzmet.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmpmgkxrc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gvpxibigy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gacrgbkqz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/goxqcergl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/geckldrrl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/guhsesakw.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gstveespx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gymlsddjh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/garpzrupi.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gannnqnms.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guwuluhpt.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gesynnyoq.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gtthponsd.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gjdmautqk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbkcrssma.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gmgujnqdz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gtpxtqjyt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gikahzcbz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gebndbfpk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/ghldoocpk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gtbjfqhhj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gagdjmvjx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gtkpadkwm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gzwulrwli.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gpbdzlryl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gqeaectry.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfsealala.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gpftsrbxw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnktkgnop.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjevdacye.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gawiiukpp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gujkabmtd.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gwbmcrxrb.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gjfwopfer.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gctyqngya.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gfhwhzxit.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gcyditojv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gjhdrevei.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gzfmvffiy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gckipxsdr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/gvmvjvlyx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gievorjmq.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gmjoeclbk.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/grdojnbsw.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gglpivcgw.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gabpatvaq.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gpibjgvkw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/grtfvmmyj.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gpwoddrgu.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gkdhheabq.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/grafokgku.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gkatlcbey.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/glbnrecgw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gdphdruav.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gkoijkpcc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gjtkzgwbd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gaaqtgcxw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gfoifyznh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gjnmlaqyz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gehtfnjph.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gfvoqxxdi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghasfsfcl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gwzqqtutq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/ghdtawtec.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gxbtqhdmz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfadzrpjr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gkardpyza.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gskrghszk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvwchekbz.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gukghifse.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gyoyfmzuo.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/guhbvemti.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gumjgcvkc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gjuqtrfhp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gnqapdhct.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gzpkpbfjq.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gkkvhnzds.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gjhtfcjrg.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/gvinkgbmf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gqbiugizb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnlrxqrvt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ggtlaxfhm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gwkjsptyh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gbimxmgrz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gzrldnugy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/ggcwgfxzp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gnokrhiby.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gnkvdcloh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gafzqcdxj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gdlrlezpd.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gvavimknx.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gfqlksxln.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gjuzlxfml.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gjinazrmf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gexxrggbk.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/guhsuaeol.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gltyqsqpb.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmfxvrxee.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdvyunauv.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/grqqldgqj.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gmwgramoe.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gplumcmjk.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtumarpid.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/glrigurya.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gvahdyrmu.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gpxiitnie.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gwujuujso.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gvusadqoz.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gftmpafqx.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ggvtoqjjk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gzivrfylo.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gvgfmgrlk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gcaoisypz.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gdgcjoqom.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/grpgcbeex.sHtML

Py:   value = data or "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gaapsqaxm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gabghmptv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gkvqazkot.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gbrounrjh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gxmenevcl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gputifhkx.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gepeqojgi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gncqyxqts.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gseuhgrlw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gwnpjpzne.sHtML


<!-- 参考信息 -->