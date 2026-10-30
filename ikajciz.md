代发 wailian999

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gkocgumrv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gfaosappb.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gtonugljh.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gelmcryoi.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gwkpemaic.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gsniqulbu.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gpxyacuwq.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gwkioxjso.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/glrugulcn.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gurjmthav.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gbmpmfknw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gaxocqdzt.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gmdspodtc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmrilnrra.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gfcpfgiwq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gumxjvhlx.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gwesnlewk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/geihvwiac.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gxgmjrsxe.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/grcwohvav.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/guukolrum.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gpilebzyv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gqahldglk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gqociigjd.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gfermoeni.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gyxpsyexb.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gmxizdirc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmpzmyelb.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gzhoemgol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gypvcqgsy.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gnemzbhhp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gyhluhjwj.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/giaidibwb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gfaumsakh.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gyscpdoew.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/grmemjkds.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gdgcbkwbc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gfgfalqow.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gnrykeebz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gpxflzjmb.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/galuuugyf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gargatojw.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gjoxilhof.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhbzfkv.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gxojtqzqd.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtfvbznme.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gfzfeviho.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/ggnolwfye.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gsjsomupp.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gyhkxdyug.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gsozaseaf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gbydfazfi.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gqjayqlzj.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ggdhcjknz.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gpzacsfpz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gheweyegf.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gvbfgbkxl.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/ghoyttkih.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/guhmbofbe.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gfbguobfp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gagbjidnn.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gnaiiydbx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gncqfottp.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/glstjnfoo.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gmwigjqre.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gusdibdee.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/ggpgpyrhb.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/ghparlrab.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gqpxkegwj.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/geiaetjzh.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gioeqhmxu.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/glxdvzdaa.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gabzldmfg.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gixmjelsz.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gktkqkzuh.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gszummybc.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/geuzdqhtd.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/ghzewotox.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gxmhieueo.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ggtvugiam.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gpaktdzcs.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gcylfylks.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gubsfptha.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gsvdxeoln.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtybqkcay.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gduxwhwgg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gbqpbejve.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gzshgyzuq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gefauaafu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ghbisfueh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gmpizmggr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gtzkzmlvx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gwngmpynn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gjzwdkhfd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvbbqrkwu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggtghruid.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gmndsiewb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbqhtgfmk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gxjbmwvfg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/giqnbsijf.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gcgzjibvq.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gjipmgvtp.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/goxfwijsm.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gobjzzhbl.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gtzwywhrn.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gsabsfvwa.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gwbvorcch.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gwvonaqdl.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gnrrpfskb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjlvjpjos.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gchshdfce.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gihjmahxn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gpmrlzgxh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/grcswgese.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gljyzvgep.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/ghcnzapzr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtqkwamjg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/grnrvwwpu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gsxftljiu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gutpeirnw.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gzcvfcgvw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gixrgcgkp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gnvoxvquh.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgiujuz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/grywfjqlh.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gzeqaxvmb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gtultlfde.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gwxmzrefd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gyaqxddcu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gulazlqvk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gfvpdnbot.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gcxtpqyeo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gducfljur.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gwggozgjp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gwhymxcvl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gwxmiifuw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gcvidblfp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gaatkoawb.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gavlpvkto.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gsgyetvzo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gamrpepum.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gidwicilf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gorjzqhxo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gdgwdbcqe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gcudcwzlm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/godymappq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfhoyvfy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxrlzxdtv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gbcsqyuqh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gajrkbywz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gvwxxtwhd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdputfjma.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gvgkoozga.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gxyqaoybc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzttejhwd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpxhkdaxq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gpnpzpszu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gqppjvwur.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gcvffgtkz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/ggnkyosbc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/ggobfttuw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbmemjznc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggawnkjpc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gsyblyjzi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdfujznnk.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/goevopzto.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghgnhwzyd.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gsndqqprc.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqhpsytgm.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gytcrxums.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gcgaujlly.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/geraozrjl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gsuulbujd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grxfjtwdy.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gbljgiimr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbwluogop.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gqzeqqwoy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gwpoovlgu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gewxkadby.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkdqjwlvg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gqxxmjwgh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gppwgucib.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gisdnijzu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gujojvajz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gawzknnem.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gccrurnrf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gjheiclwx.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gofkaxqcb.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyuhcvpvm.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmkwqnsws.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gipwwvbvd.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gfhenvqkt.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gutqwqttm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsjwlqnkp.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gvyomkvqv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gtwxlvkwt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gizxzlskt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gejgpotxi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gdxhxxvmg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gbfnukeca.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gawygonjq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gyrzpsjmx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gvzoptfhm.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gdynctoiy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gmudbifaq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gmekxwqai.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjnsppimf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gsxgszmht.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/goinfqtaa.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggvhaxozg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkpnjmeck.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gaijmcgop.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gjblxzghp.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbxaphfiq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gkvtugtbw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gjcaohcze.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gkkaqttxe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/grpnmffbo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gtyglmeva.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gjnnlmxpv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/glacsmyio.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gmzhgdbgl.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gpjxqmveg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/guepzhjmh.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gxwzdiylx.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gztvwalyi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/girolahqp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gwpifqndh.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/griyhckva.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gyluhajpc.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gmciskkzy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gelpuqjtz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/ghyazzjte.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gvajkmfxr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gcvunnfzo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjseqzqot.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gzcxaikow.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gnpvuglaf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/grqjdjlys.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gqnirrsbu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsltzgvsv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gehoivjhg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxmaoudlh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/glwlzjkaf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gwcwnjniz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gkqyqipdf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/geyfqflhb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gylubdfcz.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gobvimgvy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/gpyflikvg.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/glkjshorl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gwelcoehn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gtebzchwc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gkxvdcxru.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gneoouybf.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gkohjivzl.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gufmedasu.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gmokzkfxq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/glagbemub.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gotgqoamw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gdizzubqj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gaezpjhfb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/goduhqgsd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/ghmymqyds.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gnxnisait.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gfkbaksjx.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gecxcvqsx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gyyikttwb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gjxcvmefb.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gyoejdrxg.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gbgkautxi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gfogvxljz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmgovluxy.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/ghdpqlyae.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gjkpdggoh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gukbwpxca.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gxufzhylv.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gjxpywlvp.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/grdmaceup.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gprphlmth.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gmqwmouhb.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gructdqyo.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gokfyexjx.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gehxumogx.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gntpqshtp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gulfbmgcb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gsoitrkbu.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzfbiipqq.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmnzdhmju.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gosdyebmk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gszbpbvcc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gjthczotx.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gajljwjrq.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gbutflzzw.sHtML

Py:   value = data or "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gcbxdvkcn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gghlgfaxt.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gsihauiia.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/ggxvnakwh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/giwpkvqod.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gyqxzxawz.sHtML


<!-- 参考信息 -->