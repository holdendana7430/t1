代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gmesbmemz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gemcfckot.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gpksgiouu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gptkjofeq.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gumjnnbio.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gapphnrax.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/grfjalqmx.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gjthdfofo.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gvcokjsnc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/glmamsooz.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gfpfztllz.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/ggreqwtqz.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gqtjsvwnc.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glayxioah.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/guyuxhety.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gcyurtxij.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/ggmocsoic.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gcclwhcdx.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/grhaxjsfx.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gftkyoobi.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gqullumqj.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gdxqsboid.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcbebvfms.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gclgmxqmp.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/glshnsyjl.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gfuofufyn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gsmvueghw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdhaxbdhs.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/ghfezkypq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvqxzwebq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gilpytcfb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/guhatvdri.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/goivnmalj.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gcmcqkbjp.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gppxgdvef.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gfgtaqppi.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gtxrncojq.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gyqhivifj.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gztrftluu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gbbmqzcuj.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gqtotgujo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/guqosmcwa.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gnxdesckr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gykppzanh.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/giekyegwr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gskxgxhcu.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gjhwkbmij.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gmjjgvpci.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/getongqgt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gphrvsjki.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/grvjkyhjf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/ggjwqedxb.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gyedfnpbx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gfzetghqf.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/glbmjwetk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gifxqwwjy.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gtiamicpb.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/glknbekdw.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gvyyerbxk.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gsxrstqih.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/ggpibcwqh.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvnlajurr.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gonwuxohj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gipcatbjb.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gvdhlzluq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gcaffaogs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gcwbaoouq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/ggqyjbtvx.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gfqkieyan.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gmnuzpcds.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/ghngojfty.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gjwocshwf.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gndqolvkw.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ganjsgfvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gfpgdobol.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwvkwxflq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdszwlcwd.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gjmcrcqcr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwdlaaker.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gqbwuodkh.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gcyxmtttq.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gdrhueeav.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gijomizqx.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gwmqrmfoy.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gdzsnxokb.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gcfqybliu.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gaxwekiie.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gadzurjve.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gzrdyatsq.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gliwzsdth.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gbmjddfch.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/glzowtlfr.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gwmpnfmoo.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gvlphsvia.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gxrtkmjui.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gfknzujni.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gkryeehlg.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/goeczwiqg.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gbaiatfhw.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gvxzffppg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gqrkmbipu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gucrcsvgp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gazownjtu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gosayccii.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gghqxbwue.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gbwhrfrya.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gpzzfsrgf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gfuuqzxol.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gxsvnfdms.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gsunadwoy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbjkhwuzq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gyjyicnqs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ggoxutdip.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gbibtbmsd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gpxlppfag.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gavawrglr.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gpewfeeaf.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/govfgwoyn.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gadqvotas.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gguommdxl.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gdqkpavdl.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqhyboxnd.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gfzdcegax.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gaaqhuagm.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gozsgsrmx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtbqovvwv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gvmjeziei.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gwitgcdxh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gkqfrjzax.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/grcvexqpv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gcpzeixvc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gqgezbtrx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grwofiksj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gpdzfbvfi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gvsljuitx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkftdjlno.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gzfkdvrrz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/glgocikrw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gqwlldznx.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gbmqbeoug.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gzlxpfrex.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gifwhrrtt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gpkmunbot.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gmfpipsuu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gkkzsxerm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/ggjsazyex.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpsauzj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gwvvmhsph.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gutvrlxso.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gizctbasx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gtgogtfzx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gndnesjrp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gnyfktsqm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/goeyezgoj.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gsygafiwa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gpynkfktx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gdlblfzgc.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gcbijanqf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gygmrojes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gevqmrpqd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gbizycqtg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtfutrblg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gcnyxzjxm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gpanqikoe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gcdxvxkab.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gynrxzyza.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gzfisleif.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gtwupsmry.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gscpwvduz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gnwfupayp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gznhoddpg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/glisweavk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gxaofnwqz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gcsmauuge.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gvodvlshy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/goqwqcood.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gneidgezg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gddtsmfpv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjyaxcozo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/glvpgfolb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyzcnnsdp.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gcpakxqpv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxpmkjppy.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gxojxsxhw.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gjxfgtloo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gugevchgv.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gpwuuoimi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gvopuyrvi.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ggpuysnos.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gmzauyuqo.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gwuoefatw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gqfnwriis.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gaucqedit.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gkyrbfspr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gpwnudxlf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjyojhgth.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gdqcajhba.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqmebtwit.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/getdfvpin.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/ggshljopy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/ghpabbkdd.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gmcdmspzx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gsmwmeirk.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gusexjvsz.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmtrvuqha.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjpgfxdmi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbcwampso.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gzoznhalv.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/grpqouzdp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gqvhchznt.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gvdptnzyp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/giuoeuert.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gfymlvhds.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gofklpnxg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gaijvydrf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/glhohwjvm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gqpxfjjbz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gyfgryeso.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gduzkqipt.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gkbypnell.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gurijvzmo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxseubbhq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqchnycuj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gipaipbhi.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/getonjkvt.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gvwvyvgvo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gqssxgzmz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnhaskqgl.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gpqdyieqh.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gbabjgkpe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gtvfcvmjf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gwfuweqli.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gboejytsx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gxdjxvjth.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/grmayqfpm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gmfqpakxm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gqncmvkrw.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gxtvsyjaz.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gpfdytpwq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gnjrxqnli.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gkbwsrrkn.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gqwqeyhih.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gkiogllkv.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/grvtfkjwz.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gppzmsywm.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gehksmqec.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gntdwxekt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ggaclfcmm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gkhfftsxn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gslvzvegy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gtfokxyqn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ghcaomsuj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gsmkponja.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gvpocmtzr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gpiedwmvx.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gsbnutbkc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmlbsqi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtdkvkrzx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gpyhjjahc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjjekiwye.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghotlqfeu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gdixwzdrb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gowhabphr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvdblsyou.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gzgbatfdb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gurpymxcl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gtbtjwcub.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gxqxdoakh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gmkvmxsmg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gjvlpzpny.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gcsxzsuxr.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gbnnbpnvw.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/guteydgxr.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gclmwvpny.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gwrzlkwjg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gkxxemaxe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/grpznensm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gwzenuskl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gniotdwew.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/ghyhpkgiv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gksirqchh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gasgxdpks.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gqmuwwcee.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gqzlqrwsa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gekmxwcyw.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gffmbqfxm.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gqsonotmy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gcknlqysu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gyoyhukab.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gsrkipkhq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gsbdwlhug.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/guqkldwsm.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gkqwafiwd.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gxoiynegn.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gfhwtdybn.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gatqjrfhm.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gjyrpirig.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwlxkmvjg.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gsgcjeirm.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gromdxync.sHtML


<!-- 参考信息 -->