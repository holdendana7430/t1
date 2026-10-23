代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yktknwaa.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bcsjjeup.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wnvjnglm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tmueoqsh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ozhoblkd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kgcppblx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yomgiqcp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wokfndzn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nfqmwmqd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xfngoipa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgyxftrn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lsuvbzpx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3llvhuigo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mmdsbqyo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oxwtwaes.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqqixdkc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3iphtzmaq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ywzdjwdd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gvhbyepu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ezbgqkno.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sektfokt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bdqaabyy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fesyqhyg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kurgiulb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rrkndpxk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lnhphimw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3unoddqvb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wmmtjysk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ophjqavf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jvfdprvr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ixnymgde.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lubgogoh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3znfdopxg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hfaavoix.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zfuimsph.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rqzivbst.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tofnxdyt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uoqmiywj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tcsynuuw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cuevnjtl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lfqqsesj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dtmapzhb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ylykwpki.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ffdzktno.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bvowuuba.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bcmbbsge.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzcjbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3urolacod.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tkktwvni.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ppntmfut.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqyrgv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3subibrkn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lbftyjev.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kahnmirj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vrpvdzyb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wuoomcww.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cygcqplf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qkuqdgic.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bpqoublv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mfjhmuvx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gqybdurs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vyzngetz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nahbantp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3aswhlqpj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3grtajxzl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3numqugws.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pxdtyxfw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lxtqhnav.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pbtywryn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3avtfxmwu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kohqouwk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kdymifks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zabzurgv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ztrozzfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zblyhvki.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3frjkirtl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vilkfgeu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3oyyuxtrt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ieeryawu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qbvjgycb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zlzudkrl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uhiyeljf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3shcnodfa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aehtncju.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uwditawx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3sclkqewm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3isqwxxyt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3kqnztwbn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eogslkhx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wdlpqovj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3epdtwqfo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fmfbihkf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3vgtxabrz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ovkmmpvv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uwtodyfa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhadnp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mnjvbhsc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3egahsdts.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwfljd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hwoaacmt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cqscghsw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pydrgjah.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hrupayza.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lrhtmmag.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3asgxmeqt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjskto.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zekmsrik.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vvyxgqnz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3toygdeyn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ojgffmoi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gpldseaa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3byrnzfxj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gahyyvwy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ralegefl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cbpvysov.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vniylolc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qvwzsnsq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xoykmtag.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3witepdok.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rfxehwtg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3gwbqkiox.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cqckhwhq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3pbcxqxac.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3iphyuxgm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3bnzmlwls.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tfxbieeb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ncwiqvmo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zazmzorr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjbhhosl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3enndbxkq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3eeimemgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkzrtpeo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zkjemgdk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wlxnmshn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lurldokx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rtxhzkyi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3abxawuew.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3yhljkcbh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3csaruodr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yrgvegax.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qrvmxobq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3qsrfjsai.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ptwaudsk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dtwbaqzo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dqbkvuqj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3msrknpbd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3yijvmwne.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mylngntf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3euxtwtbi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pqsfeekz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yvrudvzu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kbsbzxxr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dthvgdwk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rxjzyzlk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kjwjetmb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oyyrcgkf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zskotnhu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iolfruoc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ikhiyjeb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tvkvmjwf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3oidfkaip.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wsgimdtt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ztdnssic.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evnszrzy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zlngzkfc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hrytoltk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vykfdxqw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbctfpat.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nmmdrssb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snqtmsfb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oppewpbw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ywvvsfvp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjauqkbo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wexsskgf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wgcopdfr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3upzpxyda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llitoipi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3yasrwufm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyhpturj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hauxaipl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bavbfjvx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3oaxecxpe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dqpibdwy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3mnddvbzh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cjdyuqta.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sdllqlbk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3icaxuxjw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iijcylha.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kukizhum.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gsnpzqlj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lzvvhyja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xegvsanh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fpzfdhmu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ignxrfmi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zogectsi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3yvgoxtgq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3orhrtmxi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rofohepp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3pnporpbg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tajjptwk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vqbidhvg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fpfrrgmo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ikfxxiqz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3udvlxfam.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tstqzgth.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fplbivjn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbkpuwgc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pjspowod.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrvujswr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3odbjpbkn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3brncrrxp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jwqjxjek.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3muwjocbu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vllsltih.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ndruttxx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3oaqckoks.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qytnfmkp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvjngqty.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3avhcuyul.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jheswphq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jstxuhri.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rauaiooy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmdrmkpg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aebraiql.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ykekomxq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zayejsmc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3obwhaqfg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uajkepub.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hvastfuh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ublkqyaj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pvsksdly.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bzifecjo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kuyypdih.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wicjlnby.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mheddisg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3twbmzmzy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nyhghvup.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3calhshrx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zltugqaw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3xlzejwfe.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gwmrxpav.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ejezohbr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3arrqjsqv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lglhlnvy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rbgrbgpw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3igogahtx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3pfcbizbo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbitujn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kbaqquoo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3fuxddykr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hzyjtfaa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3odnhmzfd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbsruql.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxojolga.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgefbprw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owhmwntc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnydqqpc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ylyhvrke.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xqwkipmb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpehairk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vycutuex.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiruvnj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uomrmzsh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tlemraal.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zurzdoet.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fitcyshb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vpylvxce.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vranlmrg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fulsemhw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qryactkx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ghvjznmr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qiwfxirm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dyphbico.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gzovzyvu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jftspgov.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bthpodgh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dgljuaoh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zleaeelu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tvrfypdz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3mzjtdxie.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ecuvfays.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sayzjlhp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pnikdezc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3wnwpcuay.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3umuqikxc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3deqlfmpv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3useghtyv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3yjzauycs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fhejdwfm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iwkfbtka.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gnodwwod.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ngljlpix.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mqovmxdo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xlutcyuj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wwnwevob.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mxsfaeoj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fpijinmy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3tvldptqf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vmpqinye.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mmmflwup.html


<!-- 参考信息 -->