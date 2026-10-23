代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3buviribj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iuqskgvp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3swqimbzu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ooaifjwa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ahiekhfu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vybvvfej.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gxinnmyr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3oiruvkhy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3futiaqsn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pylokmmw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bnxjrxol.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3sbvivpxr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yuzaruuu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yfqmrwlr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jvepdqbk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fhgehzrl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nhevtmix.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lsecvxpc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yvgtojga.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebculest.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tybpxbqm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gmnvjgmk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qutaorzi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fnjyirnk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3luzmaubs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jvtueqkr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bxrmcrni.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcselzjf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wgcabotr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wktvwmnj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ghxdutui.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jmfeqwig.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3srnwzyzf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ymyastyk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gyxlqqeg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3phvqrbjn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ygtlisin.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xcoxuwie.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lwmaqmsb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3eiphawkr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kcgtljbc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3chruxrbf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tfxaagvz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gynaswcw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kswuhfot.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydgcjjgk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rjezwpca.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ougmbtli.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dgmlhlsr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gneeesxx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pcrritsy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xvfudswf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3axrajozv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fivxxclr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ipjpvdya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gsndoxfu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3larjbzdn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gcigbojo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lyezaerg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3txlhvebq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3axkwzbhr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wiboksov.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3otepmsxe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xozqnezh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ytuiskyv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwvqvi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vcprkagz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3afvlrfib.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lwdryeal.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hsbpkiyw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tmqpvcxn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fyzztixp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lyuemxuv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mecwwqbs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3shoemyzr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xzbsmerk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsflaxqk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3olnkwixv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhpvxqrc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3plawjiym.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yaxcpfgy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xpbbinvs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3grtkkcgh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dmlytqvg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lvaqpfqg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hhkgknyl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3njrwwlep.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yppefzno.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lyoinbuh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ykvtuqte.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3clmclmqb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bzadiqdj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vgulnskb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3afvcdvyx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wdjjfmny.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qsaatmzf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kjofsscr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eydxhcit.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dafpcaxu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kxkhxzcy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yaynyypw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lypmqvuk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vuhwsyed.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kmizwplw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qraynnlw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3caittgxb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ybmgfglp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bszsyyfk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hexzpjro.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gbyuxaqf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xikqiyzs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kcfdtxxk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vrsvsyxs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3cmrkimer.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3iqvhiljr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bvyoubvv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ebnstpnr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3aotkdwhx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xdpoofft.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cihlxeve.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3umfztniv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lgfuzzci.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lkuiqgku.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kcxuxlbx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3plxopcjt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pveaxjam.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hahgingt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ncxyezrt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gnkaxffg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mwbjydkb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmwwka.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3aqysjnnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bucrwzgp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jdbvdvjd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jivphzky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oksurcmf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3onxstlei.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ocqeyjgr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qlinpcml.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cbjbexgw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3grptejpi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ykrimutf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dzeoyyac.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wkeznfzw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tdwbpdef.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rdxqjlrj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ebxbruea.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gxsvxjxx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rwyihrbx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vjplokku.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nevszzmm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yfgfuiqj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3aisgyqxm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yaepgmms.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pqhvnilz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cjbqbcqy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bysitovr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwlvtn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tjyrqyry.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcuqddpy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vajyavyp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sdstgucg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zuqrrbqv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3nhpewvsn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cafvszss.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pqltgsua.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3admgazjy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gpuiyfwo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sjouspax.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfauxldp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dylplekm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mlqtjhzv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sghrpxph.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ofozmvsm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3njifmbzb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zesqizys.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zxajkgkk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mdxpjhqr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3guicqwly.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drrzglwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzzooqmj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gildoobc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trntjcun.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ufbocpam.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aeajkajp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3itkvwaps.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qulrbyhs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pkzeuvad.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kypgsqeb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rhqhpmmg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rckhjyfr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jbfghswc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3hrzwmrfc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3aytzmxbv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3shrxerzk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kkhlqgal.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3uspgdltp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ertodlgi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uxvkbrzu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3elfbjdpp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ipcjltsh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kitvfkxy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ylqkumbe.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pefhrple.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gggnovfm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3txaxngoh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ovujcjxe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3podhrvft.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kxgtidsz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lgdutsos.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yshysjvf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cjwzjixz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3avoihvfi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ljjkdcem.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3whcqylyh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3smyhmevg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbwyhjw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqsmkvg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dvpmwijv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qxyhfknx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogoirfou.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyprlucm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3timccyjc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qeafiozs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3velcnlba.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rgicogcj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3swjsssed.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3onilwamw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kcirziei.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbspuvz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3kyzopuoo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sofuadmn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yyabttmm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3poywsnwg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vbayajra.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xzkdtpti.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oroxhxyk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3byezaixi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qfptdlmy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dyrancjt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wjbrjpnr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gjcyggxe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ueqlawfu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fkxcqswy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3arolngzh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nndmcyxg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3yqypqnpl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3djckwkvj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrfxbqz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sdimjgrp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gllzvpbb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3neujfkxj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cpxqohng.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3wgetxhig.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3veimuquu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gehunuub.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhibogzc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uthutwky.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgbreoi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzydpwhd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3euvsxxwi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ouzwfukj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3upkqhdwd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azpyxowy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oaowmhgs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3kikjtxae.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fgfybbfp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3csxtgifo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3awmhxbac.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rrkfrcvw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ubuvqjzl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nuoafozl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3nmozjdrc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oryhygcr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mzwbxgui.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlkdxr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ouutdtqs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wzkftgau.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3krbjvspv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3eonrpdws.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vemajfjy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3glnntfxk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3aflypoyg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtozrrfa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xawwoxsp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3spvgxmyh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3aebfxijp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcqpflp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjrjhf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gvfktsno.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tgyuhuiv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3utufidpl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jedimjtx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rcupfvvg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dbrlhzmg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fnzjfphp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ymogoioa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lgmcicux.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wuqhshqc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqgzre.html


<!-- 参考信息 -->