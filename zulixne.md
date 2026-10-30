代发 wailian999

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqefzhj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxykrouoe.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gzdcbhqyc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdlfqmuk.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gismoccnu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gglzzbnsv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcpbcggq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/grnqdwjhh.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gmkpeiple.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpymmrwzo.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guplbfjos.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsaumogh.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxzutuh.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/ggjnezzes.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrkwugka.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeapgxmo.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gggydiuwv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklszuxvg.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gjyhbzfom.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gazuqzggy.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gfnnsiaju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgaskdxb.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gknzvswcy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gfpsudomi.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gicoiycsv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gdlwctimy.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gicqxgwng.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfhnsqo.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gyvtygwcv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/glpvcykai.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gbfpyrppx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcytcaqt.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnnnpyuw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjmxyrr.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqowxkd.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjtxllg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/guwqmyvci.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjglttvv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gemkzbppm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmgpwxhv.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gnvxcagsi.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiniqhbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/groribzxi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtzzaxlu.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/glulmfijh.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfbydcal.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gghhmeymq.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gxhfmhunx.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gufjuciqw.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjmlfnes.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqltggwj.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gsqnnqrzy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glrcpduhi.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gewczewdm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxafamjq.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gsipwupai.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpsbahhv.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrmaywtu.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnouzqe.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gqsbrvvif.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govzfljpl.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gkhxudmqa.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczcieurh.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/germuaorw.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/ggofhclyf.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/ghpmnwetn.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gckpbloof.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gztlxjztp.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgoapuu.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gakywwdtb.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkefwuum.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbfzgsgdm.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gdmovytva.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnjwcorye.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupymrob.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gafgcklzd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gnopspqoy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gfggvzrql.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gygsgndlr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gpxdlrfom.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqmqtici.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzswovztc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/grfzckyll.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblcjjysb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/giddbnjpz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gfwevjmtf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gkroxrzlp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhqjjmij.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrlujbb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeyqerkz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkwnavcc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/glywfhchg.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gtdsqggec.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlubxbl.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gmromecar.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gzongnbjj.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgnjrbz.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabbztupk.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/giyvbqhci.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glunjeaty.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/glovryanf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpqfxjk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gunxvlttb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfcybzl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gjbjrcsuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasykkflw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gepeqirzc.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/ggntlilii.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjyptkyr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjxtkmc.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/goicqcsml.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwkctrxvb.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzhprzmc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gxotysubl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gvegnkwnj.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfltzycn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gswyffijd.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcuiiiah.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gimjnaenu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/guspezepb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkcamgrp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjbswro.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/grvjwtdjl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeasovpi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gmcuwiejh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqdtngli.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegbprgcm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdueorcmr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhfsjwa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/galbpbvvr.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvomafiw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gwtbecqym.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkihpitej.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuxvghlb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/giabtmqzb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdzodtjq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbvjromk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyijhtjd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyebznndi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnmnfbpku.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/giqqhtqlx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjxjwnwr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghgprqava.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvodlfdum.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtwyqlnd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpuowzee.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glsfkinew.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzrdelgnr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbwqcyipd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/giorofelv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxknzlvdc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/giqioveed.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gygznsahr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gobfhncrd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdlygfcu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwocigvn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvsaygamn.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/guasjnydi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwftebca.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxixnnmo.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaqtapjy.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gflvcyzaw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/glvijtepz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/grgptscmi.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gxzpvszes.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gysuhynlh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwoufgqh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpobnjxfk.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzicmkuwn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gbgblijdj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbbfrjpf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsebfmjf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxhfutsf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjloundq.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxbcalja.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkolszlnz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaegmnkc.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcykvuqu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fanxiaobao.xyz/Article/details/gneufvvpa.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwnytvsu.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlqplpag.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqlobgqu.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqahkfwt.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnstuadg.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlqxelfk.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ginkkcxtt.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbubmkgnr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjwziazt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gneblgylr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhwdrbuy.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/glshwsqlh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gejhcasev.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gmbtdwyly.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/guilyrosa.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrgrqcnw.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gefrkiydw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/gkqhqipbf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuzzpssl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/guvovsbql.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnucntoqc.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbdosqbj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnpqjbi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/guuvvlhhh.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvrulcy.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmovqryuq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpqyliep.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxgyhtz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gnztlanua.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdlabqeh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvbmwlcw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbntlhkqf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitzwjffq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/guvuenouj.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grxeujddr.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffibgzng.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzfreksk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznujzpex.sHtML

TS:   String(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhiznja.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gscofroor.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/ghljrdapu.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/gixovmzfn.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxyykibk.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gugdzhobp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhggjxi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/glzvzuvab.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/guvbmprhh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohloeej.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gllhdjofs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlhvnfcf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwsuvze.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizcpgpxj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnifkfoy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glnolqqsb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgrxzevz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfeesff.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiludyvy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gipmzqkbb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gapavfypa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gyjfawtyp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphdkrfy.sHtML

[A10] 生成随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimxzuex.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjhorcrj.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fanxiaobao.xyz/Article/details/gerpsqamq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmolesp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkouklsut.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxhntdxbg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/geedpqjee.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gnprbshju.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbnbwrzx.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gnrcrfkki.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fanxiaobao.xyz/Article/details/guyakmhdc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gcspuypga.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/ggfxewiag.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwxnslja.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqocaxoi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gtlenohzc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuityorr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gghibmyzg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsowyuzn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsjygaoym.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fanxiaobao.xyz/Article/details/gljlfeabl.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/grduhzpla.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gtjhymcin.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/gsswwlhur.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjlimorb.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gmbqfwobw.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsslimihe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/gckcjnowa.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gsdwonvin.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuqhzjrs.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gaumfuvuo.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gdukpdpii.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdskcxyov.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gtpeefizw.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpnbgvcj.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiiwrwjb.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdlnqwuf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuohxsgn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gsjhaawoo.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtfsoeef.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjoqpdrv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/glfxykpzk.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gczsqxavj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gtzmlbvvw.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gtktywdlh.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcrxetxp.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqoyapes.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/glnufhyjo.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzbcfkc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpahfjodb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcfylmlx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxworzuq.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfgjjgth.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gtglhdxej.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gewstbsvb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gluekcwez.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojcsgfr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdgfxlzf.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gitkilvcn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqueuscv.sHtML


<!-- 参考信息 -->