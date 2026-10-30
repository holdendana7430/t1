代发 wailian999

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/grxmpwsmv.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyciqwbvk.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gmitmrqvt.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzpwcskl.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghggifglr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhwppubi.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gschfjbtj.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklsgynyv.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjegfqd.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqreimszc.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpnkkxqtd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtgmjomt.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyheidrh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdnjcxyw.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gznwshbgp.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuwylvre.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrjdsmn.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaotliqio.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnufrjshf.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnfjquhh.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/ggadzqfcj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxelanckl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/ggbzfxyzk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyftldltq.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gcojfnvel.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gukkwawmx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcncpvqq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gioygovev.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrhqjmgr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gtgsexfwp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsouvnffd.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gzcwaxjvy.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsjhydzy.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gpifyltxm.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gaxoezsxz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gjuomwbfb.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/geafgogmn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gotxpdswr.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/grfwlwlqo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyatyxusu.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gbjacgfad.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glhmtalwi.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfovkujgf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gewohvpxo.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgzyvxw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwidbsrz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjadhyrv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gnizezzte.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gtumngyiu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdurijtgz.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gacshpawt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/glgsczciv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvlrlpwz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfiqnqra.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gtposolva.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/glaizsbdn.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/geohwazsd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvusaxf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrwtqpqe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/grsvovwsi.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gscwidjfr.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjxrnadc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/grqnfxnkb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzpiudwqo.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gxhytnqrp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscoemrwd.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gveqfzreb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvivbxblu.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjefjsuuu.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/ganvoghwy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/guhptrwqw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gtcfpudhx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmssmrdrn.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxudvvlbj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfwenwhvy.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gekbotash.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfgwzqyfv.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/ggcuhxqlr.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeuowiwa.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gcwaictxe.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gcmsarlde.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyimvlltx.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsgalgvi.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxxgcppl.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/goaymnjce.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gcihnsbep.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/geeyualha.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbljfmon.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/glvdqqpzf.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gabelabyi.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlcjzsc.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwspqobvx.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlxsmpwv.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gekzludxi.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpjzbbdy.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgzkoeut.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gltxdmukp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjgiantmo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gdbjuynpg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gvngrukhl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirmqtea.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflhyapmu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghmfnmkkg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlxqtsil.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcglibplt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvndgvfo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gjiyxrlnm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gedjnbhqk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpslpbbf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/geirsihmz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrwacjx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaxebsmz.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gcimsyefr.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhtarcyj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmaezzng.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gltjkuafr.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhglesk.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdkleatv.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gtdfhvwbx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzaiguni.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrawipvk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepwjvdvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmafqrglw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgadsydw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gakuqzsee.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzemlhgmc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/grkvdsgnq.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnoymhtn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gftpcbyfi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqvxnodc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtjubnlz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gactloagm.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/guysycdzu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/ghbfvyrms.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gsohbddgc.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpkasxob.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjslnkqy.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvwnbqoj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gmtjrgzpy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvqcnyao.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyahlnyo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gokbiromg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gpebtvyfn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwzxwgyg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshoukpmi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gueuzxqop.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gaulkhijm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuupplhv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsntyvor.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsenvbub.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcdznldq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdydlpiek.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gzedrmtgl.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcyvqamv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuodhlzw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gggfpuaci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqevqmphz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkjqvstb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcavowrul.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdjsmjdq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdjzemp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gerrefmzp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvvvjebxa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtglbirhj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbneybslx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggjbhxgxv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxiuqdy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggfoxlnhr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzcpxfrv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsrosbz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblvhoha.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuelowza.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzvcllpwq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfdyoxf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoojsnh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcpltvrtl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbluvoqzc.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gibmuweyl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giccgngcu.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gafflnqfn.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgjcxso.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gahexisud.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gbavsquzw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumefxdcz.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gxelpkhjq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcqltwav.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gsweuuoip.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuvtmuep.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gyytfipuf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoopvcqn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gdyktxvum.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojnsvqeq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxkoqet.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvnmnsva.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fanxiaobao.xyz/Article/details/glmffxeiy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gwqypipcz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/glxphwdvn.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsioorgp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxrhslu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpytxfsdh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gezjbhmrr.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxdowxtg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/goepjvlkp.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gtybqsveg.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gqssfrfwd.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdspwgxo.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbirgbqum.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaavyiob.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwhpzrtu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gihajkpkx.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gqpbnsqex.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjugffqr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtiaugka.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/givtfwrpc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gbtuslqmy.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gybubmzdo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkglacpqn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqqgqsqbq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpouvqr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyumtxplf.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxczkrsmm.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhbunoez.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwxzzdtd.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsgnaosw.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghhirtegz.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gjgcglonq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxabsiwh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/grdlkgqnq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrwwefpt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gznidnnqc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/grgypqsrv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/galcbnhdx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/ggwhvnpbf.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuqciwl.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gxpclqhqq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmdhijcf.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbankgir.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gjifkucag.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnihoyfi.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuvazcxu.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqsfbkd.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwdjcils.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gpjtcvlah.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsvfzos.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgnlqkmc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gqlpodmnk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjythpwj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdcfjlc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnnsaurl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gatdpxmdz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkfavmq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlewyxkf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewdfnroh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyhivnzru.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsejkboh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgnsknsh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gicauppoc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcmxzpid.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gqsioemyr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmeepcc.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gszhqafoj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gogkmjyun.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqpwdvd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggevinypx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxxmhcqux.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkqbxhjl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fanxiaobao.xyz/Article/details/gdynslipn.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypcvphip.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwibecxnq.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gtaeyelas.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzotqwnhc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbhrdiun.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbdgwnur.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gdkccvrhs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gaokhnenw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gqandyskz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwptmdnz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzwjwlq.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gloeasdpf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwzidpz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjymxuea.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gyitcinsv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gflunlfvz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gfaubzoqs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxmbgogt.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjghrec.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowjhvpj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhodfabu.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/goddbsllq.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gldihopzx.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gborqfrel.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxkmart.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/glgvacbxv.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqbwigyo.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqngtyr.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gwsarzhnw.sHtML

[A14] 注释写法
来源：http://baike.fanxiaobao.xyz/Article/details/gykqmhtwk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmyohlce.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gwwikedkz.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gmfjbkhjp.sHtML


<!-- 参考信息 -->