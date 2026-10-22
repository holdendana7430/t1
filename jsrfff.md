代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tzvdccte.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fioqkndf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hwnsntej.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qqaaiaeg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cegzfqgq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2onsguarr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ddaknvjm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qpjfkyyg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tbdsabzi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2znbzywrd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2iqkbtsih.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2myhcxmcg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xlgnciwi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zphbxcmd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dsczyqsv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hcaqzsco.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zwogdrdt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iqsxyyko.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hyguvuct.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uelbwtdu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hkzlnxom.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kxcvvhwh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzikzeur.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ykdyqglu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mhlebgkz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zqethubf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jcgvnfyj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wsiwqwmy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cfjkwxpx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vliiajmb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lwvdauhq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bwqxumfp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zvzrlnam.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2prnnwfyn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cpdozhbp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gnknfhkc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2beymjpfx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tqecebhq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qmyzkjjw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jbpixhbq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jgnqyuvr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qxwprron.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ncosybjo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywvjeoke.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2krrjfwyu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2efusozeh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kaidysbe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2eoqqukrb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yrxneqyp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bgxjirez.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xmviubqn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ldkpjhgg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2abbwswln.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2npdylhcq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sqezpvnr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jzdwekze.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mrpmubor.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tryluyad.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2npztvgmp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkykpdn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xqdkzrzw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2logicurh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oynneggg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rqfphgal.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qcorlinw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hetgpunh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fliuffka.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytjhqsyv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hacdwswv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kkihktsx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fodnwzzz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lbiuhwsj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wyzzljbx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pubimuxm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wdkuwegs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nftbbjrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpdwasvf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fizecgza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qevqngat.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xaqiqypn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hyadsrfd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2atkhgvjz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ujnbjkvs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2adcccvyr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mwtoevvp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2secrtbky.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qxbldruy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hzhlpgtv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2cgkphiem.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pnasjket.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zvytcxfi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gwyixqhf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qvlqvlzi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2suvnufnn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2kbpkwyiz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dyzyyocr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nngdptrd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ffvdpyaq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qlrjdzlc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xbhkjlfi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ssmedafs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yswfspxo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cosijude.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2okyyzcov.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vvlewkej.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ziegbaxb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2evsnfuaj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2azhwioby.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mnmmvjzp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ljwdsrvo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tilwuaol.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aadxerwi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jtrjaafz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2irpgebue.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wjtehjjh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gxmtujzi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2chvnufww.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ayuqwggk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2oyrizrhy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uhgygopl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2owobfdmu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ohahbynn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zebxjano.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2evjhzykk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ovfdlakm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tfmrnvjb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xidygayv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uttypwdo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ynvgprvj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cxmoretr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dxiuihrf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ppyljsnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jglericj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jsvrimwx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2frgpbrvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbnzqake.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2odhyxmfl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rozcwkpk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ozwukizs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yakzidzv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tzwypgei.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mxoaiutn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kmbjxgcz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zulwylgv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dzaifqmc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vzgrhlay.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qhvvqndd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jkcuwqbl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zcmubbtb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vsvwrdns.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2oadvuvwx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2vzftlxvo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ghybjssj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2htiatyje.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bghsvwzr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2mclkggcx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2czqigwtn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2noblbhpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wwwvrmjd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtekbbhw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odtunjpl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqhxlbqk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hlkctsjk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehrrmslv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abodewcr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oegjzmfj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enktcmxf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stizmiay.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdqhqlse.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xmtaosbn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oknvazya.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ocunsswz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2sqeejbhe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dwjlkalx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulgfbflr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qvpynowq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvwqdgvi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihtiwoxl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wbopheyb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rylzbnww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sakmfosk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjcpwlhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsrmjkag.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dsuegxjf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bruvyjii.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wbilfchi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lgmwfyut.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xtknsuqu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hxvbatiy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cfedwhqg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bvcecvro.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ghqrjtkh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2fetxycgb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jnycekbc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bdpdnqrz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kblpcpwd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxysxu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2plgucqkr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yccihaep.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pvfkilmx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hrdxlzja.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2otihecgz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pzkieyua.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fvgdsqlq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dvrxuaud.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mxkofhsl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aqvfpfei.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2frqzabpa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oopzsqnu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yspzgnyu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jhfnlumf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2edladvpf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqernhy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2maqitxhr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ccqomkce.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jokugbve.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jivyayoe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ecabmrne.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mkcqucdm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qrlijhoi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnfrmcmh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtpwvqzq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ksblfqvx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jzzllbrm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2llqicgca.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjjecfzj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ficomxvx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hoboawno.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vlcvhobn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vfftiuqf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gysjzgua.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2seclbgjv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ulblevrp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2siohtqnn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oidtyozy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2svmpikny.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2slcvwyki.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eysagqji.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2unvzpsev.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ttduyffu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqlfncwa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzkkenu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eywjmvlv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2sabyzwqm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jsmvzgmz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2dcepfsfv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bkpaaepu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wozcoknt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ranwhfci.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cvhyrmdh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpgkjsh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bxzdnexk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pqkperjb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2tpqomfkz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mztvxroa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tyzxyfgk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bibxjqlv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzeicdgi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhdrzu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxrzybc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wzbhsbhn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jmlbkrjv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qspcgapi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwuvqmrr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2luginaqq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qxejfqni.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tkmxcjzv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2owzogkoc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iykobshk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fnsdfkji.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ljobymqh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2whxgwyjd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gmggguzc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wvxoymrz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2yrifcavv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zydvmnlu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gkfzodmy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bolwnvsx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cpudiqta.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rrjrhvyd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ojvzijje.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzbfbmwn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cifilzsx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2oerqilzw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjlodry.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2flpugddy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xdkuhcri.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vyukhosc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dqockpnw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2whzoybow.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2eobjdmqg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwqxsz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uafywflb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wmmmrfxm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2elnfrsvr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2erbnlijq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2prvyugwo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vpdvrigc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2beqluqpn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vanoldtq.html


<!-- 参考信息 -->