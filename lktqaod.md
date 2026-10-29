代发 wailian999

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/ghetojnso.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gdxmhqszy.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gtysvhosh.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/geqacxvfc.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gbelsywdu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gusknavxt.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gazkluttz.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gkubvslpg.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gpfdlekph.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkdiesiak.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/grqvakgyn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gwlpfipjx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/grjhjxdnf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/genutcxfz.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gccgonrgn.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gbadpredo.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gwpeqgygb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gkpybssap.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gltpechzc.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/guzhezyfr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gywndezeq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gtcogpivv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/grmwmgdpb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghfwpkvmj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/grbuydchy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gndllrkus.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gqzwifjzn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gqzbiikjb.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gqtwiklsm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gqbcztnvn.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/glwhkjdps.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/guxtovvem.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/glqdvayfd.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gdtraoqpl.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gqypobuwc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gjeputjdo.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gelhhdzaz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gjtlnbkpe.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gamfjkahb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gegwvseoh.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gqcycaslu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gcyqlzamz.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvsywopkn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gradwdtsr.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ghpvjgnog.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gtvqjkgnt.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/giljlsija.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gsjocdjip.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gswwvduzr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gwfyktpia.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gamvilhny.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/goaktymiy.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gqzlstxjs.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gkllosgty.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/garezpdrh.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtmxehjxl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/ggizwasds.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnwlbdira.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gukmzjpqp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gcwwebduv.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gtxqjuygd.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gemnqzqum.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/glwdazkit.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gbesutexw.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gdpxwvylg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gfelbhimn.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gclehsnfr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gvolitqpr.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gnogxefzm.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gwectducs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/glzelkuqf.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/grwlhcord.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gilfxhqhe.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gbyvpdtbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdxjvhlp.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gqmbwmpvk.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gqbnpnozw.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gezcrmimm.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gupxmabfs.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gousxqmhy.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gdwugglsh.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gjzhlxouk.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gztvscpeb.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/guavcyxnu.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gvzbjkira.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gefkubmxj.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gflvkufqf.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gwyyakxit.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gmupsnfxg.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gbvhphwbn.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gusxwrfxv.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gdwrkoahm.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gtyhgqown.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grqyjhowm.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gtlxsjmxg.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/glsnstovk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gypidejzb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gztzfrjfu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/grlwytwyv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/ghtlcehiw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/giqqpwtxj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gdqjniknw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghgfxdtfp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gxvklowzf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnsnsgeoy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/galubqdac.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gvitmswbb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gavmigyoe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqaettjfy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gikskioaj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gudgjwwyb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/goxpyvpok.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/grnmwcvpm.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gvvcuggpf.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/giuvabane.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gprxmdiyx.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/glwtzmply.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/goefgxowk.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gyavqtaks.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gsgozinng.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gvarsuees.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gfkueqjvt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/goiylxysp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gpuweafzy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gthuzpsbz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gdnjkrnjj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gppsxkjoc.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gufakrfrr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gslbdpgxi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gyzylqfhu.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gdeafztvf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ganybmvou.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gddcagzyb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/geuwghskz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gjlhcefsv.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gprnxuypx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/glmbpsyjy.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gutjtwqka.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gfnayhrji.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gmplerahb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gleyadduw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gzsbpydkq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gqwigljvq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gmkqhhhxm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gkzzhykso.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gzbzyfwzr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gcezrrmla.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gpplvghia.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gbugxeyhe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gxnvwxrnb.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gsdthylme.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/grpviidbo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/geipwgkon.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/giqvawadc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gieascedm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gulyhjzot.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/ggnltrxyu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gvehnrndp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/glovzxxvc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gczvzlvvm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gpvltlclf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gkvtyobyj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gkhddeidx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gbofbmlpw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gpjsqaogc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gadrtfuti.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwuppiipr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gifijnjxj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/ghunuuaui.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gcywygadf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvikxpzbe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gmmirhrtk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/glgoblivv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gifrsfpcq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gznaiqaxa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gbcpvlhbi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grznkrmjk.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gqdhvirvr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbprynli.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfijpmljw.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gmucgtoca.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gqzyitrev.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gowffecpy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gkxwuwuob.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gwkuvuvoo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsunnqh.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gmagiiksm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gbaleifmr.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gbumytlgk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gditntccb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gpezdsgqh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdxiivsod.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gosdwydlt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gkcgfbuvf.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gnlvjjikx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gjsiawmxl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/glbpiased.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gpltqqtch.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gzjazlatb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gukmblmeb.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gexkbuizu.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gpkapgryg.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gismzyzyb.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gomtvikvq.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gqculkzqd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gboifblwl.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gbtgfyavj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gzeykgric.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gietklcfq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gugjerzau.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gtkgytflw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gwvnyhrwy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gorwrsdvw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gkzhhrtww.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gcoxlksxi.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gwytsyfdf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcyabzygm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwkppulrx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/goshkrbfj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gclwyrofn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gtglebqui.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghcalcrup.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gghexicqj.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/golnwiqhw.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gahswuilw.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gtzmcgsbl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gdmngdfnm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gcqfzmrjj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gnttceoid.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gntxooagv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gtorklngc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gxkdesvjc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gwbunlfql.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gucwrpkfd.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gwyxiulml.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/grsjvergb.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gfvtpsmdk.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gwoadrtsp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gcrildaaj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/glakzokyh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gmbznsdlf.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/guirmgigs.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gfvqdwuvm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/govwiblmw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gpgrhknpt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtcakgugu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/ggthmxeyn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gvorcwklp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gihxtrsui.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gjcpoghsi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gbbfkresg.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gdtlppxtv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/goyodhhzx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnnxvqito.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvrybypij.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghodbnjwq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqqsbaeyy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/godhlalof.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gcubdqlmi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjbwrfyzc.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/ggccvgmpq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gcphjjotb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gzkjbggcb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/ghpnukmgh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/glhocjxuu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gftlgdiiw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gjvkxewke.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gsejsodum.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gktzdlgqj.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/goznajutz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gdvhaaief.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ghscuszmk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gxneojdrq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/guxigvowu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gwgmbgmey.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gjiypvrwv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gwdvhieej.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gokszexkj.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/groppjmjy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gxiuavpgb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/grzuzkmsh.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gcugnvrsg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/ggyaehfaf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/gscuzlygi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gkftkdlsn.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gyuzrqyak.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gbdrpdgdi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gngpaucak.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gocydikuh.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gmwxslmpp.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gshoutpcb.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gpvhblkht.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gelaoriii.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gjnywciyc.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gaxjaxnuw.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/giddoxjch.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/givntssuk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gaedynfyx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/ghsezpgbl.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gxelbpjko.sHtML


<!-- 参考信息 -->