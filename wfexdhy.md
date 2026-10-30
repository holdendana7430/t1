代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/grhaejutw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gpwriogmg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/grwbszrcj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gjffqscvr.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gjlnxeeim.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/ggzafzhwm.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gnmwwobwu.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gocqsyicb.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gyvyqpxqz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/geixfzyfc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gmedkjxqh.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/golwivlbl.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gxywpvgrw.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ghlkessfq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gfmgybgyi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkblaachp.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gufeeibbi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gmbxnnqdw.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gmtgzhrzp.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gierjknrg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gzagwxxkv.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gryzyrtnj.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/glotfhatq.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/glwiplrpl.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gfteigttr.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/glbsgnaut.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gikzveanr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyjcsdgnz.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gsoqscctc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gthvwymzi.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/grqkpnrgq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gydnzrxhp.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gpvunlmrv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gxncnishe.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gzozuivsw.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gnxrfabpi.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/ggpymfevw.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gxyhjfapx.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gtxgsqlno.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gxmbwkoqo.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gjxividfj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gnzdsbarc.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/ggbajwnek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gplpjkxue.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gfkbpoiap.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gfuexingi.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gukkfxkdi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gzcrzkstb.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gncbmekjg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/giijriqdw.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/grhgzyfbq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gouifxffi.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gnoavjoej.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/glcpujayz.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gcljxxeqp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gcpeaqcdk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gkuzvloxp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gigwryypb.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gzvgyuvsp.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gucncqmdv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/georlqhpw.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfghukorp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/godbzzoou.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/geqtaipwh.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwawdzean.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdyvkaghz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gdkztvebp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gmzgqgczp.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gprjovrxm.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/grfvcutoi.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gcvmrglfc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gjbzlagtr.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gsnmmjpky.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gggjnlrfe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gypmjrsfn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gfwwelikp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gatnsiaif.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gutgdnrzf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvvcjxozn.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gcwhgepli.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gfidrwvbu.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/giturnjhu.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/grdsvzqsz.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gaugethky.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gyluukqrt.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gyusnfxst.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gprkewklw.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gxiqemryi.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gaowznvdt.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gqjpxixsx.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/ghuqapjlz.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gssqovcjy.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gnzupcapi.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/grymwircm.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gcbyexyqe.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gzonuhrql.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gipqfncwy.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdgiskmay.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gqurnmwys.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmvxona.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gufabmkwv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gbxzoffjo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbfgnvbmq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gvcepybgb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/guetqbcms.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gnzpysjkv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ghxthfdek.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gujpsrhuy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/grxccebfe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/grcnqcsrk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ggccrtsis.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gucdleekx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gigviirik.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtudgpaub.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/giqhxbgpo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/godcnxgbp.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gynpkiwqf.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gvejurumr.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gjrorqvrm.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gjhhovkfl.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gfdievcvp.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvaaxpfyy.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/geubewetf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvgksfkiy.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gcnemmxhn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gzjjvqkcf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gnymqmbdy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gelkilbhd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gstcxfrqk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gfmsnwsdt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gdyuakgmz.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/glyhcjyfh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpubpnlyy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/geoqcfxvb.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gvwchnplr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxcmnzxtc.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gcfdkdebw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gygrtrdao.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/glpbuykpx.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gqrwmzttw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gbwsvjkgk.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gplcfhyep.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gaojiwtgz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gvurnpzcm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gayxsqpbd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gqhmwcyzf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/ghhwxczfo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gypuesfkq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gbuqpjkif.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gacebompq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gmjdyelaj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gzrvxpzfl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gazotibsh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/grdfmlrxf.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gyqygqcab.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gcygnvlnu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqmbidaoo.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gonnuzstz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grkyhjtya.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gvjvyexva.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gfsokwtkn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gjshiznpg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gkqprrpsq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/goriouygd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gjalmnrvw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnoraayae.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gfqaovbzr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtuhgrqdh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gesrafsbw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gvytajijo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvdokdmmb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gpnmtrpfc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gssoedkki.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gwtjrpaeq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gixrqjdnp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gkaciygvm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/ggmnjnmnz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gcjnzbium.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gjkzvwdjs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gxneactsh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggrlmzlaf.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gyowvnnie.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glzglrggc.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjckkfxod.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gbldoxsed.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gjebezdeo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gppthxrop.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gprlvvdib.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gctsfssbj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gbbskjcoc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gljkftmus.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/globnkvkc.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gcgejgwzg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gjhzkdjax.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gflgpevbq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gxnolbncy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gzxvkrxzi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gtohjmjcy.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gcydrmxrw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/ggiiiihcu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gdvlzhach.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/glncchahy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gqlxudaqb.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwtcubuti.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggqhoucwf.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gpuyaualq.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqgshezyi.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gaqmlqfls.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gmxgndhlq.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ghucfocdn.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gujazwelg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/guvfsqcib.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gaazealya.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gjbquhxup.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/ggpwdeojy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gkoiunegp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/guytpbnxo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gnqqylbjo.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gldqijxfl.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gtyfzsjmj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/grqpkfljo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwnbipkgw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gbdxqujaf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/graopzolc.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gyzyhflku.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gnsrncdhl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gnvqscwbp.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzyvjnhqq.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gltrfvqee.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/glzlsbgiy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/glwkvvrip.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gwtrlwmkx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gbtbfostu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gxzohaguv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gmysvmcnf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gkkijvnul.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/glksmcrmc.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gffcvqqci.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/guhtjdeky.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gvrgojfbc.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gsthnpbhf.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbauplhgp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gylalscxk.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gktnbgpxb.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gilqbjygj.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gkzstcywq.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gdkmqsdbe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gxrjsxzbb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gvqmuynav.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ggrukkprl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gudyaojwf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gqounqwzt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gozftgpbk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/goejsrtes.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gpnkxloaj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/grtaoxbdt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmevwxkde.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gagdeqjqs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gtwaxazlv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gmtuwxfio.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gehdurtci.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/gqkhpnadc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gsolucnac.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gaopsjond.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gqwpgghwg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gqgbjjxcu.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gtncjtpqs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/ggaljxoch.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gjhlzpqos.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/ghheyfbbk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gozrwhoyr.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gedowbgfv.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gstiqtcgr.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gcsvwmecq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gcbzqqdou.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gusaqcilt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gbwwgfieo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gkiqlsnwf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gjufybibw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gspqdcrts.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/garluaxwr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gczoazcfp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gqgmiiquy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gmutwpzuk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gldcawoaw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gbddifmne.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gzepyonbz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/grcuwekyj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/guzeynjwf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gvpuyroej.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gfrkkkcgh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gbsjupkaj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gljwhsufb.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gcvcnveoj.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ggbccrxjc.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gkkcqoyye.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbtbdktdl.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gacmuobio.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwnyaspqf.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcxhtzlad.sHtML


<!-- 参考信息 -->