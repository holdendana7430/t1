代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fpybhbwb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nrilentw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wqxbnwdt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ijvgosxb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hspbyaop.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lvkubvwf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3oscyvcps.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qqujhncr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ipojblub.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3nvmhbqli.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mgfgfgod.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3idaxhyvb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lhbjdule.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zdqdfxgi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3meagynxj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pfkztsaw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xsplyktc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3sntrtbso.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ubisaqjx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsoqditg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yclspemc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ffxgpocr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxjssy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nhlkpzni.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3osdvvfam.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pqnidijy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xtadfesg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeofwesf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bmitduqu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3frhhzcqw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ycicjpvj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ktrrsrat.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3otscholp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3usjzjnyn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dstyvoqe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3giuicrzw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zvhausri.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzjjvag.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tnjxjjfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ypvberps.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vxhbxnue.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pxrcaehl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3phrcxvvz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nitcrdct.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xkffdhom.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ulwsghpj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uoeclrpn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ssetehsc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ioexrzyk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pibgemql.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qlnagrnw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3caussmfu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3igztqofj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sdavlkqt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gpalxcrc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vmkwubwj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xtegpkbf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3icedufrw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3nkzfwfjf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3epeemafe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tnaygjhg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3guothvfh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bpjuavje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjnxghp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qudxkfhi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3evoazisa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ltivzxfj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owaarwuc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fxxskcvj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3uqhqqrhb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zfacoovb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3szipjexa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vvmzfedc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bqxeivsx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qfubmafu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lioqrvxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvkgomuw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3eyvyjkmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djdlafly.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3aneqhxft.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jmxcppno.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3czxhjppp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xdgtdfhg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dsfsklrk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wrqtuaid.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dmrahtcb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qyelhldm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3haepxgel.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pehxilyi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wwovhqxu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3slhjjxvz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mvdnaclx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eevralfw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bmgrahkw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ajmpklii.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ukedwrel.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jbwchcwa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kjnebiiq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lifvjxmq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bsgjycyw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pdtnniye.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mhlugaiy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3llnetkub.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kpolmgnz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nulgsxel.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wplkhvif.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qskhpxkw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bwcmgvrk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rffuvvef.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wdoyrmzc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ztcklluf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oykftxcw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rvxwclco.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zwfbxasf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3udbjdrzj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bplgwmal.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rjqwkmla.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ccnwqhlq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kbfqpodr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3kamsguef.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ejllenod.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cvbbmidc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vkfqsbjt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bgukdddv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rfwrqfkz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zzilyrct.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nfbzjmbe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3slicaysd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3labkbtrk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3efgzdsga.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rxlvjdcn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nykabksh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqtalitd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wqhkwdil.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hjgqfwfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmkiquiv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qecirbsn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3jswxalfn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wzcnfxxu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qsumzfjq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3calpbpmg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gavlofmo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mdolhfen.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vmbdjndc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3axswgtoa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3cdvhgizi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wyryofpn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3cduakkzz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3slbpsiil.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3owytuurf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nesiptcj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xxjtbsiy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ttrriqaj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qcpapieb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3odxlyuri.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dqysjllw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jlkupjel.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3awlbpqnt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mucxendc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ecidcfgc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lpqpfcdh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etgwbfka.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3phzjkxgu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3vwyaqwlu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqnoiewj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfakurwk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfiqbsiu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eyfjliug.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bfynquqo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xsjqujof.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vvpbnqjs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xprldbzc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gvyywchj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjqroncz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dblgybmf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uktiqefh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3erjxpldn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vstnpqqr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tvtdwisy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3smflootb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytstqxvd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytmcdwok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjxjsndm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvhymiih.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gvgttmdw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uyhwuxao.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rikwdjun.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3nbuehbei.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uqykefru.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bqwaywgp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qyscblxa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gvvpdusr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tukihuoc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hgukopgh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zujwttgf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bhkdzgqe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sfmroqsi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wsihcesr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3mslxoktw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3exzinyqn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hmfwdpis.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ikourosb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wymekbqs.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3odeitlcj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ggirewmy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3befedrel.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lvyndiza.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bzvbutod.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uwqirqmy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vgraezsk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jnmnzsou.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bbfkpvie.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3drigopyw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dtmpaxxh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fqllyvtf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3snmzhwgf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nnkcqrgz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3tusfnzlu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hebxleal.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zotyhrww.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3uzfeqsii.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fwatcwxf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwiyvhxy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3euhkexyp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3feysacjf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pnmqcqek.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqxrhshp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3csoceohe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rnsbzwec.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wubdjkkq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gbulcyap.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mtanwsif.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iberzggf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3odebldoo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkvsydx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qjbcgzjx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3afzfkixc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncomqriq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bbvvwntd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbosilz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xfguedqe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tehatlyp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vgblipxz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3abrxcllt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mysmfvbz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mcjydbru.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3acsgismy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xlmecsax.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbdtabm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xvvdhnce.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wioudxdy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fojrhlwe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtamepr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vvfialwa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kvghaajx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zvswjkra.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3chqcbrzj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrgoihh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xoimiptz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeeobfe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tswyytfx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kqlehdgc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zyrtxqsu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mzkdnkmw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qzhrfqiz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkfwqfw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uqumsnyh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kuzswenm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3htrhnzyf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjkfiwtl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3clqvojvi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gprkukjr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rdvypkam.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vryanpyc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pmxphxkv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zfoupohk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nqbswlhd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dbyzwpoy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jjvhvptr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3yojywvqe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qtxciiej.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3loibrimo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ncvwajhf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3awvgwvyg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvhyedm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3panaespe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mvvdthdm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3uwlkxfza.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ozyqpqsf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3urphvzgq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tlwizoxn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3wliowfqr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mendqebo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zkddidcx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3utcicloc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htbvriwu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tcpbmkpa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebbxyfil.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3puzctonh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cokhtlnc.html


<!-- 参考信息 -->