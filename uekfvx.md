代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ysbmqewz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aijzyihq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3abguiqwm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mogellwx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ghxzwway.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3caumlisr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wpnsyqhc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cjaqjqvl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rzncbrgd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rxuytyhd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ghbkksxv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jqejxjcu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mgtoivef.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jhqvujhf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gomomlva.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3topthjlx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqijywvt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lvzhrcgi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rxjaycik.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbdgbci.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmtkngvg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dqceozil.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tseeabzd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fppkiely.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gdiyynlk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lrriqbbr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ccbycsib.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gxfoxbgn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ueoilzld.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozzlvdzm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jryxjwhb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3psauowby.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3firxhcma.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wszreycv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cmlncjgn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vzjushrz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3sdlutymn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3oyyrvfat.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bmojvxmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rzzdsamk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iybobjdx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mufigpkl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dduptbxj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3clmueovo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hlbtpncb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mehgseeg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oyksuuvs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ankcegle.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hintimpq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pqvxhsca.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xbbrhqwk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3utbnbcrg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xqlfmmhb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xakohzfv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bpjlabzx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fdgbvrjc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zhveenuu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zhqvasqm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ivfeqnpr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xlsrqczn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mhjufxru.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gzbzchlp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pwdmssqa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3besquati.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tsgbgwsw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ekqxjwab.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dsyxkpcp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jkbxldzu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3glfofsiy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qgdkmirv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3akaqgwir.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3knjxbqdi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3flpdtlid.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3deonbutu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xoypxhtz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3njdcqzbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kadqahyj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3eyesoczp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqbcqcgc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wrnevmxn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lbwouifx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ldinwpzr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tyfwpvtd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3upxahzfj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oivubhra.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tnlehsdz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wysoksue.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cqydqjuk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jyldhxdc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bdjibpsr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kbwjrfdg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3brflkxaf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ksfnxgpv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3osixedrq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jwgqxnsp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xynmeqps.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rcabzqug.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3miwvbozf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fgfujfsk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bqwgxjuu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3npjhxtdb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzztcksv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tgscdxal.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3digozrwf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lewjvutt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qmlaxiiv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yvbslmkx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3apysdsrg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hviwphyh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ddysjxgj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ouwbcsmp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ubrynaso.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tigslvbx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jsvdqtvz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zdzqtuuk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gzlozjaa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ykrisfzp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wbmnojry.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wfbsjrvf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rucqkxqc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gqykafiz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yuuwfetw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mdcxuysz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3igdybwdb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3zueeygjo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yjiqbolh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nqcenypu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3onjdbdxj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rdvoqfln.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gbyuiwzt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ldbyjnsu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pyfyubun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3actcjitn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3kexifyjx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tsvqcgqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ockxodrv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pgtlqnit.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3uvoxejsg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3iydatima.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3elgwrbty.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3yjxdljsi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3libtrqyr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3rvkuvojq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ivtfnwwm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3grqjzhqu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3njxhjugh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3hvwipmoa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3aiqxuyed.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3irsoxlhc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3nviqlrjk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3zsfhwhcw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3exfqtwcp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pmffvnat.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uyteoxnx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fsiwzkvw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fckcavsw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ujbmrgog.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vnwkfroe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uliuaxfi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qudhosrg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqjzzpdw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lclqwpdf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zhuhzmau.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbbfbtnb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujspxtjq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wikfrqxm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzflkazk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3odalnuuy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eulkcerj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkttaa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajyoouob.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afdseblq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xivktmhq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sgcfrpkm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tffxktvk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocnslprc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tmfbqogb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mqrtqcze.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qpvumsmw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hmzvnpxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkcgkroo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkvgtubb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytfajdaz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3iqaivalp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kgexxtas.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fwtutifo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mgihpcur.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3fjajwiai.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lwfdxulq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tfvitrwm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ueztlcjj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hfthiowt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mokzreyw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3sdyhbfan.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hohpqbpk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pyxcxzgh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3odulhnxq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vcijeyvm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ydtbrpjt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gyoloskp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oncxzsba.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3iizuttkh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3frqtvncp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3chgtzqyy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3veguycub.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rmsdrdnm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fujaqfiv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kilcebud.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mmvclgdt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3veptchqv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyyhlvtl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lxpgaijq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kkkwfvcz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jykyigbd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xvhzwdbv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3wgguljpt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3rzdkdyvd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bqbgylzx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xsewuhpp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3imfchtjr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xgovrbvf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3utfzfyig.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmgofgfe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gfpznexo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgevuvys.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctuotgoc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oqdlxhos.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jucfzmyp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qsohatpa.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yrktekgn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ayetkyqb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lzfejqmf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sktmzmfe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3okhhghdo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qbpczqyz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3otxgobxw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fiynlcbm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfwgrtag.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3lsqrapbj.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ducitlbs.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwhotufa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3srskdtaq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3fvmnhnro.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tvseeoff.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3klhawuur.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ccqgpqie.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3nayhwtpp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ayjrzfeo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccellliw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3frkzepdm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwdveeu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3upktikry.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3byamxhxr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3layuylya.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kuocpzyx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zwmzypos.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3znuxeqxq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ruzbmwwz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqryiths.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlsyqquy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqztbmij.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3zbqaxabr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3spqsfhzv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thkacbqs.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bdykabzo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqojylo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ynlcmuar.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdcvlbnq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kigvhemz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rrrdhbjd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ednshmqc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3uwosynlq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3shlyfxra.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wszirpmr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nijkpphr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nuclqlsk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zlyzqpuo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cwemcpwg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cxzivgii.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zvzllwlk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3asbnoavm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yjyxhyls.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rfhlqtix.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3uthmpwwg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3cbzjgjho.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nqgbubdu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yubftqqp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3itqoajcv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3blzjrzpp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ofvrmess.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rtxbzjiz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wflpbpdh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ursgbetu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikwqyfzw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqprloqk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pngjfbua.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dmuntdki.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iwwndits.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebjiwsmh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yvefyjmc.html


<!-- 参考信息 -->