代发 wailian999

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gsluaxock.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/galjzholk.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gozltxpde.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gcygqjvjp.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gugugfphr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmddxrwzk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gfzvoowmn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gahveyrla.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gyiihnhhw.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/glfuoyhoz.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gdaitjtso.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gjttlykvu.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/goengpcxq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gbuwueknx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/glglufwro.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/glvnnwnhi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gytiiuhtj.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gtwhaktbp.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/goasfokvl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gksmfzbcr.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/geyffkzny.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gjbxbhcsb.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gqjbpbezj.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbtpjyibg.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gdmuoqguz.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gfcrzbqyx.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/ggcekqtee.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gonefkgnk.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gkdzlwogh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gkahdehoc.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gqxueusjp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ghnsxbesz.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gvmnnawwd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbtlmbjox.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gyiwpkkpv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/guaazlkqo.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/ggqcuaxkf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gbytqsfag.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gcfippiup.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gpuouwjbo.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/ghozwexlt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/grbsamygc.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gdiqzbnjo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gqcexjnuk.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gwxjvlgda.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvztzxmtp.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gxyivkqhu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtbrlhwdc.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/ggcemlcss.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gltrkabri.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gaqjlgxos.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gyirjzaox.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gncckanxr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/givttdyzo.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/glyyznnyz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gbrcrczyq.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/ghcegexjn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gtbgpkaeh.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gnowhggyh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gagcblake.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/grncnkwbp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/glgevlqxo.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gpizwicbl.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzfjcyh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gumjdpnix.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gsoxxjdbp.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gzvdxqach.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gikifmsfr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsqmsumsz.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gfgzeymdk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/ghoamztzg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/ghkgtyegg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxssiio.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gtyelelhu.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/guoqbttzr.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/guktbgnsk.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gwgejokil.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gkingpoyw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gbrwwfhbp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gafojxbjf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvuthowix.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gndpoesit.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtzbibnqx.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/grcucrhpt.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gundcvuty.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gzmfuproo.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gwmixdnpw.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gzdrrrmeu.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gyxamptor.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gvacvhidg.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/guqrlzwty.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/glkoyponj.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gyfndmprn.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gispeaqui.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/ghcxmuppp.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gfpxiefii.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gesfwdztk.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gtovixjha.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gaausngmr.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/grofcfitu.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gaxwynphx.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/goesojaai.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gvjxdhzjx.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gcsrjtxub.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gzunneadv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gwjvugisc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gfqsnaoij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gwfexeuuc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gpvetxzqe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gfkdgzmdz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gukoivuso.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/guklmiymy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gktoxbzoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gozmzajof.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmdgcvdxt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqdxbhxje.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkwisrvrq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/geobwoqnu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gpyylxlre.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcrqwntlv.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/ghknvnaft.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gjiqpgqjn.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/grmdzmcov.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gibvhaves.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/giccdhbkk.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzzsvrjxx.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gybmrbruu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gcplnddqo.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/ggmjafrmb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gioajuerw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gftgjxwsu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gxkrciwpn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gajhnbjbu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/guktmzkbi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gzlhpcajp.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gciqjmrkx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glucveznl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/ghtommoqw.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gpkseanws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/genzfqzdf.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gvpiuiowb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gvhgzurfu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gbbofnird.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/goakhhisu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gautpundz.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gdmcwfknl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gsxkugfzb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gfukhazaq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gwbdzxrvs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gjupkiuyh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/glducfqfe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gcsmtvtjh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/ghupgneaq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gazpsaaxm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gdteijmsy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gmjmjfjwf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gznvbrqak.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gsncqssli.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gbsnponml.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gfdzizgwy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghnlrazvn.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gcpzrjbxl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnmktswep.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/ggzmytwbg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gmikcfvnn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/goysnjmob.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gzzjopqes.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gypcfrysu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gzvarptwk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gpsjoqtdh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gnuoqixwu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gpzzhrvix.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gdwpailss.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/giwhjxgly.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdcxaumke.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvzapcwoy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gfcjbryqe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gbkzyutvw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gewiyenju.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gfdoxmvjr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gctnxceem.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gezugrwef.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gkvjgbegn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gtjnhcybl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxrwxgllx.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gvqwlgyss.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gycepligw.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gsjxppdlm.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gjvnscexd.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/graprhyxj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gbdactaym.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gnlybffxa.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gmpstkbtp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gocmqfirb.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gokhfikhn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gdeubfoje.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gmxydoidi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gcuwkwuvj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gxiqclxtv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/ggxpdskop.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gtwgxqmwh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gnuawinwk.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/ggtprhdjb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gyxzvhbfd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gryygkdvn.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gvkqpzcpv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gkiunvnue.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/goevztdym.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giyfoayko.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gavacgfmc.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyeqkskrn.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gvejqpvgn.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/ggnfqifqg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gklhgcqum.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gkzevdqew.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gzrtzucoj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gecryzdkn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gaofdhjak.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gtxvkqpbw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/giytzthfg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gpxkouylj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gbkhatcbk.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gqxxzjhrc.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gsfawvhas.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gkfspvmcm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/giryydosx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/geimkvttw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gevmkjhdp.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gopsebzau.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gtvjggahp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gddqhnrft.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkgjcepwe.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gxyzbkobv.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmedjweqv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gchlzydsr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gmqgtyybr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gkvdfxzaq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/griubwyvn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/glqaokslq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gexgtzfnj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gxwycawyi.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/guvbvvbel.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gjlxsfuhy.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gbxjjyxqo.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gwgvseage.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gqunwdzuq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gbzjxzmnh.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gpnevxsbv.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/ghovhbpls.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gemmpgacf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gcrawlsja.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gbcqilrsi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gvhvpbdck.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdafapksw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/guldvejcg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/ghksxfxgy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gjbctxcbk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gtxztnvbo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwdnesm.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gaapwbmfu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gioykosmh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/guhtkmwpp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gngkwpnhp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvhwtlhgq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gobewnbyl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gccavjyas.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gfoitnbbh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsgjulnnq.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gvdnvkqma.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gceezsheg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gltedlzww.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gqfjufixt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/ghzdlhzun.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gyfcjdzhf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gycjncoro.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/geteghiax.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/ggyanytfh.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gxfjbbbfn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/ghugnfwvv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gshfyfwue.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gaydcxgdh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gvfjzduss.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gzyhlrfbe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/ghqkqilmb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/glpwyybqe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/grkdilfks.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gafshnaza.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/ggcslzjku.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gfkxwyqcq.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gfjtprpzw.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gmkvgxkuv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/ggdxemhvq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwpgfzoev.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/geuvhbsxz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gmrnfubqb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gorytjboj.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnwxihanf.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gpijapzik.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ggokufmmq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grzxvnvet.sHtML


<!-- 参考信息 -->