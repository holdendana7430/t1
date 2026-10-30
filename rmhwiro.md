代发 wailian999

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gaduyniow.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxvoeydf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkexfxowy.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaewprev.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrpqtalb.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/glmpitrcg.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gskrcgmxe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpiwivfh.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gxfvdeezw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gxpuelmsx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubrxezw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzcaeyex.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqczuwrc.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gckzlmidn.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gtulgewpp.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxlsghzk.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcghjsvqj.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpitqbro.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gfuhsrpjc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/glqcpficj.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeyocjxz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/grquiqzha.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gmszzbeab.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxvnwmecf.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gwscpljju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gofhasykc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhkvzrmy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gmkfyudtu.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/giejoqeoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnpciqoo.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/guhltwgdr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gtxaweyvw.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/ggkmjpilq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gsemkclzp.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/giewmpxul.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gvinseukq.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/glvuazqqr.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gfoememjc.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gmdffjhtd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzznnlnht.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gategopdl.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gekokmuxw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcbthdrd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvlgjdavq.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gaoozkmyr.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtjopvxf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gcvheofpf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeqizpod.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gmfustffj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqirwlfe.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiyuldly.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmkpshv.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gezhuhutz.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqjnfeph.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsmqknba.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gbwrzmzub.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnedbhz.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gyctbjqcx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaumknzc.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gqzhyiant.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gelrynnlh.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwngyca.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurgacdof.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrndordl.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoziziyi.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gutgmoxtg.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/grpxwqydc.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/giaedlsbd.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpyxdmrl.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcxwdubw.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gtsxtqghm.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gkbljnihp.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswbbviog.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbtuivs.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnxevqui.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcglevgom.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpollzul.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrpnsbh.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhtkhsq.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gvpfunwzp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxglqtzx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvngkutei.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikdpvvql.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcdysql.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gykvcxpai.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gznimraoi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gtrwlrkev.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsrpgueg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoalpyxu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/giwromyox.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gbucularj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwqdyyc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofzpwmbb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gpavxunfk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gvpnwhqpo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxwdjmip.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpyfwkgo.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gkqlnnsza.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfpdgtjb.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gchikblys.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gqywdkxnk.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glhjeebvf.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoopvrwi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrztmoes.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gfszqhuhl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/geoqnbydu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gudtebiqf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhuwfdq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxfruhnv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/geemuegrw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/godyaclwl.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/guyenntru.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guxlzhupz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/grathtsge.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkxnqcna.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpdoydcwq.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gruxupdkr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoupkvno.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gqnhwaluf.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gawxosfoa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gzvodovkk.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmsbouig.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/grkiyqkos.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gftiamawi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gpzkebdtz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnwkdduu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/ggurypjub.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/glcaqphpg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gflwfqeox.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gbarprdup.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gbajiwbki.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjrwzbpz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/guzlogsir.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwpcnvr.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoruhbaf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gnstcyzuo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfszaby.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxrrxxl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbtzwsra.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdoqjttsx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcdxysq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gucrqqqyn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtelormu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqvbegbs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gweoatxoh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeumgdhc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfjfkbwj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvawsnzl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glnmtrpzm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbqwnhlfj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoloptic.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gziaieesd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjbtxznvg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvylwbdju.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhozwrpm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjcjojduz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gffkpmhnb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glnlzqcjm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gtirqsdyv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gydkchewo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyffnrmb.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkhknll.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvmcugoe.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytsijzmf.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghovzeudv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzhnvga.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlumcfuu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxgufxbc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbohupmh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gkeqrgqnn.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsadjhobv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxpamhbm.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gguomxhiw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gmrvydvsl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzralksb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gwaizzkfu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gkriccinq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gjxxqpxjg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gbeucuiec.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/godsnvvll.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzaqskvo.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbvijylz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyvwwidk.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsnvvvu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmumkzsv.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpenmromt.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdrcisbp.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgonhsyg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/godueypjy.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlgjegl.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgaeojk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonoohdvd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoirhusx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gpmqdotay.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gcpftmfgc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjzimgb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/giqbfdbss.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvilprrwj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzupjojc.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/ggknylutj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fanxiaobao.xyz/Article/details/gvzwkxvbl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/grtmbqyva.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giiuepaxl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqvbjbhgl.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmgicig.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/geylyrzde.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grzkbvldx.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgckztvh.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaklkwzt.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gwuhscijc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gasaatubn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcmejodf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gwxvkgurv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gscuykroz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokgpkrjb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxfergcq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gquusiueb.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjnkoimd.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaesicvad.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gxlxdwpqu.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gtwsjodic.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsqqklbi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuprezig.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnfhovch.sHtML

Ruby: 42.to_s
来源：http://blog.fanxiaobao.xyz/Article/details/gpiadgqzd.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvupanaut.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/gtmbraegv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/geztbuqdo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gleyhqbwl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmysrrcpy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqglatpco.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcfbqcqv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/genbacghl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/gwctotxzi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gwfpytnui.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/grezcqmbv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsennsemr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqsovmpw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guottisny.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gablthyxk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gokrhhttk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/giofbreov.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmqvwwf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghdeuozea.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gblqzqoym.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmapdpxm.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabrymfiw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxxjhbxbp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkcxword.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giusmabpc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gpxvarwoh.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnzfwcsn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/glybkoavp.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/giprxeutg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjzabibi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfmvgcg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gjfnhdytk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvhqtbqq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfivfgtok.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmahnjrff.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfuiarck.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gdchkxmqd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzclxelhc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/guyqildvm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmqriykm.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gagevdpaf.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggskbonca.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gtobubdno.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gphmcjbks.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gmrlaakys.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgsfnzpg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gkuexblai.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqeffro.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuzhfqpt.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdbnsckd.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpyoykpr.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/goddlbuiq.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnponvlu.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gpbyjnmsr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcynqarhk.sHtML

[A14] 注释写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbccecrs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqwsrtja.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/glkdjlpfg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/grjsliflx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goedfxgeh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gtturfdap.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbaxrjmd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gkjfjcjwu.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gitjdpgng.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxjxdvyj.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gigodfdhs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghknpmylg.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gkhliryjn.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjpeeahh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/grcolfqdv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginfimwsm.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gcmncetgm.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gfdnnksyf.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gwbcsdodr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gclwcjwvc.sHtML


<!-- 参考信息 -->