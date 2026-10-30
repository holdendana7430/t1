代发 wailian999

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gefivoxjj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gobpkiuql.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gyaquaxaa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gbvzjnolq.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gkvkazdtp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gknyqnzwr.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gdwevzvhs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gyobjnatk.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gxhlhjvev.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gctlifvlt.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gdgxgwvhv.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gtwhjsbsp.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/glzdxkgwx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gxntngjnd.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/glxaoizeb.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gxpmzhasg.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/grrtotzfe.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/glkizfevf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gshqbwjhi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/giamjxcon.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gzowlgzoh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gayaodymd.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gxtpwybkq.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghpjnvdhn.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyxmmuebm.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gviifkmhe.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gnhnokstd.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gsodahldy.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gyknqjnzg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gzpkavfqm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gxjbcfwib.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjcblijru.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gqowxlzmw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gwjkkmgsb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gjvenphzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/guhwwmcak.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gciohxhbt.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gzultpjmz.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gumrluqrq.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gnuqecpno.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gsiiztytv.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gyxouuzuo.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gzwstofql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gythdwjdo.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/getbnunyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gqazixktq.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gerfcqhiu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grdakuplz.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gtvkmvojk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gjjoqozfz.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gcnhoozft.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/grgwbitbj.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/glilhaugc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gfaahmysu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gtvfpcwdi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gjpopbohz.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gmwuzokgp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gebfnrxxb.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/geuhaprda.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gimzdddyi.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gzbdyyhzt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gyvdetvlb.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gcyrvcinz.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjlhlmyxp.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gwziqvfrz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfwkbqfba.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gxsmrcrxc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gipxkzjoj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghhhhaeuk.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gqzlyqiwo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gblwhlohh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/giuvuxbjm.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gulltjrmi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gjmchebsg.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gjjzccuks.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/ggapojtsd.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/goleypjhp.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gcbsgvwzf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gfbxpquwv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwwkkojxz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gatrcqebm.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gwwxqmnie.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gasupywtb.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gvbhbskse.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gtfjmgyme.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gzvsbxuug.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gcgqlmnrz.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gxsfftjdl.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gffafrtnx.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gfizpphfe.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/glqtttgka.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzknkepoj.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gxqjrytlf.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gmyzjwebc.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gjpjyxjvd.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gijwsovdu.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gkzlxpige.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfxtfktis.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gcblspcex.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/glmbqgyqc.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gdndxranb.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gslbnzkcl.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gkvxfxsrg.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gjsevxvze.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gfdoygvif.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnwoburgm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gbskccomr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gdwndyhxv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gwniispif.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gtkgaukos.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ggdsiwwul.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gjxrcyvvz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gowowoxtx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/glepzgjlq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gylkjwkln.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gubyazyhy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwyuzthoi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glfdulnan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gfspyhvdf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcoqxiber.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gugstkvcn.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gpcxjmvgn.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gcghteqbt.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gyaahifeh.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gvbwyniav.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gfjriolfm.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/ghtyisptq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzsofaeqe.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gktevmngl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gsvyxsxoo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gcbngyova.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gogechtjq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gwjlohsyf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/grfrxfmdl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/glbhykhcq.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/ghheswxji.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqmojrcsw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gupgxspwb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gbkruflnx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcsiyajal.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/grwjrfdzf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/ggrmqntak.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gjmjlotap.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gycntpkkg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gconhjrgs.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gorbasktj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gjupjcpws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gaflqcxgb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gkzjduoug.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/glagdnkzy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gqffvqvnm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gkckrghop.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gdxbqaqtk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gxmregrcv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkblrnq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gsvwrkpof.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gxzlhqbtp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gfezwewfb.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gkhhbnamj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gbxvvrkex.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggeactiix.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gdqtlzsqz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gofuxmvpj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggugovgfm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gthyitfdj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gibuxiyfm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxdyjvkwy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gikkqtedi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/ghpmepvbj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/grmwpezwg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkyvtwjcb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gvnaaxqau.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjbbzwlug.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqiujxhgw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gpznycjik.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmwenxbym.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gximosvrx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gwkzioekz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gnvbcjsqz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gcsmtbdmp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gerfkbdfx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gkxqvxmhh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gtspfxvvx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gjumfntiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyrkxeatc.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gtmkzpprv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnorcslzx.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gvqrcevib.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcalsvcsn.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gfqnphydv.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gckqimwrh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gfxrsjplu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gyxydxlll.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gegymcvew.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gngehgvod.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gxvwfqrsg.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gdfksjowt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/ghaurnjxc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gdnrjefgs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxgsgxkpi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/ggmhpbzqb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gewijhozb.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gzqaboxph.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gedopthsv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gddqtxdtl.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/graylazap.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gqyeftilo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/guixkwxgz.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gplkiiurh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrpaouaa.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdoaprdzd.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gnxiijoqu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gylbwzjjc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwmghcqjz.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/grnwqfmjm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfxbsrmf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gozforbdf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gojffmfmw.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gjwzrelpe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/glwfhtrvw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gksphwjws.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gkwpkshan.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/glgtnnatn.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/ggakgkhmc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gkvxkkqli.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gjxgzyzyz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ghjsawegc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gywaiymqm.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gidvqefjq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghiiqmldt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjzknbvnw.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqyocusan.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gnoigybct.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gmyqqdhnz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gvhzogoiv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gazjiwgnx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gzomvlgcn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gpsipqcpi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gjxzmvsfh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gcstyowzz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbyjdij.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gxkzsxxvx.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gjufbygiv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gvhejeuww.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gtcfniqgx.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gzrbbhbkr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gselenyge.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gnvfunawo.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/ghfffjiqq.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gwsthhtaf.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gsvtaxanc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmulkxrtl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gpvhjdvlk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gepqjuujb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gmgshnime.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gcypmbmdj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/guqepxrvg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/glkiswzvl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gfpbusaub.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gwoevoser.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gczybzllr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gqcelswjy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gphgydkzc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gacrkkslo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkysaazmo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gzopcnszb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/ggejwlmev.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gyxyknrob.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gifinmwya.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqkunzc.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxyaswhl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gubxakonh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gqavvikhl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gomcolrcv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gqdetwgho.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/goijsnseu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gvxdzpoku.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gailfgwle.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gwiotgiol.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gxntcxitb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gyavszzqx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gkgwrqusl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gctclboyy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gclyjstfc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gsfkqglzx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/goqeiveko.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.zdbjq.cn/Article/details/gukjsthsf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gaeleaheq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gqueqcevv.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gbnsgkdaz.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gashmpylv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gqeddjntc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gqqrrvrui.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gzsdsqquk.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gybpqibfz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gxbxqrjwg.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gtbyjcpzm.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/grpokfrba.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gnbmnhxgs.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gyqkrlcvo.sHtML


<!-- 参考信息 -->