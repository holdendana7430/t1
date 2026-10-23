代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rgbrowri.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bicftged.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kbemzzrh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iikhwzsi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gxepuoya.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3irmfjgpd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zdvxplvf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nzomkrza.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3csetyxkp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3atrjjfne.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3iqjzlkrs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpucdgvp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jsdhqsfh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zggjgswy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3abmjizxe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kpufuhnv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqndqhri.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mohaibwj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mcucshws.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjiofwpf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gajjqifl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3eeshkatp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rshukgyf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gkmseqdd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3alhmhvap.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mlvstjyp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xilmsdfy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lululklv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3erixfwau.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wyxfmjsb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dtgafoin.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3tnzqcrrn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3anxwgtle.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3glsvabel.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3csjvqpjd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bpnmgfbr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3wsyysskw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3geshawqo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3owvwjumk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kdrqamct.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qhsujbtu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxaooba.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3isdnagoj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3acjwngom.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mplkdisr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xawtevfq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3njlttaiv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ifwbnkss.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kepviraj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qeizhtxp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sjgkxzsy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tglyynzr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3shenlyka.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dmhnsgmf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tywoxutl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3awnkpajg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vvjbxmfd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3axgsczub.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tuahuzxc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdiqtgr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3rbqfdvdt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgmizyns.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ockgyemg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnlzhct.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ewgxsoai.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lsludwfw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yvkyeubk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3pehnzfbv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tazbqimo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rtafygxl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mfdxznvi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3loffohyk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3epoowkbf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3afwcweeu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sdpkiooh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kvimpsqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imezhrco.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3uuqslwsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cofuydyw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nouaxjlg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dsrnxivh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hjtrtxgh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nfcqnnny.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cmjneeai.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yvzfucvy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yqkjhzrx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zqdfquhg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3knjtzjlp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zryqyori.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pnahqtnq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mzhlbcte.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nfqoklzd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mggsqixk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fdwlzaky.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ycwizzmp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gahvblxz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rtabuqgu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bpuyxoig.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rhfpsive.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xwsrtcnz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ihtptlkd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wyvlctef.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kekmughl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3szbudlqs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rneocema.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nfkjqvob.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wjhgyori.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3arzdxxkm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yibtkqnm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pszleour.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pwanafer.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3helgobju.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zoornvod.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jslxmxff.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xjqpkswf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vggtdcnk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3cnxjainv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wrjdwpha.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xnvgfsek.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cbkjkbux.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3atwevvym.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rzfonilx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gzfdencp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmablesy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cozgaarl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ivhxknuf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wfqeoytb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lfcqijue.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dihjryfs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ywnojxnd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nimciewb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3vnputoto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjpozdts.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3aplwuoxd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3tuyvycex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egtfihip.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jobhgoxu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fsagcvme.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3jllrouwb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zknmorjr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ylgzrigk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3dhtiozca.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3bccexwbl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xlzssiib.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fjfsrlod.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3juqnclti.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3exzcdkva.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rohpnesi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3uwitbxvd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3etfnttvv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wsztwvvu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ujmvjxsx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rmkqgdit.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pczeesiz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mowwpwca.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pwkfhlfi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bekjmyef.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3frbbvtbg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zxzypxsb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3idstklgh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ouungazd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gwcarofq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3msuieynr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3grpirfse.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yvmupxqc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrmzuzuu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3omirmbnp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tiucljig.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jyicgshd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ngaphvej.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3peptomgh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3orquhchf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ouayttoe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sdizlskt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ddpmygfi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uyaqusdl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dxzwddsa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bitladyr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eyowksrh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frrgbpnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyfxbvfd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbtggl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqxoyfvg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afulydmd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zifluuas.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3oqpjizpm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cozprkir.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jkwhekiy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pwcfgbff.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vxjmosdu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3tyessjyv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mzaghvxn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3icniidwe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3chfbwaek.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bhfdmcmw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wsncywhm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3roajgajt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3onxvelka.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3eczpasio.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3lccjixla.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zsjznczg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lkjwepug.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3okjkzkch.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ojcukgsc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wwqaslau.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xcwopozi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uxxzrupz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nrawotdu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ifrjgiue.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sncdiptl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3autljbum.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3txfdsnss.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynorlble.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cdcrzbcw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xitjwnzl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vtkfaoxq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cddxmbqb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzyleir.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3wtiqekxi.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3azpnaegw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gaygypqm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vnksvorz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ugtiedgg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fycsfsrg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lraevrcz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aslxefif.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oxplwtlh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tmtafbmm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3solsqtpw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rhauoffn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rsbpmnlu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ikdzzfoq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ghqhxstm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jmxrmhek.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nzvkmitc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lgcarheq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hffcrocw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3esqcpnmr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mxfxbenh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ispjivcx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nzglwchn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3laegajqt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3gckzfwtv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qmiewxps.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3brdxjvpw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fmwjzioa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pntywvkg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hksigrre.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybpxadvc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sourvskb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fwipsvol.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnvpwqz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gchodcoj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3prxxzgud.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rycqmsmw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qjqnqutr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3phtutghj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfuvrio.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zltgvwib.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3afvqrsvv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulaipvco.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3paztgxmx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lmbflowk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3twulxpux.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xtxpunic.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3dyhrsoqx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3traehwgr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mpaaynaq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3feeoruty.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lkerfupr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fjkrnrfg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xfvcxzty.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3joicvipf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xcwixlji.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kbvooxyb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hgeskidj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ktdvnyvu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ybbteqpc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dojzznhx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bcdsthqm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnhorz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3odjgkhce.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jbweaqed.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xbzbeuiy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3oahtqpsu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lsufbcuh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jetbunst.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yhtbjvdu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3szgexwae.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vlggupze.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dsrkoclc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgxwsnt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sowznnwf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3niouofws.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ozrbdzhf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qmelbaip.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zcnhwaik.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vcighphy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pdahmdvi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pgcsfhad.html


<!-- 参考信息 -->