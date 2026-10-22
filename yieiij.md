代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sdbicqlx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qgupgjqv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jeesujyy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xalxdmga.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jolsifob.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2obqgxuum.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bpnrsfnb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2znenufwe.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nbgvevai.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kmyoieke.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jqlewkvo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2axrnbnon.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lokbnfxj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2frrbkslz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pwxkzmyx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jczuelah.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zoktdlfd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kwwzdgtd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jggdsjai.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpafol.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ifykuezx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2iqnnokgl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2veawmnds.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nntxcizz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wejdsstz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gmraptnj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kajiscfz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hjrbibim.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lcategwk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qehckxoi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2phcboctq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zrhkyzjl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zqunejrk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ezzgzwif.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mzmmrlok.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tpgpjokf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gxnyqqwq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vmdsncsh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2stifsmzh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2djmwqibe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pfiyphuy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2deeiclnc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nuhnpivb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wvaoxsrz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vikaebee.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2erwqkfud.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gctvnykn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qleegtaa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2inxvgwcp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qeqpuqvk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pioyhuwt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fhaahpgh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pgyaknet.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxpxdoq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xlujevey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qwzpideu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fboqkwce.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pyocsgnw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fpnwjesf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2duniramu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zsifmjsz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pqznnqcf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2oxnwqfow.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iatlkvap.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cjvoyuzb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cbecpwsp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2uvszjwij.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2krdponpb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sebtqmue.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uqwvoyoa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mwgnyfue.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2naupklkv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ndwktkoc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hcbbkxwa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tuaebjft.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wulocwod.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lkedudxz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wyrrvnlb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zkmewsyc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ftpyzbev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opbosmla.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xogbjdgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jawnjujs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vcmjcozn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2akuxqxsk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qqbplayq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xgnfqokr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gqmfamqs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ffayobgf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sxpqqbcc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xvwszvak.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2utqwmmmg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uyryavbd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gsgwkpez.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uotnownl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2iioatplb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vvhjnczk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vwmsopxp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvbqhjcr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ljjmvlba.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ylunlsfl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rddvtkdy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2audirtlo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uubozoie.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sxibybrj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dorvsnxg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2timxsefp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2czlwqcws.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2evieyjqn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tfrdqsmw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hkgdxval.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxewad.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2imcrbwhf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mugdzjee.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ldaqcnsz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pofaoscm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2quaaxtrt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2efyslozx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ggmfuqng.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fnifawec.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fonzkabt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hzvblsme.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ijehbpfe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zufbshhu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ueteqfxn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oaecbycr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yvvhldjo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgbrls.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ezywkhyf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fcjdfadl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cunvlamr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vbujwhqk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xnkpdpot.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2undresoo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qxxsuvfk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2izbbcbfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpuphsnq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2okxoqzhr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xotirupa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luninopt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2muhiwfum.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2errgjhah.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2duftehkl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ktsgltsd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zrhenjqp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2clolhatj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hjpsdiwk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2exnonmbj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2uedmjzcz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qubtrgnb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qxuyarav.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ijclskrx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vsaxxtky.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hqqjetqs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2utmyxxkj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tyyyqzrk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2htiihnxh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gkmsnmsj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nbycwpcj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tvmybpzu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2slpfttbx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2myvrttjf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2spvzpdjg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2znchdqwu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2unbyyhgb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjkuxkft.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sjcixlne.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvkhrcaf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2roleooas.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cabpyfec.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zbfppixk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nezcivdy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2artxhort.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tqzntiwq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tcqlwuhe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2prhovwya.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnkyrqkc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbnhwcmv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kjxrghdw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ttofzpyk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pvjzozie.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzlfpqge.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dfhtyerc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwfatbfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spdfnshx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lggqrekl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gygblwjd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mpgmhikd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xjahikke.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hfmiolqz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2crirsxil.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qzesjknv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hxwjcwhz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2oukbkeeo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2khyhkaja.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nuxvzeaz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pyeicfys.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pvgnvnbl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xomeevha.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hvtkqnof.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ewatxgqt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2chhjfvlw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xcdtzmaa.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2agypnqnu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2adgjptpi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2tfzuokmr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dvfuctsm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2giilhyas.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2levclsgy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bqztikwa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jcwixekv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nzqiwahb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aozfqgeu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wxicimsb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bxarhzjb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2irwbfaki.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ricnmmdj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gcnxgovp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dxktbfkb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fmxlemkf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yhpwnmai.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rweqfmzd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ckbxbagt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2norvhtbt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2izayhkvk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2beuxvvqt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnacjiid.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2orbyusje.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkqpbkuz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2znyqeapy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zuegosoi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gmmbwrsf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yzfpdtcw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fuwposqd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ngkqzjyu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dycbmwju.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lpyqdpxq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yhtmtbhj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxolmlr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pdjffrhn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aqxyrznm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipfsyfei.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2izqauqok.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zxjqroqc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dvqzzhpj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzkhedz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2czbddogp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kyhuzuof.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kufjqsno.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztbtofei.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kwfqhaeo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ethybluk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2efovkcuc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2njhndsjv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhugjvt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cqlkicgi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2solxyfdw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jgvqyexa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ffguxsdj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gfhdrdjq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvdtoryn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jyehwwoy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvktfzhs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akdptvii.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbhbjocy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bjdaysvx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wbofvcsw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trvapjrf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2thawkmau.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2czxgxcwu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2alpwzyqo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsgsoilk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hovujdan.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jcwouehe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ngtyujns.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nqgeoczt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2dcucssxh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vynioqfc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ooicgixs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pbosfnox.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wkfhenbc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xtnecpau.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mssenvhm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtrfvm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2htxsrvua.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ezdfegfb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pjkkfcix.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2aeoxekoh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wwpekttc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2edsxiibu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2waerqrzi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zxssutrr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rsgrutab.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2numduiti.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vmxkszot.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2buhyssmm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmozfwvv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zspkksno.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2juxjhyps.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjkqyr.html


<!-- 参考信息 -->