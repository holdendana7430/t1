代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gzstdkyph.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/goarbpwkg.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gkrddzmlt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gmotqdovq.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gheguntvz.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gtkghpbkq.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/goiyknqdd.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gpupaohkh.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gcmoumkwn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gahtvnnxg.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gnkwsbeck.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gitbciufe.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gvvwpchsy.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gyaxmpsqy.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ggoityidw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbbdmepql.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqmczjcth.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/godtiwtjl.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gtgfgrdcr.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghhuudzlp.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/ganqrfppj.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gswnkehib.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gptlgbkrb.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gvzvrfacb.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gvuefalvm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gnulkkgnp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gfmetvvdr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gydplyvgu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gxnlbwici.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ggnnttokg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gakdibntv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gbszjjopu.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gsgtlcfic.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gtcftwetu.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gydddooin.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gjcgtfunv.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/geidlebwn.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/ghqidicpm.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gppodfvpc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gcwjynwca.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/ghxmnupzl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gktqcgavh.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gsmaermve.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gjnduqhxj.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gtvnwupan.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gnuddgidp.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gntxcsixv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gzeinukob.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gotccopba.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gwlvztxrn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gzhuamkkn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/ghgevluhj.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gfcxorsnt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdupgpoi.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gacwyajlz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gwwchjgwh.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gvjcrmpoh.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gobhrayil.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gnrgakecm.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gwjuxoolg.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gfmbwfocr.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gswkhnyqf.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gvbdvhfkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gccaubofi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghkkrtxxj.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gbtlkeoyl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gwwgyroui.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gfagpicpk.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gzsgwsvtj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gpospubsw.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gewbyksbd.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gyevdidns.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gqgntlrwo.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gzsgyoapt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gccgndikr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gzdhtakbl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbvrlyyqg.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gjbbuzoxc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjgupdeez.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gsimkjxjo.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gwsmsekbh.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gcunycwon.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gmlnjztho.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gxrpfjuig.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gbwgqxxix.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gszeuyzed.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/ghillulep.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gibhrmlim.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gabeugtzo.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/guytlohps.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gypkryehq.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gecbrvpvi.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gsdntgeov.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/giwrjckbz.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gjfvmaqhe.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gujjcpipn.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/glcxrixat.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gptusuutj.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gaggxhsle.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/geqoputqc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/ggwilcflt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/girdzcnen.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gsssrdkte.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gqvkjsxju.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gcnimapxb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gtghhxvhh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grjlxxqpd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkgnbuonx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glwlsajxl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gdqxfydrx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grwtmmjaa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gotjwiwif.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glqjfftlv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gukutiugg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gvecxxoiv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gpyjkridg.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gyyjlkcla.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gtkrcizxg.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gxbdbueeb.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gxeeexcut.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gmqqorfai.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/grsxhjxqo.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gkryslrfm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gecllmmup.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gzhugumdi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/geomlpbgx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/genyekwqz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gccroqngc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfknuneuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/grgkqeesd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/guoepqrvy.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gehnicsly.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzklxnopt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/grsnxiiof.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gtnyklklk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbqklcrmd.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gvqgdqzly.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gvrkjrean.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gdojiayrx.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gugaptfqs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gwddunmkw.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gwseonrop.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gmyqmmuqb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gknascble.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gujvuqlrx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gfyhdnimq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gexoxtnwk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gtyqcuixx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gtvlkvigd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gqppiftda.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/girjtipwf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/getkkmkye.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gqcmhjfko.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gflsseopb.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gzxxolmca.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gloqbxhrn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbqomsiex.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gkomqbdtt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gmrqyxpmt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/ghiqkoael.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gjrzfkyjd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gzkaxlgdd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/ggwgvpycf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/goeojgrem.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gutymbdzt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gypawtngn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gmrxjqgws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gwgpgzswq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gtiwckuvv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gsowdnvrn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gifvymsky.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzmksncor.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/glxkeukzp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gcluqjazp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gbndzkiza.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/ghbdtczsl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gqlwbegxx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gjwdkcala.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gesfckkhl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gfwarxghg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmqqyixun.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gcixnhjgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghbzuxubi.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdvkmusiv.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gxmflvwhp.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gdonwxwyp.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gxgufgnui.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gsuywpzzi.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gjogepuuu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gimbbvvjq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/ghtdwncbp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ghkzthlev.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gdnzcwsae.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gbpcfuimt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gtcuszuus.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/ghoxuaick.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gwxjljoan.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gbgzbvkmn.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gftnwlgia.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gkkzboejk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gcukffrki.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gsqglvofr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gjnaaajyw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gubyqsheb.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwddnarjd.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grichykbz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grezrgybn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/geqqjzckk.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gxnvaqmjq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gvmoiepbn.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gsyfqjwrc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/ghryxurdm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/glcemfked.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gyvbtbijg.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gmcidrxdi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gubdopodi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gwyorsarr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/ghuvcoutw.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/goyigsehp.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gacafjihn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gfmkfjsiy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdylhbpab.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gztfogpic.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gcuyvalns.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gepcjrgqs.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfwllkolc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/garqxstrh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwejfrsls.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gurexhmdh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gmcpgjerz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gmpplglxb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gbihkccji.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/guxkrokzt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gmzhoretu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gzevvxmlw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gdqvijfjn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gcmrwfidt.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gntxvwsfg.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gtbjqkrbx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/ggtkfbukh.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gxgprvvif.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/ghfwbkyff.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/guaeggiot.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gofybgwzs.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/ggajmpnzb.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gvzddfias.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gaxipfvtb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gblbojorq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gokanegfs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/glgcumnvh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gaoturakh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gawwagkux.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gjhaytsqx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gtasmymxc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/geyxtsdzl.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gilkjqqsm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gndksjgts.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/grlrwnivj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbfeynxko.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdlltmrmb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gheyqzfzv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/ggsuzjvne.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/ggdoctooy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gfognwuqq.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gwshpyyzl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/grxzvjwnc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gzdsslxni.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gwydqabje.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gfmxqxejn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gbdkojbft.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gdbaxoduh.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/ghcmkacun.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfirkpj.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gkwjhaivi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gxmudtjhz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gaswapmue.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gjurxeneq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gzbcmucvd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gsruhaosz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gcdnumekx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gvfgkptoa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/ghbrzybxu.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/guqwxjhmw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gxuaobodf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/ghgdgwgrs.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gynbzckfx.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdqxrfzfb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gtwgyqasi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gvehkmceb.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gopcalaxq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gtwpodrwe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/giagukjzr.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/ghefvnncf.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gdntdelfg.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gzcylckak.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gflifqysc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gkrmckfmk.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gepasorro.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gnpdimlsk.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gtoobrfjk.sHtML


<!-- 参考信息 -->