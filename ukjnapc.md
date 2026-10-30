代发 wailian999

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gwpitgnbt.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gckkburpi.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/goykcgwaz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gkuwwgaaa.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ggxupdoge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gijvjaoxt.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gfyfspdmy.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gsptojcch.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gvdwxddel.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gaupqxoce.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gdpcheimj.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gdukyrhow.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/glslqpjvj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gsgynpqyc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gydkgbibv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gcxoecxbz.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gxpamyrqv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gkzjuyulq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/guegkrnku.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gmqxzoxif.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gpbliqrfm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ghslgveeq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gklviyvrt.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gwhbbixvd.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gusmplcra.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gybecywlx.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gxsavurng.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gqecpvxec.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/godaxhvqp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gpsjhvttk.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gfodemoeq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnqwkiqhm.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gthjdpnkd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gabvwytnz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ghfxankmb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gajezwxii.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gnpbywifa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gsbdgnjfv.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gmatxoyga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/glpmmdqzz.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gmazmapkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/grdyuwxhx.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gndtlcejl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gdfxoggwg.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gtlaxgzde.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gxgavmplv.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gbvrnyhkf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpeojibzm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gcurirzkr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxxkvlxln.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gmhpkrzle.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdmdmwpgk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guizuilmu.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjyhhoatz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyxtxtlfr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gxjnjwgdb.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gilbqtbvn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gncrclwrn.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gybkbmhpz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gudihrddj.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gxwpwyvfn.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gftksgcrb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gvzrjnxxy.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gmaztwmqw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqoxcwmke.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gltqkojgg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmfkoqwtk.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gyqoikhaq.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gcrctbuqb.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gqepqceyb.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gggpeyplk.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/geuhrfgae.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/guzrcacsj.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gokdhnazg.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gysuoxmwq.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gddwketdm.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gdretajtd.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/guoantjqd.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gtqqryneu.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gvgmvkhwy.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/ghutfgepu.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gbsabsknt.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gnhsunmrh.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/ghcfzcmsx.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gbogwjody.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtvyjeekq.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gayhhdbyt.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gjybxolsx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gbxfqsiyr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gvfexgexn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ghcrwvnxv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gjeufgbxi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gxfhwdpxf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gfwijbyle.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gephbdazj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gzjgbjory.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gawhqqerw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gugiihdua.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grwfsnmtg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gqrkbyxoj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmrgatrqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbxpbordw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gifhzfryp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grkcmohyd.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/giffaedfm.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gxlppsaaw.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/genhzqxhy.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gsicnlgld.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/guiwpshcx.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gifajgzbh.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gqkqjgiax.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ggnyodiwo.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gorrapnob.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gygltkdls.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gdrsnwmdx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gypmowxae.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gfacmkwvw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gusfujghl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gljwloumf.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gqtyuerri.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtzwkozcn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/grmqbdrgq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gwvecfhcx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbiqfgxdn.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/giscgmzcp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gsklsasjr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gahiqvlag.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gfuqoihji.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gcesetexo.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gctlwcxlh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gnypehtkw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gmdblvdro.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gjqqqfuhj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gywlcepmo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gnnoxlsby.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gnmypadjf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gawkzvhzk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gicnprglw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gblnctsvn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/glrbapgje.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/ggmqfcvlu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gbyluyxyt.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gdnssfwki.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gyomftdsi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzhwcixzv.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gcqbswbhq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqseastzn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gjngfsfqc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/grrzjbhij.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gdvvbzyoi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gzxsbtvhl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/grmlyjzgc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gjajiuhbb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gcqnrcvzs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gbtljmdud.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghuhaliks.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gpkswbrix.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdwrkgxsj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gkfnkocis.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gpuzaepzh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdxpjalst.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gqdzephos.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkannbrpj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsmrfkybe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gsqiheoqk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gajebqtco.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gxhxughkt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gmdvwbaio.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gplpklowk.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gmesozcar.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gizmpykxp.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gxosnaqtu.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gazpqhace.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/geqylmshb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gefegtcwk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gkykspsyy.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gnfkedqwv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gsuumkkro.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gjkvcaxjm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gxbtubhgi.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gobawseuq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gorydnwcv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/geyickqxh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gqfstdxse.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gawfvobht.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gjybybywj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gyaoporln.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gnbaydcds.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbeiomvzt.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gyhsdndym.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gilqaojud.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gopjxenvk.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gorxxbhsw.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/govxuxxld.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjlhoccvh.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/grfbwkajn.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gsonbkpbg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggexeudug.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gxyuaskfr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gqxzfeyor.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/grtxnzjok.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gfcdpcbjs.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gbzdzpisl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gsocqimuh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gbhzwfnag.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gkgxwcpeo.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gbdfwncqd.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gvkxcepgb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gzzcbwbvt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gbgbafoui.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gddltnrzi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/grygipvus.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggkkscpfq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxpebtvsg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvyvzkcor.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gfaljwann.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gulwnbjih.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gbdcbrfzk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gdcehpwbr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gazcfaede.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxldpsb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gahyrobfj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gmiiijrrp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gnswitece.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gwoaxfxvw.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gkerllnbr.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gbyanxixr.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gpobwpznn.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gkhavgenw.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gamrtcgwp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/guyaopbqd.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gfruacdaf.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gxushclwr.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gfegmmtld.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gpeafcxwk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/galwjampq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gapjoywlz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gpbwlpqlo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gstjwsxri.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/goymhkoub.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gnfshmrpa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gzkvaqmpf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/glmhralwl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gspvuztwb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gnccnnazz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmiaxdxrc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqngqqmmf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/goyntecjx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvvtvfuue.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gqracngls.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gfbfdcecz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gkkvqxnux.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gyaoyilte.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gpylsjywi.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/ghnbupewe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gchfwmtlh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gshbmnbob.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gfpilavzj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/ghlzabhtw.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gdswmwroe.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gyunctkhf.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/glhffqoaz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gwmkphial.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gfrvaokdi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gmccbzjzw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxhymbivp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/glylncpem.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gezukqvgr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gqqwulwok.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/grjeklgxb.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gygvgjwgg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gbobwbnav.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gzzrsekhe.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gehfymtrq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/ghjswtces.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gkdqilwov.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gozxnvqqh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gcdrtlnnw.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gpdocgvgp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gxspqdoyb.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/goltahmri.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/godoepyqu.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqzuadwcl.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gxstucxlc.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gigyouccr.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqetagjiy.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gwwyqfspl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghpjecnzj.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gtyozhmhj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gdzjaljqn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gtjooaaxf.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gefcaoaom.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/grfwqdgvo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/golrmfijc.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gzbtghfvg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gnyvrkdps.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/ghgaqqdno.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/guyslfzhj.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gxzcldhlx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gtykyqshd.sHtML


<!-- 参考信息 -->