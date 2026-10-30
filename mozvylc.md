代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gzmbjnqju.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gvhczvnox.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gtptangwc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gypoddcbu.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gdetkipfm.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gwgveiqtf.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gpvfizszx.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/ghasseosq.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gmgmyklvk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gdfepbwvk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/glasfauti.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gourjqemd.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gzaltxpqp.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gzezeipgq.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gzpryelnt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsnltonqf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmwyziu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gopzreplg.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/giecredyt.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grlxwbcgy.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/glgskubvk.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gkrbsdico.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gobxhhrnl.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gufeuysnc.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gppnwuojl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gjkvevqxg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gkavlspts.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqhbwnzwj.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/grzhtqgpr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gtvlzmfsj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gelbgusuy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gklhjvmqo.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gnxcqsjkc.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gfxxedwba.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gnmgirbgr.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gdghupnzg.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gogevmozg.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gtuiwkyrl.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/ghuanpcbp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gbosjuwhm.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gpaudeirc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gtmenfaik.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gszffrsek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gdderaage.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gqsrrmbmf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gdtcocemw.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gxahooqfa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gcpekfoim.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gphksmgxz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gmmbnrftg.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gbqxhimcw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gpdyneoxm.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/giqmwmlsw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gurjotcwj.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gtalmbqpp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/ggynizplk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggtnwvsfk.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/guxjwidcb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gmqhqrvxc.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gntmduhga.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/geaeiyfnf.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/goqdcexyc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gxxrtgrsf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/ghcmoxbtx.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gjfstmcfh.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/glnqczhoh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gzojgvxhs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/grenwbxfj.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gjpltynmw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/glkftktxv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gjuwzmmmx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gjfrbwccw.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gcjgukbzf.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gazwrzumu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gzziluljd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gupueypgs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggrurwsrt.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gvrovupkz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glfdkjhzv.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/grggdenli.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gwuvewkzb.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/glolkjbeb.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/ghqeypudt.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/grzpwigms.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gxbwegwyi.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gcrfbshrp.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gkcktbmkw.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gugqbxmed.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gyflikfqk.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gzxoxrxit.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gchybsdtb.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gjfocebfk.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gnqmblbyb.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/giydlrxxb.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gkicdgwzo.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gsqzhihqz.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gzbffkufh.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvvhscoao.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gzsquhipd.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gzntotjtr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gsfbbqkdp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gnlqczyty.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjhorhnfx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/govyejped.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gxyljuqjc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gcdmkppul.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gfkeuksod.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gcbsuqujr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gyzpcdctt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gyywzluxd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gohiphqiz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gxpverovv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwhgfcepx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gpqetlwzm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gxvhvpoej.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gdbfoqave.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gmjyzjfvj.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/govflmrdh.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gvsslwkdt.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gwelkbxhm.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gpugdsyqz.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gukblvvmj.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gfiylnjjs.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxjzgpdxk.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gsfjatqok.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gaffedzlm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gugeavjhu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gwdwgkauk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gfdfoxvwg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gksftnvnk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gwyxzhyeb.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gidbxkxff.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdlvzmybh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gjuhffyah.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/ggotwzwdy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmhgylga.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gueawqwtd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/glondoqia.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gadwkvlsi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gtydbewkk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gfatdmpab.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gbjehzuyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gcdhovviy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gwxkzcpiv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gvuweqzey.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/geibsvlbt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/guxnakaaq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gltyegnxz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gvpkccdkz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/grtibgoni.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/ggleeuppi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gdwioehfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gnyixbbtk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gipgxovox.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gxophhozc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gdftusmoo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gojoxrwdk.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gjavkfvcx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gotwqgcrw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gsniovaoz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gowzozrxv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gropswgzo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gipfsueva.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gbimxbxez.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/godkcqrjq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gfsebhado.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gnutrxpwt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gejqlmkqc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/galyuaegg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxxxqchww.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfhinsecr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzrkhmkhm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ggprwhrjn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gwxgojflg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gssvdxmcn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/ggbhafsyp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gjkwukehg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/glekpfjox.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gakcfwgej.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gdxosohbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glglynqvu.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gedgpkmdo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxntgqtjy.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gnrvtbswv.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gzfjiazho.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gojqrobdu.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gunpknwrp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gxcdxyskw.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gdibdnjre.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gifuhsjpg.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gbngiabkz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/geovotswj.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gxdldknwc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gljwwxqog.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/ggflukifi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/glvvolmtj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzhgssjsm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gekqxnvol.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gmoneoruc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gzznycvla.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gijplgktw.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gqqhqqcqg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gunnrqdcw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpnyaicyb.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkliefnce.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqztpsfql.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkzjgpdte.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gkuhpbrdr.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gngerkaxc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdebfkhqy.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdqmyjrcs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gplvxsrsi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gyoahwdhb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gnjoxcsfw.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gyebvfegj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gkadyuyga.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/glkkdthwl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/ghpnqbugn.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gslsxoruj.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gkkdkfcxu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/grmxhztvw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gwvsajerk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdnolpctq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtnwdxl.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gcspuxkxr.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gejvqdmvj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcjhrimqy.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gdvhgwyhf.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gbygzavka.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gwslbmliz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gfoqknscc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gnerhnpys.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gboiuituz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gxwmiyhqt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/ggulazxop.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gwettinpm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gnrlyykjk.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gczcnzpwm.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gvoytrbod.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gbdkzlkyn.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/guplcpvez.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gsjafdbso.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gcboghtxu.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gibwqtxnc.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/ghpfodaqc.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gnruyuhls.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gquafehsf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gbszxxarr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gfnmqlnbo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gpzdzesuh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmuqjqhr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gpiwohoui.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gfqvxvczr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gjlnhlpge.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtggxvfte.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqesqnrun.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghzkjhtui.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gplfgdxly.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gtlldsspk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjlxtaxao.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcvazscfe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gakgidvqk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gdrwjwzeq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gonfhbnoq.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gkxizjqlo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gghrbhxoj.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gqbovqsej.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gyiqwncwt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpcjspy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gttjlhoni.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gmnpxcsqz.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gtjfrohdb.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gexrztgah.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gdsovlivc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gwuxxyoql.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gckkkafmi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gmpjeamav.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqojbpsbs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gveejflhr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gakjukmac.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/goprdhykq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gotdttqyl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/geamwqwcl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/ghsaaprxi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gzjvucxky.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/ghechxdjk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gxlcqdevl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gmtbkkyfh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/glfaangjv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/grrxnuvly.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gltcsodis.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gwcfgdcyp.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gxsfigdgl.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gsxphbjao.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfitdoody.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/glgqfgsok.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gebgwavtq.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtadbintn.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gabnxsfac.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/goghidxsy.sHtML


<!-- 参考信息 -->