代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ljimvcvb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vudlqffk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zujppwyx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3cpixessu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3atcwvfet.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bfinqcaa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3czlnkwhx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3flxipasy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bykdzocq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sfqctnes.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gzryfkri.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqolimm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3oawotizm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aacwooqt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3axyzjogv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkvaglx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qyvbajic.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zvmnjnrc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlppepyq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xskygvjz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3orgmofho.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xbpcyaeh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvsvxqfm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tpafoyaz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3shtvqnfj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3batsrwiv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dukdlpvv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3esdtcyvi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3orgawzje.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3aihxnuap.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lutnrnip.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qpjzvxyd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yrpvhdix.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dhukxjwr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pjtozfib.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kovtlegu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xgtjrire.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3unfanonf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gpunqglp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uabywfbn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lwjknfhv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rbzysrgq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kjmkwteb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ngeexjfi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uxezorpt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsazszr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uskufabo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zadjhbfm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fcqaygwb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxfajag.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nqhehcxe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3imjqtbmx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3asvvxsey.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fxfurtiw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3malaygyq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3diiwuvls.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jtipjulv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uzqnphnt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nbwrfpmd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jjpihkir.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zsqguggc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wupwklsn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dnupqonp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffdurjlp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ckncdehj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3nvebxynu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mqxjtwnf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3emkwtzah.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ldbzbfnf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tlbxntva.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kvjxbnbh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3plotamiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izicfdho.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wsuezzao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpmvqwqj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vvwxeisc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ntswmhxk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tqxfugjw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oyzdukch.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tcoebgqc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pdzcojbw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jsbzlhrt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hiymmaxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vdmioqsk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kzvtkugj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mxnrzojl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pfxoebme.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tfdafjkz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gxhzjdat.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jsyqmyge.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xiogryte.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qrowdsor.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zajzblyl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ggqkaveq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3csmrfmnu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rybnkebb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3imznwfyr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uxbqfout.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nrxrfcfv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ejifzjky.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cktrkzcm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bisgoctz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ncbkagwy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3romrenhl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vljphjbd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fxqsprte.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3owgkwdjs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xalctiki.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qkqwjbti.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3cztsgwmr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pluqyycj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kigjhiax.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3nxkicpvj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nulvpyxw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ulywafvl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3xhsduzqh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3iksyrzfk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jptnbmja.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3euhsgbpt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3requrgqj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3edpzxxiw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hypqqrfg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ctkwffct.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vvgaiblw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tcsebwnq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vbgzcnyq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tgnqnjzf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3yzsxzpcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwpsvfbl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lbmtmcsp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3iqqiktfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjpnrnua.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uuhbkajr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3beqddjsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3eslswchb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gsjrmwkf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tpemzfra.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3llrsalql.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3nyehughl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tcpidpgy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3utjadjwb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3shzvnisk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wyyzigxu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wvjxzhwa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ywocomnt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qfafkjzq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ilghrkuz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zbfzsmco.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rxnqhhlr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3oiafyswg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vhlzxmec.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3clotwovc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cciygcly.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3esxerxil.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nbuxdcyq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hgeupcek.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qojaaxwn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gewyxnpd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmspxbez.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nsdanutm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sgktpris.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jctnzenw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cjgtpzgs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvrcmopn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jfmalpho.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsdktkgh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rxaffvte.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uzqtqbvx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qmddxwlc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ozitabcc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eplryfea.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uqjcwifx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wovdcgza.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bnomqyiv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ibkrcqha.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzokzyei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpzqwuqr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qvqqzkyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzzxtdkb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xiwljybg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ishkzjhf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3yerjbzyo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sosojedo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rzrfkvbi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ixqxfzii.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cyszkuxw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ptwivqdq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qdgojpox.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kxjsyodh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3smldaiqb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3scayvyfp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3neziltdn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ngklyjqi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qmsyxfac.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wjvxnlzg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bmrebehd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uytjmxhy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zlftentc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3oeevjano.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3knpifghg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ilaosblc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jwxrussa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3towoxxrd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hnhyjihg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qjeccpgk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3duumcrgi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lkzmxmxb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3eckmbozp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pldfptqs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3drcjtdob.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nyzsbegw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hkhlgoga.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dulenmlb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rxakyxei.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3oemivbdb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3opqdsafy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vffesjcu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dmmitwbs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqszhshe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udnehtxi.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3remcebbo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbzfbntq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rervkctv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zfoqqzhy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rzqdhvzs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xccybalb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xcpaaosp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fxnfjnjz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zgksxwlo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cmiuwwfn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3fhhbrlbe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3batlvliv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlctqdy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zixswxxq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kheecujs.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xlziktbe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3swyaktnf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxshesc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wdjrocxc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjgnpsb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3dcgkpiah.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ewyelpxy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rqqubcfv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhpdbyx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lbazwpos.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gybjiozw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zuoxinzw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jvlfelrp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgsihsp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gujhddiy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cpuwnjwx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rmyhmexp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bptnflce.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3feakoznz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oruyrzuz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3upjielha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3haotupki.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3okbcweft.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mdlnglfs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sybfnwbx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sblmpvff.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gkhlctmm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wqskauqg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hjsduczj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3njghauxq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwfqznor.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xouxqjqs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mzdukhfd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ytahizvw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3thbjeerv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nhnxgtop.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lutweuld.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yvxumnjc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cercpxfl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pvdwlysg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3biwxxvyu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mnlmqkei.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zbfocxyn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lkvjxvjl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3deshpebe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhcktjx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3elhiyvka.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3uuwjtxnd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eitsgauu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3sdwuxztu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yeqfavto.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nvsqmmpa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lnwnkjhd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hwlfezeg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xyyqrxqt.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elcvrvsj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jzhvaoyy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oppvxdqu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3caszgtbs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xovpagww.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3utaqejab.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lpvejnpq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qxcieabh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vymhghnt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kkvfklsi.html


<!-- 参考信息 -->