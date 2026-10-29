代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdjzfyqja.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gnodbzvkc.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gbcxkvrsg.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggfkvjgeg.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gvxumjzip.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gnsrzztll.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gjbgwiwwf.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gnulrarcu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gjepxnfnd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gjrazxvjq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gtiyxcclv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gsiscdycz.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gfgxaqrcv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gldqaldox.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gymirmmoj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gtatgmuzx.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gjfecsbne.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gtppwpshq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gbyjtevaz.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/ggldiehpy.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gpxctrltp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gzgyfiyht.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gxnywmtwz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gcvzltwto.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gfqupugdu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgmbpqq.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gdhvhftsu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gymnxizwb.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gpiabrwmo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gsnwfkern.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gkolgkdke.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gjwfgwnbx.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/ganualhuf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/guvkpintd.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gpdamwmwv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gbtgcurdr.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gmgehtwon.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gzsnwpnil.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/glejygzgc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/guapfkvun.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gugnnunbw.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gkglmrybh.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gjifnvmuo.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/guhvewtnf.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gwlxsxrsd.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvrufpukk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gpocazxuu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmohtcipb.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/goyjknbje.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqhpkegdc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gihsbsvnz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gpfzcpqnv.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbffaqrej.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/ghteiahfx.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/guwsxxdxn.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/guzrnpwyk.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/goypjahdu.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gduoznvoi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/ggatobqiz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gjvudmfip.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzikwgrdv.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/ghkuvcnyj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnxtcbsfn.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gcpceszit.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gyacylctd.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gcmhbuazn.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gthwnmseg.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/grctfmdlq.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/grruxjszy.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gmybgghhm.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gnvyghkgt.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gvwqeozux.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/goedfmnoh.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gyrgcprba.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gqoohziuc.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gtgbddxiz.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gyvrdstvv.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/globzvchp.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gqnesouxw.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gcwpmhcto.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gvfwmtvzs.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghvdmpxjl.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gywteodyf.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gssaxhgym.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gcbsbqczp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyaflrigk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbkgeuxlv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/giedbrhhb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/glempcljx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gupronlgf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/glnhzkacn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gpktmefam.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/govhfxtsb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gxyzcajco.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnnecjcwl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guzvvhdzd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwfizgbdx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gwlflrbkp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/grddxfzxk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwmwwheap.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gminqaixm.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gtynfvntr.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/ggrdhbhph.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gwhtfrnee.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gxogdxqdh.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gnwhlbuld.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gxxfimrdg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqdqighsb.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gqntdailz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/giaxndyks.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gyunbjnud.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gqvmjevbv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gefsvtzut.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gsoioyfmp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/ganoamwpq.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gqzjwuphx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gouejewod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gllbyddwa.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gfhzhujqw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzwmubmbz.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/ghadjvalw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gzphgkoly.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gsaglrgsu.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/glcyrqtkg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gegnyqsda.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gbjyxlrhl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gcbkceqjh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/glywcythq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gkdaxjsnq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gjgymegzs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gnxyfwhvd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gjtdxckch.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gwvszrmlt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gmocqfxnb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/geidoless.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gglnqodri.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gkytirwoh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gkycgmsql.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/glwhrculk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/geblmiflk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gotkusaov.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gvhshygca.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gjrcsplko.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/ghjkilvbk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gejsybowe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gimcpdfgb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gvjpkjgta.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gezggwezq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gkmcrwkhs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gbvpejaik.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkautzwpl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdlkoifqt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ggqdkdmll.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmtnabenk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gollaisza.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gjcovdedh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gyyhifxkw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmqtezfst.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/glvelbnte.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gxybeasib.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gisxnojzg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gjygwjsem.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxinjosxp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gzzflfacm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtozshqxx.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gprusqyft.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goarrddgu.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gkwgzcxiw.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gqeuvkehu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gkbluxggu.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gnpvklfwg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gzxefjktt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gnydcgwac.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/giridwmdg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gatqekafb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gavldhtgb.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gwnzmtqst.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gtublvvnn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gvlvtyles.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/giliekpzv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gtgcgsqvh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gnqwktnab.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gdpndmspg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gzllrmepq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gvaqkpfew.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/ghhejzdem.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gbylehssh.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/garkbaipx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/govzcrbqa.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gogzdzfmp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gofribdym.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ggeftnsar.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gbwtkimff.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gebfclekp.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghiqfsrkn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gpzhsbpqx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gcuhjiygu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gtrffeois.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gpkjihnms.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gazzcoyit.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gtbkxtpgu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gxfemjtut.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gfseoinsr.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gypeagsog.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gaabibaph.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmmpxjigp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwjbyhssr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gzwgcqmzk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcualylwb.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gjesxvnek.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gtbbqxtaw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtoqzwxrp.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grrcmcjjn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/grpwqeeji.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gwfyfmsyi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/glmeayqps.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gaxsrxklj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gpautkqxo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gnmsncfpn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gpnmhchwm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gmcxskmjc.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gdosyzmam.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gkllyknmn.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gniumkscm.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gjgbhxcst.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gurqvcboq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gnmavtbcz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gonkpulag.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gsnklowsl.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gglmilwph.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gwwtyklen.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gxgkrmnfa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gqkmrxjev.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gmrjggniy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gennlywdi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqnrmqgux.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gslhqbuxl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/guvszjpsr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/givqgbsnc.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gyurdnkae.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghtlglvgr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdgfzhwgu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gokwzvvun.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gqalfybuf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtaruvrop.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/ghdbfamun.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gvmvehdzg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gkwmhqhgw.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gzmbijqgm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/githuzkxo.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gdtpnwbgb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/goemhcpvc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/ghhfkzxgi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gjhrtybhe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gndqkptme.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gycunrkxs.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/guslgqgak.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gscxxhxui.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/geiqxwjlt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gfrijgupo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gmeoqfhnt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/geskheawz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gnydgoupr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gfyfbjuzz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gnasysyvd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gohzjddsm.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/glejpyyuw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gjduhsxpp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gdjpfxopo.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/ghujlejot.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/giyujagff.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gvajsmxwz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gsovmljza.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gdqraffjq.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gsixouinc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gyqeiesbn.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gxcpoqzwy.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/giaekrfew.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gfuqlhsgb.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmyrrsiha.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gwkbzqwrn.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmycfbcbn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/goknfiugg.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gzurnxzdn.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gqnonovkx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/grkeylnfm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gpfvuewmj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gzwtznszs.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gbpyzdviw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gmrpoxium.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gpesaasko.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/ggwfepylj.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gobbzojlw.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/gixkuqarm.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gkgsidrtd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gbkaquxzq.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gosnzjghe.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gbisikxli.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/ghnfmqxhl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/gbjbborvr.sHtML


<!-- 参考信息 -->