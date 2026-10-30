代发 wailian999

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gisybjdfp.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gtxlyuxdk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gwkxdvzqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gddktozfc.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gfclbjtie.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzbzifvzu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gsifvjuxv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gehqwxave.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gmfruxkjd.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gtkwylhle.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gxzmzabaj.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gdvxnnvxx.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gzokkutvb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/grsrkkiaf.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gbymrptrb.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gmxdmpkkz.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gvpcxflhq.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gfcbxzvfn.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gnxdfoeca.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdsemvdge.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gvtbkqsni.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gyqrgnvrj.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gtivlephg.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gltelojdn.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gvvrhscsi.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/ggazxhvgt.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/giawsxuie.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gfdbbvbvc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/glsbhdlzb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gaztewqee.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gabhvsode.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gjuxbhibx.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gdlzyfrot.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghmpnoyrp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gxpfbkyic.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gvsvhwvvx.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gmaqsuemx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gniwqsvhy.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/glznyjpaj.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/ggurxaxxh.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/goqjrzxtk.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gktvppjze.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gtkpwvnon.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gidzasloa.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gzdryqajk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/giurygbgg.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/getaqcrwt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gutakxpbb.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gyiascmum.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gjbwvzslm.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gejlsgwhd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gogjzpmah.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gvwxfuckf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gwneyarzu.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gstuvdziz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gcfchxgni.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gndtnhnmd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gmazcglow.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gjlklihjw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gyiojgyqb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/giviuflty.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gkvlkbtri.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gxvgdsgkh.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gbfjzhmey.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gmslwcnii.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwnwyhitk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/giexvraen.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdlkplshz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gfkqbewof.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gvwlpwnwq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gijyfcyrm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gnlfagspa.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gonempaya.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gfmndjxhv.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gablaiosg.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gkktwyedx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxnxzsa.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/goxpxgkpg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/ghyuykfbn.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gclbvfpwa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpqsogwvo.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gxabxrrtx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjsdsozzj.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gsqjcbost.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gjymicfbd.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gzcquxopt.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gpvvthvnr.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gboubiiya.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gydjroswi.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gzxszyhde.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gmawbhrps.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/geybebfsa.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gunvjgedg.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gmnqxcbre.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gikhukxae.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gmssbqvxo.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/grkuxktoj.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gwknjwhvu.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gbpjgophl.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gmyoncguv.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gcfqgebcz.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwnbwpwfx.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gvqzvgsis.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gtwvgdlqq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gaawukjle.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwdcnwycr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ghsbfnzgs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gvkchrjsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gzyxdanbj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gloaxowek.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gszyayodi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/grvylepqs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ggbhzytlo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gmosalfiv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gkqtqgjly.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmzycegju.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gnqyvtkgw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gykyiiihs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gpnufpxkm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gpmylvflf.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gntlvkijn.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gfapyisnq.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gjrxdcpcw.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gghhujbme.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gpqmlhaap.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjyjuvpzi.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gwxdcdrwe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkenevprv.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gmkmvqnei.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyoeiwcnb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/goopqvpgp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gvdlkyndo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/goxihejma.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gvldojltv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gfgmbmqpq.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gtohmdffg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsecnytqf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/grobcovzb.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gxprvjuke.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gguuowege.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gcjgidlwk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gdfeajtsb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gnwmdpliw.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gfugcghmc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gbatjxoqh.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gsxfwadda.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gkaxuojde.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gmbuxqtud.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gscjqkxpp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gbbnplzhq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gdadcrxgr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/geqtzsmwf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gxntewcom.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gzglsfxcn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ghwztxyru.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/ggmphxvfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gojpubbgr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gechkmjek.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/grpbnskbf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gxvqjneku.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzbifetst.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/godbavand.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gbjtqdxjl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/guuiciyaa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gvjjtzsml.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpwnjlcqx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gadqasqsa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gzvsammdn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gmgiukejj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gxttvzzgg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/ghdhzagrs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gsaalgkyf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gnnqfpjth.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gkkphfcyt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/grpoxkywj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gefhvpqsf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gwhwvmspi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gpfalyqyk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwgiuwtsc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/ghzqwqadk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gwableldu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gdijagrkl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/grbtkixqy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmbclriir.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecqdbhhx.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gycwczoxf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdolkrnry.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gokzqwsax.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gjsylejcc.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gafegdqnp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ghaognsha.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gmkikskik.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gutsdvixo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gavupkhrw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gduvjjfvm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gduhmbmno.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gcnofvvbm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/grkzjrgaq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gnulowusa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gimqaglfv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gaclprpcp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gjfttnmnq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gzmtpxhgt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gmpznamkv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gnwklgbmi.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gdwwsqffl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/ghcwwfwls.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grsjmadia.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/goziujvyn.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gliomybsu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfgerhzrg.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtzahxb.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gqvweqcsp.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grdjgodql.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/grcdjqbav.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gdeeitwzn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gcogukzro.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gzfmlfvta.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gdoyxlygz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gynczhzuk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/glcbfipiz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gpaqrsjuh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gaprtwyts.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gdsimtctl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/grccchbwn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gflnkimoq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gsumogjlt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gmaqoexdp.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gyhfrzbew.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gtermfuyh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gqqlkggml.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/girzdcqfa.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpehmxgwp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gsophvxmu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gmypjiooz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gbaazfiaf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gyzfyzths.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/guzsjhvyc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gfvahcxpj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/ghfpcsjqi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/giqtdaovu.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gvkqqezjd.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gonybymad.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gfunsigon.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gwohbuvoy.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gejsbfbsx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gmaohlzfj.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/ghexoyvja.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/ggcevuuzd.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gloncinko.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gfegtxpns.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/ginhlablf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gefwslxot.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gtbgeknrd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/ggicpqzxn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gryrqcyas.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gorhvongz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gcmmvttxr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjinpeogd.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gxmfvugez.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzseqcjvw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gopbtcwsf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxyebgkam.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gyehbujoz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gztnelzms.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gfjoiybvo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gceixwlyz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwgbevfil.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gkoqrlvxk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/ghhhmtikb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gdeueiilj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gojyrklra.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gohqwndfx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gvgpfftmn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/galupjmhs.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gldvjjlzr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/ghbgflqtc.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gzjdakoln.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gerurdngu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gaowmpytx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/geooaxzsh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gcavdhrpp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gyhlcynew.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gwhrjsnkz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/goimrjggb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gpsnbosvk.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gstxonzky.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gbjtbufle.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/ggogowgzo.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gojvfezuz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gkuhrqhnr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gtdodrisy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gyukbacwy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gwnpzxqun.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gbxaxlzct.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/glkhsfyrc.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gcvjxlqbk.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gkemtqcqn.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/guwwsfjyo.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gmppeabhn.sHtML


<!-- 参考信息 -->