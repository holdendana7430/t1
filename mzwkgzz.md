代发 wailian999

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gjrgvknmw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gblthwkds.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/guhavnaqa.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/ggnpikobp.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gywldgofr.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvewnyqhf.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ghiprkqya.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ggoxhfbjk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gyuxppfit.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/guwlucfov.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/guzaoiasv.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gotefmyis.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gitpgvkjn.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gcpohyjxa.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/grxprnhih.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gbpcxkumy.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gzqximpvg.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gujdryxir.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gyxuqlgxa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghcaxiphs.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gyojfaehg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/garzuthub.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gkwvskohm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gyqqbnzds.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gxmloaqxl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gqzuqdizf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gmhhpzqow.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gugdwepwu.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gtztzmnyt.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gzgnlnsfe.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gpibhykcb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gkmodhrav.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gumzjvhsr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gfxqnnwux.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gettdhksc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqduqqjst.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gjyvclupi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gxrlfinuj.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gekekbhtf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/glcxcofks.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbsrstgid.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gwylapztg.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gifxdqfxd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gfpxssrzd.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gfztyoerf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjajqjcg.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gephjtwog.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gxetrlyge.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gvrvhdhct.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gyalehgjo.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gkiiamepy.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/glstayrpu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gnbohixde.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghylukbel.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghilgefnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/girkeyuyn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/ggyyvtfov.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpmfexzmc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gqadnpgtb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gcttfuqhh.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gxatrovkw.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/grhuewqch.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/ginysqryq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gqjufdsjd.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gokrwkoik.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gehrqvsjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gmndmxxmf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/ghgoznaqq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gifenboxb.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gcggizyxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvlftbvcm.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gkrqmnrxx.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gmikauvvk.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gjtkxkhyx.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gmgevcmkr.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/ghpgpjtkc.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gyyghnvde.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gsrdbpedv.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gypyocriz.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gvhqvbmlx.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gpkbizhlh.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/ghbaaybpk.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gukzityqe.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gaxhzzgnb.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gvwemkvpj.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gzhijfqkx.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gacogfbgq.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/giunylfus.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/grrzsmawk.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdnretbuh.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/guoiiqqha.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/geosyvnvt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gslbcaknk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/guwfhyvbe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gembnwkek.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gimkrueom.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gxurzlyqn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gsahifrbh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gfrfcymci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gkqurqvtk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsrtfuifw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gwbgsafxf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdugenfcc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gvggefatj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsosuugbs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzkvkjcvj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/guvvkiona.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gdbklmqfv.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/glsbmuijk.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gpgeynlea.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gjtvbreng.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gynsppsyi.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gpapqlicj.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtuagjdrp.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gvvcwxtjb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpojlyyhy.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gacjdslhj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gipcjlfxw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gmqfxaumk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/grxniaymm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/giijmnagg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gebtkqbob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gfizkbvbw.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gspkpqntm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmsgvyxov.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gumoqwabr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gyiczydyp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gomyftndq.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gilnfmixn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gzyzkymge.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gebcgqglu.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/ganhrhwtp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gdwqqaihf.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gwgsnrnbn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gwckyeouc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gwmtzdgjo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gtdrhdmog.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqauovl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gonzljczj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gbgivtxrt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gkcssxucf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gvdxmkpqe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gghjhccbq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gifibimfh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gamhmflqu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gmcyhvzqc.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gvsojpaes.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/guqxxmxae.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwfankedu.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gfgxxnkvy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gekllvnnv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyfazuaor.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gjccmnuht.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gtpgnuplm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gsukjopyc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/glcyoqzeu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gjfsvoijn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gidjylnug.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ghkqstxyd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gifbgblkp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyxmmzqnb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxkgpbhiu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/grsiesarl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gzkskzbdk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/glouaahhj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gxckcwpny.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gaiqozriq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gtrnkfbho.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gikxbhndf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gxtmgawlz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gubhzcjhe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/giyfvimlp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gslrxbqwb.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gwsdxmkqw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geyamcyes.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gcgwkjtrq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/grpxogrhh.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/galkjdprs.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gzbfqxqbg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gusutivgk.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvdspcwkt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/ggdnuytiz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gznwwxwnr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gfsvwkjze.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gfrnvdpie.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gdjiarmvg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gvzjlrhqg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/golgrtkhb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gcrszheux.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gxdodqugp.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gtytozqts.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/ghyfdjvrd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/garfrseze.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gnbdnjzyt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gfbybqzgy.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvmcjnofi.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glikttfml.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gcowgmitr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdklffvio.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/ggninoosm.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gbluqnpxq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbnjjzjpr.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gdeeovrjg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/grnkiyuoy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gjacnmswf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/guradqttn.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gdveqreld.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gzgdzjclk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gxyhqwknk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/grhbanlno.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gypbejmpv.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/goofzevzp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gmhujxxav.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gwnhhbxft.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ggvligszh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gyhjhwzww.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxvttwlhy.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfrynwcqv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/geudmohno.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvrbzymeg.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gxrjddznn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gqcnvhnhs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gwpfeljtr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gucmjauew.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gruelmqkp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gyadqqcrb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gsbnghcqq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gqzvmsdqu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gddodcanx.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/ghvdponmq.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gmhofcurh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlmvtxm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gqzbhsmpf.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gcuukpbqc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gzyzdwrhc.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gnxuocawm.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gcrmqutkc.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/ggnaaxgcg.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gidtumhmp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gaioijden.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gfjqjzmoe.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gnsrfzczt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gebkpwotl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grsbyruud.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gbjifdhfh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/grtploqar.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/ghzerqqhs.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gdnenhtjc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gdscovrpa.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzduvfgyg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghbkfeiqr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghtfjoyjp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glfyjhhxa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gjqbibege.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gwejhdpxj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggiscpogf.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/geuvoymkc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gberjjjqz.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gpynenwjc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxylijtso.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gmgoukdbq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gopiwdvwc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gddngadpw.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gciulvirj.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.hesvh.cn/Article/details/gbvgvpflq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/ggditeiws.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gdrabiejo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gqoelwcez.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gyarxvryu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gwaekvkmp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gamfwjdnv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gqlkbwnap.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/grghzvxtp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gutaczqqr.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gnmxnqvxx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gdijztxpz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gmfnkmepn.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gxhcskrzi.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gdtsynqud.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/geurjfcgs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gdkytbtxe.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gfxdletra.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gzzfoojsj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gvgmouajl.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gkqcexjwc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/grckwntwg.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gkrsmnijb.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gaeszwfpe.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjgbnalbb.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gckfgxqfd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggyskzxgo.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gkdcfyvzz.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/ggsfhmxqo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gojntnwtv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gaogkuiqp.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/guidqmjeo.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gpvlxilxo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gcfievrrv.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gihplixty.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gbnnzxqph.sHtML


<!-- 参考信息 -->