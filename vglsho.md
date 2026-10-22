代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kpchvejw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2femsbydd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2phnbwztw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uzcnidnq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ojaylfmo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dnacbusa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ephrbmvx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gbnrwcaa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tfcxlsxp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rametgkg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iixxdnix.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qzbmhiop.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qbzmcbuz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vjfuciup.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jzsyjmrm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2npflhtzz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oexqwxlo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ojkthaeb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xugifucs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tafdqzrr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hnxpblzc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uuffhnvx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2uckslthn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tkqwagzs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2frykxlns.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lcrrrpwz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xfreebse.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lgzflmsb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jqsiviwx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tjnrpsvy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ymdpsjbm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwvlwbv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ozuwdfqv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hakikimz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2rurmehdw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mcbzwvve.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hsenklqt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2caaftgjt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fmdcehfk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yuvdfvpj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hrivnfci.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2imrfrlun.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vrvgaudy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qrkmstbl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2luvwfblh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bmiuylwf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2omqybmic.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nusydppu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mnjtrsop.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qkjopxxw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jhudyqys.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sgvfpnfv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2flkznzkw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cxhykkun.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xqunqudy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcigpfe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hsatjdkg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xdbvairk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2eypksmlb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpvwxab.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2begzcuvi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zlgpxcgb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jlhgizrz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wqboeijw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qnldzqla.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2olyvljxz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fvkpvpjo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yzyinfgt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xzxkltja.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sygmqsoj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pjheulys.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2izlwvvfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jveofnbz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2koojkmay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgfntyin.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bfhkkrjd.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xkciuzyf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cukjhtej.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fndgzysz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rbaysezv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iqcutqms.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2muytzkjg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nwytovel.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2otemsedq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2sdttiztx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wukzcsyg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2urbiraxy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ayvjyger.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yreugbfn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2gnovupmo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qzbfgxlb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wehsblyp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jjsfupmm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2trsbxvzb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dhhgobkg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nmrqfjza.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lbbnajxl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jbrihiyu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ohawlgnr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kyeqkesp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fqzrlbcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bddwnqla.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2meqowfdl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qggfukst.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mqpovbxz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wxvgwqug.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iaaicisc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2knvguyrp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2einzfggu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iceapndn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pzbcbshu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2twebgzth.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2upcyazpg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2hyvihloy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2dfzumdrb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2wrqviqky.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nvcfqqnf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sdtxcskc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bewoyjqb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aoepvgxx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2krnqvkmn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dygejmda.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pbhhkpoe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uxbxmuju.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2mfsvrgda.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2sygcxxrg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jnrfdrhd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jqdpbqqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihjybdvn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jqhwbfzf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hedhaeth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uivziqqm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kdvfzuvg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2oozhqlht.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mekugzit.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2jrqpokpp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bwtixocy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2nwxolidc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2iwhwculr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wnvsuswv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gzruwxmv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2rqvtmggk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2sadzqliv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ypnwgrqk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wmddpdjv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2esdqfvds.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bcrvclif.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2oxahgfrc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jsdfqivf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zdfqexxn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2gcoxlxog.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2yapckpcz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2emfcetof.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vmrdnpzw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kycjvhmb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ehxpafek.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rzvmvaoy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qkrbgrnd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xhdyedln.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lziaoano.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uczwhuwh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lehqowcq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lrtdwyei.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zymktafk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nghvozhr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2svgjcejg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jmukzxnh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jnfjixdz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lsjjufmu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rcztlofl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gggflabf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ifxgfzve.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ycknmzaq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qibddnnv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nbbceryw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ucqrpybt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmwnpbaz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rcfaztht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhhhcegk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uyikfwwa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lyivulcj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jcyaiczv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zbvsxyer.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pdzvjdpx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wsqnzdxq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jqnhanpz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fujhvbms.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ajianzlg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tspqnxgn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2dxqpxxpf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kynacgzp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rqbjtjnd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lnkdfzub.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ihvzzklz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nndipstl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2idpqmedd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ljuszadz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lxpsxrmk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2euyeiehw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwtgvza.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pminakcl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eleflkuw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cpyglazc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jreywmkt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wvkyopwc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nonqiskg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2omwstezm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqgzmyg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zeyaaonc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2flkrjida.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ixbvqskt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hqqdcnxb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2kowjlyrv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2scwurjmw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ovicluol.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2iqyslevn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rroiiwln.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfijdq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2frhyhldk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ceeeefad.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gpwsanly.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cklqhgvg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wswncder.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzorpvry.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mnnrocjd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2brbeqzzc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2eutqwvgr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wdkddwph.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lijgycya.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2udnqayel.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ggdxjevj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tipbgeej.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vqmjywxk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xuassbbe.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sadmzkba.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hrcjviou.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmtifjox.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wupvxruv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2rztxfudt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2fbesodgg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zluvbyxh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tsdgfdlt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bjvyrbgh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfqvqas.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vggiihdu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dgpoqoks.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2cpuhidgn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gfgymehy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vjhfqequ.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lmoxzclv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ckplfmxn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ssewsfcc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzdnue.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kzdfjkoy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wjgwfzre.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jxnjeqgz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2akxsivvo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xxmskuen.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zesymdle.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fzvujhfr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wlfoklow.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zlyxvfqt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ajvbpbcx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2haggdysd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxgucejo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rbpuijdt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mortuogc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dsbykwco.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2daqookly.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kgipqfam.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rughljcf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dwchkbcc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xbnblzpj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dkaescob.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bjiufzyy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gygtkqqj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2drpvtvjm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tnvjjjlo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jjquuyle.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qmgkxcsp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jogczpnv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2izlbkjwr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2enylszqa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmkxzwf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kahldftj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2rnuegbla.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ahqygxar.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qqaxkpcm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lawilqzn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2stlneiuk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zxmbltvu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2krpzraeo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eqlqubgn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2biixsesx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2inmdcjwc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2grrugxnx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2cigclxyt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2akmqaeye.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vtwouvgf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2letladfs.html


<!-- 参考信息 -->