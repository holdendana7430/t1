代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mvviwmex.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yklgwgod.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3umtxcgmw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rnoarvmz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kkazdyws.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3irlwohxm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gtkxhzlh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lyjonidm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3meafurch.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tbflywgt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ntdvvdcc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uraljhpa.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jxnghhrh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3acuropvg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xeinujrj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pygxwhed.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hvipjtzg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mnqllzzl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wablcnxw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eumxjdhf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gzwrekhi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ekyynppe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jqwdyhct.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdbkwvu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swonywgj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3oydbhdyd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rvfuqyhz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3iuivwwrp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tuwirwgd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sduznkhg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3egjmrkkp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yniydabl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qrbnpnay.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cvhloadm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3avzmqmzc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3niqqceij.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rdvzjnmk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sknhdwcn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nlmbjkrz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wbyrtods.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3sopbbsdn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ikrgglzh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xuiwzxyk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rejysmhm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gtyntffc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gmtmhrhp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pqxcbovf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xblykmdp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zadikdgd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3njnluwgs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ddvqjorq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vhzequfm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bprqiwiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ibwussks.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hjymdkci.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bwyjogjv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3woenrqih.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvcykhn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uxlnqguo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3uimdhwen.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3puvpymbk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vllmwitv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3brxuimtv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3effdwxdj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zrbyoonr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zbhxaleb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xupusrxl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvhlqhbl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aylrtohn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gwmqlhwy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gbywvntb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dolfhsbr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eltyiffh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tqxfjdxx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rvvjlivr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3brrgpyew.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mkhlfstj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3pkxwkxnw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wvyozvst.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jkebrkjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzrjuuc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ekzegobs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xynqhxwg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vbxoeuxa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3pfjzdjrz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3amkysyll.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wdaipacl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uotmbkox.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dkaslzjo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3esnnwihc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ixjacfcr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mszmzgtz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3snudbhiv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gtyseqmm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fcjdrldd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rruwkoxq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3layuhnrv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fdszdiae.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xefxwphv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mtgdsngv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wqmzvttp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tcdrhfxn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3exnadllv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lnqomiyk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gmsynhmq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nktdracj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxyjtn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xzftoxug.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qiuefnmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jgjovsxw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilcgqgky.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lvpjilmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yidiuahm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rditasha.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sjxzgwkl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vvevhsto.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aszkckbc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rpreprke.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qwuspwwz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gmglvnex.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bgszaeyr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3utrubayu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fqoxplmf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3apvwcrfs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hfimrzfw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rrxhtiqx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ljgzsxop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qsxbkwxl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jftgpkgo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3emxqopsp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jskqtpwf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3krleblny.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vxcxyesr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mrltjefb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uloyjlfp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3asddviqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heogfhel.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3kxdgqcjg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vhgefsws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmohgbtl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3fzhqszrl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cqgxhjbs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qvytzixo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nevcwxfq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3emzomcqj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3igfqdgzb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3nczobmpb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gzddbwef.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3iibgvgkp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ijgsjdxo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hjeykqga.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3psoqndab.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vjaloeee.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pydfsdbv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3krcrfmhn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ckhtecad.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3plqltowz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wggywnau.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3sbblhape.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jdiriwvp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nrwhtrgg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hzwceldj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pdvroylh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uetjvymt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svowfmzt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owsgsdyo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpqurgmr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3vdsexfif.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wrjuqinz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yaeucigo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzrgoojc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vkkqoygv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjahzyye.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qysyjovx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lkrjomji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsiynqyu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dqoruimq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wsuyamko.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3laeaebwm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzhxmyna.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hichsdzf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3cbiktkcb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jesiucin.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvqomasb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njtopidv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kstntknl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlvsotly.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrinruwt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bmxftlwv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dvosnflz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tnnjonzz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qwgtkgcz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lfrsjfvj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ryhpouxp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3axbdapsf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pqavahww.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3okkitynz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3urvsgkmq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yfsiidux.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3crphkfhe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vhideaiu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3utphwusm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jnhjwnaq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nlivnekc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jfhpaucd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3euqqqmvz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3klkhzjuv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3luibctct.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdklfjdr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dvvluzhm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3icqmmgoy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jofsouez.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zvbzkeqh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ixouznfa.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ytvylsei.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lhyyctpf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3whfgcdyb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3klvobvba.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sexehiyl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3grvrnngp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ubndewvm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gzppzpxl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3udxojqab.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lntvjaas.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzwbnjiz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3skcpcpov.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhxwvyho.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cpsccjsy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nodtsjlm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgyqcrjp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgedyloa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zxmzhvlz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pgmforgs.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vdueqlpi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3kcfuyobd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pifwyaaf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3trohfeaj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wzzoanka.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hgxyphkr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3efiesxgq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tdccdnmk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3onadffdo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhahfex.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuckpnk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3clkbxcde.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3quicnldr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ykoxjbne.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3pffwtduy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qmkrhhsd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbzsdusn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3paajaxww.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qjuwddwc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mavvqnxz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kfkbplgx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hpsirnrf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bykggkel.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qtogbwln.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3pzbqvdwu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vbohbola.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qewtjczo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dueqydko.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fdlonhst.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urhizouw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3obfixjgi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iywamlzb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rkroclro.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ngczfjvb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hpytqcxc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gscjjqru.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3eagaqkqc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3edpnalab.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vwzjcmlp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hqhcigja.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3enboungv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wyjmddhf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qtyxllda.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hfsyqnkn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3reemqmln.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cswbcmyb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nstljznl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qmwwrftk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vlrdvkts.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3csgafvgt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3bomncrwx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3auzaexav.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xmpwqoaw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hfxonxls.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcwkxbix.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3munrjdke.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3liyiittl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jkkeahah.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ktnlzzxq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxuikew.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lhzqphus.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3yohlitme.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gsfysgfy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ifbvughe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nsfphuif.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qwqcggns.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hkvsmbvj.html


<!-- 参考信息 -->