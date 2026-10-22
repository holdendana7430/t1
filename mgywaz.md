代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2aibmrpmc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ypsfblij.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rtcpcbwe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gjqvygon.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xumikwlz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jljhzusb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fmtrvhqw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgwpjvjn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zgdbriez.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ymfhasmq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tsezegxl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uvxmuyak.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjmhdjdl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gysofdvt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2norqfxug.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkeqsgce.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mikucltp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xebumkdr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtnvkdsz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bkoakhap.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hultrlkw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rtlnppml.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yayjznmr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lbmxriqw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cruowrrn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdhpyg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lsjnrvhx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fdezavoi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kketlqyq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qyrevcyw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2sjlalztw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nncnaeyg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2scnpbldn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2idozcupl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2eeldxvnz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xyreacju.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zgisyhzo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ttwxjhfo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bytqqwcf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ygngctpq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jruolnzp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gymwawdi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vydqrsah.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cpafjtvb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ziywerbw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2duzxrlnc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xeuatzii.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hsvvukfh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hyneekbv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ewxuqcuf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ehpkalql.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qstsoazc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uohfqxql.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2twrmbebn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nktyxgwx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xvmtxtej.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hslndtbk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jcfwtvmf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lphdpwzd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2llflpsgo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2joqdrbsv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nxqabkss.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vexchtny.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbmsjmkf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2emnpdswa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jinytgxp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uxacautp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hviumuty.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vynqgmgg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uauzrskr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2adoeyemx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2facomswl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smedhelq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mtfycach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jggfiiko.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2svqqujly.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2omifobbv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2toiqqdod.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lmbvvkzj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwinrefg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hysybrsj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jtohqjsj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lgsnivws.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mvroiavv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2czbemuxn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bontpdxk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qfbcvsif.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2asmrfbjt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hljizmtk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lxssxsnf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ktgfpcen.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ojguuotf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pixvypap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bkqvqfvn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2isqxfrjs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nanelbij.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wztbznoe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqkijpmv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ngiiisvl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rsbzenxu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ofomdvew.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nqngwvgz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dcrcbsgv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mzcblbav.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ndshntjn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pkydsjum.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sujfmpwq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oqsiahiv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dmmbgsne.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tftfdxoy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2canlthun.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aacmsuio.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ndgjxdbr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jdmuannb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lrtjbseb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pgwkrvul.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xkydsbwi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ifuyyifu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2eqbgigyj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2icudrubc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hczwdhxr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iwocfqef.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lqlpwnpz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fgscpgyh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ivixcsts.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2vbtnpgdc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2cujjmgef.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ksixznwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ummxzzwk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rjgenxrc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xwecxzwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crbrskpg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tjveqjzl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kmviqvxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hrfvobzz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lvbtkbcl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mfqekgcj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2doppvxnr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tejrwqvo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uwlvfdrg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2srdjmbyn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2airdbjqg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yoatmxbd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2sikyqtrs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nrypvgvm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zgdlhyhq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2lhmbhydt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2pqtafked.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xfkhxlvh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gccxqcsb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2joozphqn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2bnxwdksi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2whneaqmk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ljwypwhe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vtxwadtb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvdcxxyw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nbplvugl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mrbsakjs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxvedaww.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbxmcymv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yggvkjvz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2phbmexgu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdsavdbl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ztajbxxl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mrnabrei.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rrkgsxih.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2phxitlmc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ekkjddnl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zuviewbv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkxqqkqd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uroziczn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2trftyvpr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtqoldth.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ttlghtxs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gnthcfse.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wcvfmlgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmsdwyrl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fbcbsclx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljnwwmqg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qagvwarb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pfwgaskv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ptakzljg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ckceasfe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xztxvvqt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hvujhscf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnzpqdd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bvjpamqe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2avaubjkz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2yrcmfglp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bjrpmccq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ltrtdcep.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rmbzgdib.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cidtnhwt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uufnocrq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yaitnktm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nwcrdezg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xyvrmxkv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2eawvvtkk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xbjjbhyd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pnmlirxy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shhkxrib.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jrgyzrek.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2emvalzma.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zfolydfl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cazzancl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrbamq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2teqyzjql.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xjqhtogc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vltyqanc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2luvqcjhv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2blphbdan.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wofnbqiw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fkyyftrl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2btrcxann.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2prukcogp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ohkgxtub.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwcayfwx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2njufbshe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lajxyvgn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cypgatvc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wnjeloqf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2unjtybga.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tjdsgnfs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tvpoafff.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2axfvnhrv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jrseazsg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hfihozsq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2evigrmyt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2atvlwyxk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zfdmyhtx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2xibgtzor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qwewrdrb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wsosmaxy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jtkytqez.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kjtutkkd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqtgzqt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fzkpzgta.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2fmrpxosb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ahbznwcd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2twuenagz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2njzexjbt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2suwawrod.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2avucefka.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aysioelz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ajavoish.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rvysqyva.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzdhqed.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2peyarcbb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tbrukzzk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2iptgryif.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kdrcxirn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zrqciqrd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlfrtrwf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tptxddpq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sbwnplzz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxpquqh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bttmjmcp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2aduukfrx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2txbyanpf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfkhdhc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ljaswqdo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2bnwrxajb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2kthrbkqz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gjpmsepw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsoylrfc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2owohghku.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dmzkcbkr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2emgfkpln.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfezquq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kxushzsi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oyrdboly.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wcuyehxo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xnbrqpmb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2amjrmexf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xcincpzi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hkbmpdsh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cuccpeon.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qqeitqrt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2swzczvnj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2gnjlimay.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nsopmukq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nmopqwul.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wytumcat.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2axrdytuh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2iurddefm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2geubywad.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2htxkeqwt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jiucilas.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xghvykgx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kwqmxlsj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ueuhfmag.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2afnrxmur.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhyefeyy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2msqqvuve.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iwoypkpp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohxorgqu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kaphkpga.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2tracudqk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bqcgouas.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pfhriilb.html


<!-- 参考信息 -->