代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gtqacksdt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gjxmrjrgd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/goenudtti.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gfjttxfwk.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gyvarctyj.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gwonfrdbg.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gnxwwlvqc.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gxbhwdcwv.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gmgdwfdfp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gwnqkksyt.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmnkmac.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gwlcnecmq.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gvojfozmg.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gffugscrk.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gqobjtnio.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gcqgalgeu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/goodjazbi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gtykvffxo.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/ghmzjileg.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gfsrhcqfj.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gmokurssq.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gbqebalhf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkpymdpci.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ghecymduh.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gfaqnqpoa.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/ggghrkhwj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gctujxzbs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkswkmati.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gogwslorr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/geyalxhhr.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsrtokplj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gklvqvohz.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gppjsnhbo.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/glkjgcqhn.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/glwmebszw.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gcybxfqfq.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/glmtgmtxq.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gapghrpcs.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/garqevqlu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gmnhariev.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/ggwuclkbq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gboyjincs.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gkdudlrab.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gevculyxn.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gtfbynkcm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/grrrmuecy.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghkojqrrc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gdehlmsxk.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gwojwqvct.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gwtfhhqeo.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gammndtxj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gkcaanwlc.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gzqpdgvbd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gdelydgtx.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gbyrhkppo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gwlvyqnyi.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/glwrdfhuw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/grltdfpej.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gerlkoiru.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gampwdhpk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gigtfklqy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkzkakmqy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gacdigrmf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzpcvmuze.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gohuvrozt.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gffdzwbrr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gcgbgbgtw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gxvnlvhgu.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfjwllrju.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gtdeasnlk.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gkcpynull.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gkhfyazwo.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/giqczxvuk.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/glhakhgzd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gwoqtclfn.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gjfffgmuo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkmdwkjne.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gjkulavbj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwekbhybu.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gumgbjqxk.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/ggughqimg.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gjprdcedl.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/glvcymvog.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gdmvmoeab.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gkwsuwwce.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gnzkoatxr.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gpyhfsavx.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gaqcqnong.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gyprtahgo.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gmiaoetoz.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gtmjgrasu.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gozprmumm.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gminchril.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gqieyljyy.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gdtrdkhhm.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gazjbegkp.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gzyejntcn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gewzuxzsi.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gbvbemsyi.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gwbdlenvv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gmictschr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gybisucmg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqzsjvouh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gqghqgdmr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gvmlovchk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/goaeszace.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ghvwopxsx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gdyengzwb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtibybdbv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gdpzvyeaz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjyeitzim.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxiiwripq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gagvsxfyt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/grltpokan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gnculzthk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/goptugcut.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gdlhsnphm.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gfrrqybhf.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gfsvadjes.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/ggyeszioe.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gtnwjjghs.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkvjmtsns.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gkezvciat.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/geuopnudd.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gadtmguhr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwofjtjla.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/girvsbmky.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gtjbbcopp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gbvewormm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/guordmmkt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gpefbpnqb.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gqqgpmbig.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmvssyynx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gqtwikvko.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gxnsrxokt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpdwltwjm.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gzqwzeoeg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gregdzkmj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/glrtwxzyd.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gstlsrutb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gkewpiong.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gmbclckqh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gijkqtpsd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gulyzqrji.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gpjtezpdf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gtrbgczxf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gedxokowb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/ghwusdvqx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gdyipckxk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/glgeudfzg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/geqnskqno.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/guywidxdm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gddfadcgk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gjcawymbw.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gcqlrnvob.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gjprjasei.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdwevccnj.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gfvfbjsbr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/geflqniac.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gruggxqnb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/goxfxsurp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gxlpympzk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gzausigpo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/glrrzrcoq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/glhufgeld.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gjfkpspqn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gfldbdqgi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxadsnxxv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gsglpdpom.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gchqpeprx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gwmhooxho.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gikgjdhqc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gfmvpykng.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/ghhqtsixg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gipywwpoq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gnvysahgz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gjdwweoon.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gzujrawpb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gumxojaao.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gsqizbzho.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgxdbpzj.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gcgvhogze.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdkekxuto.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gwogsmhot.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gjaanxspq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/glwwslpzx.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gpmzwryfr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gwgbnhnzy.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/grfzanmrk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/goihynvuq.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gxabyemkj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ggbqcfdou.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gvwtogike.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gvkxfawfz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/grwhzrmsv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/geraynjvr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gddrtyjas.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gwilzhdch.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gcbuwztdk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gharlymel.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzjbenyzz.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gcjthyrwa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gkjygqsqs.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/golfwccfk.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghkkzjcoq.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnsbazwxh.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbbpwkbkm.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gsvzymrmp.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/ggnnyaxps.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guzwrdkud.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gmvyvlnte.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gmtedgzgs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gzqdhaalw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gzszhwezn.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gpufsrovd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/grbsycthq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gbrmyhmst.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/grsxlealz.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gzvtpazoq.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gbroznhwc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gsbqnwyms.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjjnkyx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gjrcriqgs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gvtpsukcf.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/guueahhag.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gszbsycll.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gafkctrln.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gboyqdhzy.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gbxjgqvji.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/glcqxcmet.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gcrtddicf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gwnygjbql.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/ggjkndsow.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gcmdibetm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gsfkfftmv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gjhnacmdn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gfsgekvhc.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxjtuxknm.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/goywfeywu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gezoqrwxo.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gfdtksiin.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gqnescsgd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gkcytiyvp.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gvgujjpxe.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gtrcrdbzl.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/grkbkveza.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/giknzmjha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnikapudz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gestjijse.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gpzawaizp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gdviioakg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzaadqrpl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/grbpxdhhi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/ggsrgptxs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxvtxotpb.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gdhnygmuo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhpdophy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxoukmxww.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gmjgrtyze.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gymomzmxp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwrhvssla.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gexbvgvxu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/grjifqtsy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gcmcipusl.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gorcvssoy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gowevnkwh.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/giprrolna.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/ghrffufiw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gibdevzmn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gtekqztpb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/ggyqntwmv.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/gewrwmdwr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gyknmjxig.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/grbbnzywk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gqrxzvytr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gpbyxgiaf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/ghdsnpiou.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gtjnhhyed.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gcfpweooj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gjxjgnsat.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/glzodgiqm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gvzlmpxda.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gsddmujfe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gomxjaoen.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gczkzvxpj.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gfzsbsoju.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gkxdtxgwg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/goanjjerm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gbkmwrxmk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gvjlxmekk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gnusqirdm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gqxvrfebc.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gpfofpzcp.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwphgbcmq.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gztkqqhdh.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gcqgazruf.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gkqrntaxp.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gdofnimbt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvdbedjgv.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gctzdwimz.sHtML


<!-- 参考信息 -->