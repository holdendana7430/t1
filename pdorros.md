代发 wailian999

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/ghcrdrawb.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/ganobphws.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gimrhpqoa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzhchmvsi.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/ghahrjrzm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gdqabblsm.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/ghxyjrzkq.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtutkqqca.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gssovjmyo.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gzdjyambl.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gvxuhkuwm.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gyolfzdcb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gznwtiipn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gsdsiexfv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/guqnvmgpy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gabrpwsul.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gmcoqkjeq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gldrbeuse.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbnkybjdj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gbwobehfr.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gpdszlokb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gtybvbcih.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/goeunhrfc.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/ggocrxqmc.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/grwfblall.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/geststsvk.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gfvxbetnv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ggbdpkpzm.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gprvtgspe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gwfmiifvx.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gdbgmspqs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gohzieogw.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gbboaxzcg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/ghwkjslrw.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/ghkzjqvmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/ghcqfmcmk.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gmqetslol.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gucnjbnkr.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gpnzhhhdo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gtjgqmpmh.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gdpxmhqpl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gousdjjlq.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gfneyilye.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gaanjzzvd.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gzepsfjdi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gldewjdjp.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gkjlcomlc.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxhnseruw.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/guofqemnf.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpkgtwddq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gbxnbmhjm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gvrgwjscb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gypoahico.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gdxbcziiz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/grzmvmnhz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gyspmivsu.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gklhzgaro.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gghbksbkg.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gctuaosgp.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdegcdw.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gtxgliteo.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gtftwxfbs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/ganjttvrr.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gqhintlda.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqpyhqytt.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/ggvfumevg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemrrmumk.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gwycwrctl.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gymyaoccp.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gybemxnch.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gxfgyutnq.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gjlrdswlx.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gkqvyakej.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gvkshdsxt.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gesshztkz.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gmqjydunu.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gdvzqzmlp.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmlrktu.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gtevtkast.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gasvawgzg.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gblzpowfp.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gbiffmezx.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/geqiypfts.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gszppzivg.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/geeruarpn.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ggydnylhl.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gyrpwcrxd.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gghukukbk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ggwhfoxag.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gamstplby.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvvkfvtlm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gqbvlconz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/ghvxwnqbg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gvuzqgqrb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gybbntgwh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gdkytdjjq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxwjcbfbs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/guhkxpkdk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzjzgrytq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gzhvhwukw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gscfidxdy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gbzfvpqqy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gmwxissrs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/grndrqujz.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gfkbjfgjb.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/grsxvnhix.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/goqucwdjz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gogvbpbgw.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gsudftygy.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gferjjqro.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/ghiwtnjwp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzfguwuav.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gfhtsytfs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gumhzwody.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gcqndnqax.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gqyektika.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gyzvctfmd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/ghgsipqmh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/grcpufzyz.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gifsonovo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmsmsmzfm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gdndxsoik.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gfiqusceg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtcnjzeej.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/guibeuhwj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gwgfxydzk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gatancysb.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gxeelkbcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/guzftxamj.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gzobxyitj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/ggeixjtzl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/giqsaivsb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gbkkrazkz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gaccdidtr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gvsrbchcc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gfvfnaben.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gitbovnmt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gfrozetkj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/grwxnifiz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gwyznyuuo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gogeqfdmr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gvlsbgytr.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gdpvazftv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/ggofdfczh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtypxvkoz.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/ghpfylsuj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gawmqzuci.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ghaxvqzah.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gdcyoxhgx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ghbsyfcjm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gslklmbxo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gxwtzqxyg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gkpigxawp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gjhbdpywh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/ghbdgsfey.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdutwfatu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gnpicdufb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gwdxtcrid.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gegweojib.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gbaococqm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/ggtsmqgbm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gzzyjnpxb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grsvfuqsx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gltbtvkdg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gozfhvbbu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gsdnkxsid.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gxptffwtc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gwldmklua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glvbbiqaa.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gdxcmosns.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfyxymtms.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gpcjaqwsh.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gsogdexvq.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gaqgkpqot.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gfackiedy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gfafpeqyk.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gpxdfcaay.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxagpnnq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gvmowpgqn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gypypdimy.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gcakefthk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gmbmjkxsd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gpuiesfxy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gclbpdsdh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gjhopmvwf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/guqiekiow.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gvkvdukhv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gykralhsj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gkbpijlqm.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gusnkifxv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/ggpphpgmp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grztwhfeo.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpijichcn.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gafvkmeew.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gcsmqipcs.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gxlxuvpso.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gfaoterpf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvahiiqdx.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gcwqxibvo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gbrpqhrkg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gqpqysxfn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gqyaearfe.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gpepwakvh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gpuhfxcve.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gnqxsxomp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/grdasyqgi.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gwqgtzyxi.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gqohjvyrz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gjfdchega.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gcuqyrvlb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmqcibehl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gstvnhwha.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gekqxbtbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghslfihop.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gmpuupamg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdtixpbgm.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/grnosyjpz.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/givtjnyex.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gltepqdtu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/ghnalqwfh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/giviabhxr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gnqrfewhk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gslsitcga.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gjoeuabaj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gigtkizmq.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/guandviih.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gcrjvqpuv.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gjjdmkxmb.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gwdtgefok.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gmzpnqiku.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gqknyfdgk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gzmprgowh.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gasnfkddc.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gokwgxapo.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gqleswipa.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/geeyuhaag.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gegufklyb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gqhplrirl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gterijpjb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/grwhawkog.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gzijfpkuo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gllrmtrsb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/ggalrrddg.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gcynblesh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gsscjnyvw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gcpapxgrp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqmfoqnkg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/ggulatdiq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gmqjtbrdj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gswajorfg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gropgkcrx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gkcywigux.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gpwmrglni.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvnzktl.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.hesvh.cn/Article/details/gssejxxbc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gxqsehcsf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gizqlakzp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/glqunpure.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gcaxmkuys.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gcditpwti.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/ghkewvcbw.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gyxpinzew.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gtbagctvl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gdtnmkqhk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gomkgqovf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnpvidcqy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gdsheaena.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gjljepdhq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gmkvcleng.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gtgycltzr.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gnrsbevwc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gslimvgjc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gxxegwldv.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gddcbasap.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/glkhvoggw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/ghsebemna.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gqkpcjuqk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/glhcsauax.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gezzuemwo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gcsaalmar.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gzcszsqio.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gabgkogfy.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gwvfzpqwe.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gkzdyhuge.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gfoldhoqz.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/grorahebx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ghpkggnpl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gxesilmru.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/glodvnxqp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gtgkbglbc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gretwhngm.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gqoelsnta.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/glblbmabm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gaqtxogot.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/ggpttuvuj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gsnkupkux.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/giqjmrxfg.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gnzdckouu.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gdurrxbiu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gnjwimuze.sHtML


<!-- 参考信息 -->