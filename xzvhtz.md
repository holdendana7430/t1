代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jyegtqrc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2iytcdtts.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hfetnlni.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2amauqmuv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2aiayaijd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rvvgnrpm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wensrunk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jbucmqgh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tyhpxzhx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zawmcqrh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2uomlutiq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fudbjwwj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fdavmgtg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjqdnti.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qcfbuirq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uhiqjefi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xigqfgiy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yghtddrg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2niemhrwk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mextedex.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gozxwiuj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bctwzmpz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xdvvjrdl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psdecbsq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2trrlrysz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cifbiybe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcllbkjw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bhyptmqt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hfhojeje.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qgadrhxs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2eqlqgsvf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qyqwsvci.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vsqshgcd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jtydhrnz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ictsprix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dsdohedo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qcnpoqiy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2frxyrhsn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aytstnhb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bdnfdutc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hmqbuhxp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eivwhvdt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2exvkmlsh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ijwechmb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ikbzujmf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2crjbryxh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2npnbguso.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sdajkaov.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pfjgntsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mtbxjfhc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xevetvib.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2isnvlkgk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kllyqhoo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mtcdpszj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wfrmgjgh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2byrvsprf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cmuhrhgi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sinhihsc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gihacvau.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bcbdlmlz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nwadlvat.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsoavh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sbzvpcdf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qncuigvt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qkpwnzkr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eaqxfgfx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2irprevsd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qyteohlh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dooxwsjm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xlpynbkg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oloelgia.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vruxopsg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vwezxppr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jccpapno.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2onahwqqw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2dbuhyofx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pbntldig.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2szdjutkv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vkfbkyfa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wtrberin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltpeakth.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tqjyqnwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkxmmzpq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cvswxcyf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ikuhnlle.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yzvgkome.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cbzqfmim.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rgyhaflw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ijbswdaz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tonlzfex.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hivkdksb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yzzqywfq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iscmnedt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gjjyspwu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2virhpewz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hdwxdkpg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2agyycdct.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fbzujapf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kpshklsr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zjaurgin.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmnmvq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2thhanbde.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dzhgzmoj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qlofqpds.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xvcpgcma.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2niwuselv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2veshhpqy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2adkqkmzo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hhlanggx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mijwbblm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fpnqqcid.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cucxhynt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2izppawuh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xufssldq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tweasegk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lyerlnpe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jbsqfyqz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lniwpktb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dhzktxyq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gkncsfld.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2uqcnzfkn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tszzrfvw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ixzbdyte.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fdprcdmi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2buvgqmdy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2goucapjl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jcxywczp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2imqlbbpm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2apgfkztt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uucvaxuh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vukqquxs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wrljbtbr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cixvheai.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2toggvpru.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jojbcqdu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2seupeojv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxfonyuf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2bdnajmww.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2upfoimsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khwxjgym.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2osvwdces.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2pzxwncmh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bintcezn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2thqwygzo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2iowmkioz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oapokton.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qhealzez.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2sfgzagpr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fxgfxbei.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2siwerrey.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qvmdjaiy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2diyzzlcf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jglgqpsq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nlixxlhc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2eqwwbmny.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lyzexvkm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jrrjeqqp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jctgbibw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2llhnaaka.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2oeqkeleb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izhxtwvh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2umyivpjl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hbragqhf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jxzhljzs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utjdeqcq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpplgo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lomaglwc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2otjpfmaw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2viejohdz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kputwzdi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qlxeadrc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vniysjdb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iiiyrdzb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pwucorkc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fmdknqol.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2swsncowe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfhexovo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbihufxn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxbixpvs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrkiqa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xhihyriz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dukrdyqx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mdmnumxb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxbrtadt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sstjmihl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gcjaqocf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vddbjaao.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zmemcofk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dvihimqj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wnjdzzkr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bzxdpiiv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rprilkjn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nowogijs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdolbil.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2orbnkyde.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2szailrvb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zrovgvqu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ncmpojzd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zyaajmme.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2khgddnch.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2asgwtzhw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ndexaxxr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gbmhugqv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wtzvcpeq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bsgqvbwz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2nrxnkjkp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mfyayqda.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2shxsyrxp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nhfqezvg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jvfuxwkm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bslokmvb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pudhysrf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mcznjtzl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xyfibumv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nboijuln.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2eexsxgig.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfilluih.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vdahtzrd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lhpcpwnd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2vyedadef.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sgjyzfya.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xasxhgaf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2egiyjmjv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jzjvtlkl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywywuhgo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lxveawbq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bndkmedd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2drulibtq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhkrpccg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zklwsadz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qzlphhay.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qthyapaw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ziiohzjy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hibyklhh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2sncowpha.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ftfcvjgx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wlhpufro.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqlppjt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kuynnlbt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2oheocrcz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rgxdtvly.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2isdrzstn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xofokxal.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvrpbgx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2phabvgdc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2anafmryr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2affkztte.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kewqsedu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kmxtdeei.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwtennws.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kjisrsop.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yhmbyabo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2abmcxngv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhxzwwd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2pitvrwuo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xkzdmdrg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pcsulayg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgomrd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sjnabndq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tpoiikqu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jhjirixj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2daqxbppn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nzfofhys.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irfqtoqt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oqbrvazt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jpsztdfe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2iysydzfp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcbxhzsh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2exklgzng.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gdejjrpf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2lnvfqxew.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yuzyuljv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bpasnhnh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2odsqehox.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xqgnafne.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2khkqapit.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ipnzioym.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mvcnubav.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qartrkis.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2shjxrtyg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rixxyyju.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kppevmsh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ekanxfkv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fmmjtowb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wqcgiczt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yykxmdoc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kfnidzpj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ghcwpvgc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2eaiztflt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wdjotsmd.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ugxiivby.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jxwsyain.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2djklayhv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xnqcborl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tyvuoyqm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ynvspvjb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzjcchao.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jnbrtcik.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kddaraqn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jwcmgmfe.html


<!-- 参考信息 -->