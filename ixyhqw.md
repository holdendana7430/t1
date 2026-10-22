代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ryawfdqc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ldsoctpk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2byjsefpu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lquwwpfo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2drnskfyi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2edwbajmm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vamumtma.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dilvntma.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rozoqgzv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2issehuot.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dgkdfvxq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pfofeiht.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gwklspzs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vmcjfahd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ewsdzkat.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rjalmuyl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lbyxuqfn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nebrpijf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xvnvajav.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2msxaxydb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbeomjha.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2rkadcpsp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjqnlfkb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kwohvqce.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hlkughha.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2foekevvz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2peuqvufj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aqawcvxt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pypeoclv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zttfclgi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ubbsvzlu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2aoigihuo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mldfbwqd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2swuwhqme.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lxequbpf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ttfohpsr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pklmvzof.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qgvqfutg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2khreedro.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mseiizxc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xhxnbdjc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jwvrctpb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nguywtfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lwjbgngh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gufwecmr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2shmaootl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tqhvhlvx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hpqxoeby.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rfpdvuog.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kyhbiser.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rbahzjei.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yetjxnmb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2finwhtuu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ebluhrws.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2psnljxne.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hqyavjtw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rotwevpr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wgrcfgmg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vysfjafo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hrkemyri.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qhaagyuh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2thiaqlmr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahfebhjp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ijuanpum.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfxuim.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wnslurla.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rjfwuirj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvdjbe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ynwjtdnl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nhwlyita.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pbqpatjs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2beeuxlat.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pbavceaz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mxyhpcxg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hbgpjnav.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ptlcjtgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxqjhswn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gtdlttfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgwmwaqd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lbjfapaz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mkuawxeo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qsvjqidx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2owdbenfn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2divvsvmd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlzawb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rzwwkcdt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bgjcdkuf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2awzwxwww.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rouspvfq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rkcgbzib.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2podygica.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kaebdyci.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uzabogqq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ujzjczrc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ocdrcfjs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xoanwrxj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rtjpbtzq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qsbkcxib.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zvqatowr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sqpbccrr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ofieanhp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lfxeaywr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ontpjfol.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2oltnfect.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ncigsckb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jlzojuin.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wzklswbb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nhbsmwop.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xipynywe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dbroonxv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mhxmgcvi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qxbpuuzh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tosvxuwm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jrmtrvyq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bihgmolz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cndwsdbl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2npxrvfvc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2glgdkips.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2syglwogh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zbdeczkj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2uevmgfrl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxdtwpov.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ljloquvh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hgondhxy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jqxyulgt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pynidrhe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cunhtikb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2akwocwlc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vzdwzmcn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2eqpgohkv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2raodwdok.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hxebycsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdewvjgs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jmeubtrn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nunwfmqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xevrpsqd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xcbifhum.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lkdrwyqn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2amrcgmtd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2agsmfwun.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2aoaqqpml.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jetucqrb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ixkvtkxo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ftzsbvdg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ymlnbkqc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2twuvchfl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qjfczron.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2bomygluq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2crqffmpc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjvtat.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2blxsnhcj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tizasoyd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kpltqnxv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qjsfesiv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jtucolpx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2rirzbvpk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2urzfgazs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kyivmujl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pauwmdle.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2trhobnhs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2haimtxyg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyhrqvvy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2autdwilj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfiysxze.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2elqnhzgr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vpqguyzv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2naiqyxzo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvrcbmum.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gpnlmcqs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oadhctgt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bfiluafy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2omhirsjh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nlztlvqp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zkqudndb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrfyoiuy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qryfqbdf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qpqkxrva.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2foptlwuz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2opysmggn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2favnczzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmmypxgk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvughcwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekwdcfzi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2czookxzv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2snrdfehq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tlpvvbol.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2loszicxd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qvhpymcx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xieqwbkb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2phntvybs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ipoqfdzf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iabezbpw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2yuxsvhnb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cmrqzkkj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xsmfpjth.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2myzzeiea.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tmkkjbiz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ntcrljhp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vgxsghpd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pgylifhr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrhxlns.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pussbmim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2hxeacuie.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pfeixrzx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2savsakjd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmzwmzaw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sawgvtzd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vfccludn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2savvvzgn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wajiybuy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rdpofwjb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2honicofj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zdmshhew.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hcmusfao.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ynpxihtz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kbcalasf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tpbbngbf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2vfolxwpr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2bwqcolin.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jjxxftjq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxkgdmya.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2buobfgjz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wuvcmyjq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hxacwdys.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2babnhzcg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxegzjjp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rhtnfvia.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oqzlgfai.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mtujaexk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yqwffxtt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2olhegxhe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mkbmsdcd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ezrdqgka.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2agfdpimm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hkullvkf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ffamdhrd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iypnnvfs.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2okkerody.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fmkohjux.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjbbned.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owawjugy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qqilzuio.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdtrrpr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yzphfcld.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cxopxpvg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2utvjimmd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pgqhhhgd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2opmycgrn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2loscdscu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yopnizef.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2lyuesurk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ckicasdk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2myuajryy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2hsepakqo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hqigsbjn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pbuyqssh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkafzuy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gppoumzp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffblptpg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yonylzey.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alhevfum.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bollcoyp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bbhjphtv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tetduxrq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cxmzwoir.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rirvnhvn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xqoamldj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vphqaoko.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2grnygcyx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwauzhmu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qiapowub.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2uvrcvrbv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2eyyzisyk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2caznlllg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ixouxoyi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cqtpkvxl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zidutcjd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nmkmftnf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hneeglee.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ndnyqnur.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xeybcclp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmdrth.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vbhkusds.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pvkhzwxg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2uqxhzxcj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ttuhbgos.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2frjyoefe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2oswyunic.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ytlirxno.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hwjmqxcd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2utcelacb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fagrqvfu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2govxtuer.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dgthnuwy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mogjukma.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xfbznpxc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zvtrjuid.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vkynxzys.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gxhhzdqc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rrlfvahf.html


<!-- 参考信息 -->