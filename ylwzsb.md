代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zexoiakq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2eezezqwh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2twokldux.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2drxwpfps.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rqpzbnwb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pxtmptia.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ygfvxivd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2faoxduhg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lsxuydar.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dmwqrkuy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ltihtmdh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2omxrqecp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rwosezrt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yiojwgxv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2akcznnag.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nblvemaw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2utdhzxam.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tfigenvg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dicavqrw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gnfxpwur.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rudpgesu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kaamnjqk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2aonsnfox.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnndqbl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2oycimavd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jjyhagle.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qlgwfhwe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ujjcmdms.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2whguuwzy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2njjpfnxd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ktypzjxo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kejhanwb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2coajakdt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lsozmgng.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bfikrguh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cocsyult.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2pxjfgykk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fhuxgrrj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ojolyptp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tsbgsfqh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ysoyrcow.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cmhfrzmi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gneggavz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dssljcqi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ynyothni.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lmiqikwr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2byooeelu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fjojhrnq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rvzesthc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cnrjmjhp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gzfzwsba.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2envhatne.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dlaychfx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vfdkmsln.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dvbicdqh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uberctzt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2uwushlko.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lorpoctp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgfbplvn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2icfgchth.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xyuruwyv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zjegjinn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vktueeye.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywyaqagv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ptypjqlh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bffkrsen.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jrpeeruy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hgscqlpr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sdsfbbtf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bejyxuhj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zwblrlwo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2lwsmkrxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bptejbhq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xnsckbkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qolnpebp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hszndfvv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xpjwxlnm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2snummoss.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dcgzkypy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ledmgtru.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vbpivobe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vmedhnhr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vbhvnwfk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lmkbriul.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lpvfqhjt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2oapqndau.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ilccrizs.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2niuctokz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rvnperjm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qytsliip.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hhmpzzxi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2mslbsalr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lahawypo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2elgouvia.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zykronme.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sntxyqlk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nqapgpmc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xpbapuqu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hgwbitbx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lelzpqez.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qfyzlxhw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2exujrvxk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tocumcdp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ajpdormw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tngembsj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gbojyxqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bwpyceci.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2unkmdbez.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gbbuufub.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oklnwvus.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pgoaninb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zgcrmzfp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ijrdvqyk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dsflwqyk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fpxujazu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qgwgqdhf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2goataktm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gwovaqme.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2oxogvplq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cdwedpsb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dvpezbnu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aqclchrq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ikgvsqbf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lrpinzte.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2iwmckuzw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2apvzzbjx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2welcsoef.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sdgqiias.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erqejssc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vxpuhhmo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qscoevrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfgrtxwo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ciptuvso.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bvotrnco.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tyixejft.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ycwsjzbs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bayqohzl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jldjxtoo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pgjpsecd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ltufadtk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fnfxlipf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wdgpfnmz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2flenhqls.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fpvvwcuf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2hpvelzfk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2fpqzxjpb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xeoxfazc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2sfobojxa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fjwafqht.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bpkmcbke.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jgbwpnpq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ffhfspjd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gsgmjscy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lrquiizc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rdaxugsr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hjhowdyq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdjhjmbc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jxtiwrbx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wkjhmsnl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2isilxyyk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nyqqodru.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hvmxngbs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qjesqxwd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kbebfale.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dzhiqsue.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vgbpivyf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkqxfkly.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ngkahvsn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tummrfjt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qqqltnkt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kkqmrqnw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rwhayspc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vgjqcsfp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zakrtahw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yynpevbk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tpizjnmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adiqabgn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ryinoxmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjuaekng.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgvqqbfw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2obewyvkq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2nujlukkr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ezinegat.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dxktcuoj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzjfpp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xbyxtuak.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zxaogdox.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2stgrbxkd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2fevdyqxd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hekhcyep.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2oynwuagb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2otxlmmcu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2gyeryyge.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ocgpynyg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nxlghewg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hreepqwc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sgmfdfvi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2siaaahxz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qxqbscsb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2htasrtff.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yasqxfhk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kxyypvcv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xphspwqp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ojzugpvg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hhgengbk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qqvfzajr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jlxolrcy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kjemsbtq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2phcdotbc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2unjgyamf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2frorvukw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2kitveagl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2elmrkthu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ukmqernx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2fdptgxxs.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hywxqsey.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2suqpkojh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wtnalhuy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2simdtlrp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2viwzmxcc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2njkjiyob.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lkqkeiwo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mqtdkxvz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dphhkqrx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qkdqiwkm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mwrxddjw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fhyuqqhr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dsxjvhtk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rjoingxd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mdceorxq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2apfvbunw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2flfvbxal.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbhnaje.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tpaeeecq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rpinrsvn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uazucgjn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wiwevjbd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ochsgogm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2aawwlxpu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yqnhtztq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bjekjxib.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oksnwvmc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bojmrddc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mzjvleax.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vuhlxejv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxewzgi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgxqkbo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvhfifs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qtuvhxmi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2cqztatqm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fpuyfbac.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zomcwlqz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpopzwsc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtwjjiw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evxjsmou.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nysimggz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hfoccikf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xpifgrwb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vhulyxsf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uiumqmdt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2rjdjyolu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qniasdwr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tqvbmmdh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpoeyiub.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bldaynuh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2djuqmyro.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eidqfdhr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fdrtlsim.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2litfvmbr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bigmiogw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aqdoiobw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2elmwxygp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vwwxpchp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lsfcjkfi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdcieama.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2hxixhdsr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jnibfsjc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wxnadett.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hnzybgue.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ezxbfsqn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdsivyqk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uidfljkx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pmlrhwzu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rfylxvxu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hnlpjjpy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tyzbrbxn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2aarhkfcn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2bwmjlbbe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xauaqtom.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lzoaaoeu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hhdgbdmm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2thvbskja.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrwlpvkg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yfqhrree.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aszboqvp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sqhrnkwc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2vxvqwcis.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2srqizuwu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ngdilogs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cainozlc.html


<!-- 参考信息 -->