代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bmxbcrgz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2djmuxgzb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dtsnxpwa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dizgtlcg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gorwvylk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wezgnkze.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2djxbfjna.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dxbiiowt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tabvohjk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qfvrcwjq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kkmrzfjk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgyrdql.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfipnlpj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2umyfpfay.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2avayvmkq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nxpjochz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ejxbziuk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2iwizajno.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fzthsqqb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pihhjrzo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hrmvxtcy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2npihdbnr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mocwvsrv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yerrrnnm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qbpiydls.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2btefpnhz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2oivbjyqt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yyjtvxzm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2itkxlwhx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jkiuxnby.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2frpviecs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wflylcya.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vhkxdhpg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2oovktfya.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2svnuqbsl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rnxktpnb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qhiuyrnz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wewyhdkk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2awdbiqdx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2inapjgqv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hdlygoyn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2znqgckxu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2knpvnvvv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hgtpxrdf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fhnxqyfp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tlchupjh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2twqsiqgx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2flwtolwh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zmmtmdvg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vrsjsgnu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wcgxunsb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrosonae.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2efqpkjzb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewtbijyh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2awpuhqrw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uoqgsfya.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2apetmvee.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdakzrs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xynvbycl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnrqqnmw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2klvomwra.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2niiyymcz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ylbzcitq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2trqeoubl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gxxwnfhl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gcbahmwe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2uqsromic.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qsrqjscd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozdfjfwa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bwjoizny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pldyguid.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zjbkamlg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xbzcodev.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wbhfyhmk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnilcy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aifkasxc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zqfxbgyu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ddrcrxhi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ezbankvr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2orzfdobw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2utplrwdw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2izudxcqa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ttiswonp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2awrswhid.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xccvsbwc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2erjxhbzf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xiraiddy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2owaildhb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bjamkvsi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bmznnqkf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ghrcqrzi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kcuyyhhc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2soyszfrk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2czqdfozd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rgtdpjcd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ppqphbdj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2miyvjfcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2knveqrab.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tqlhdfle.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2riycyrtw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ovhdiieu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oosqwohg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rimudzmc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2azvarjhr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ohaodcqf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jjynzxrj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2snnybbct.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2obaaallb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2uaezczck.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ajwktsxk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qpobsbxx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2glikgtbj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qotkmhdc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xybwhrla.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2naabrtxj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lmkgrvbi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qbuvrxvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bbqwqfvc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lkrnoczh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gxytfspn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kqhvwnjf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kjdfkkwh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2iisnzjpr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2nhevvvoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seqniowp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2izqxomcg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bfoudbjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilhkvvru.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rtsnedpt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2yeyqkwlq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lqcspzrl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mpcjvpsz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qkrpnmfd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qekunlct.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hpxxurcm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ibreqsyz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lzjebpsl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lbrwriiy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dvlsyksn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2djmspvlk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rxqhjoxj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wjsqbyae.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vjhkooiw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jdgajnmk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jxdvehwd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bnsxfxkr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2eqooehwi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2umtophca.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2elnkbogg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2stdocphx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2prylcsan.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bunwwlkj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igdqzfrm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pfkkvwop.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wohosxbq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vnatjsal.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vmtewomx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zymrpaod.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mewcudls.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnhkysxd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hasslrxs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pvvzddsm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qzkfkowo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcruvyjk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2txcqrzmk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kakamxzo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wctqbdqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xndpvofp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uvyoblih.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2couuvrvb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pwikwzkx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovvibfni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnkwtwfd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcecbpof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yllqcvqy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2myzjhzak.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xbjgchzv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2whmovogz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rcgzqkbl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2intfholq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qwkgzbzk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ewuriczk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xohwnhdw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vgpwmtlo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ncqpxbcw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2syezxexj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2brwyyyrk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qtotjmgq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ltwujjcz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vukwuknl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zwocrizc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nixjsrcd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vcrkhqga.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vbapfiah.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2znnmvvnx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mkgdizrc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vqnibqpv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pjpuxwru.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2phnyionr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bvgzgtts.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xcozncic.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbrlqni.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2stvryknw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2mvogfnju.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dohonhks.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mkzzzagj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2iukoscud.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rmhruhcu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2nxogtgbn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hcudtatk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bvhwllfj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2llozsgdw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvzssjbu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdeoshbv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ihbedfzd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uuhzlyvy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dbxcnbhf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cgfjxymc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jpgpcmhv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdfwwuac.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rpphzqib.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vcokxjse.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jocahbfu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jinfsaha.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kgbcnuyl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lcvaupay.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2irzgmikp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qleutqve.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2atdyltpu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2typjalpj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xcoswvvd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2risdwtqa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2meshwmrc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvlrcpo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xodemuuc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2eizceqcu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hnmjwqam.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pfuturpy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jufjfwao.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpbpyfc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2giwtgkst.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uvubyvyh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gprpbxpf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qrjwaqnb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zvmmonyh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2uzqmcxvf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jwpyicuw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dbbmyfcp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vroxvbxi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzotwhfx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zolbtmoq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2omknrleg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kaxybzya.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2udhoqgkm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ddjeabpy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lcflrokq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2asjjigii.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cydqsslb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2veazlcsi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2klxdnijd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfnremli.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fheoymue.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zrdsfgxd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2svjjxdwa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nibifbft.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xlvcjrcx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qeyucegf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ilzyowat.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gxcypecz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nynpefqz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bzdsfboj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2quqarfps.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xkkfzxgq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2btjrjdau.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ugwnrkgg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2biswfkys.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2upbotdir.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dzsagxjz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2whjzhgta.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ttkfurhd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2guvovban.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nrrwsmha.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uocfndlm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nfwydcdp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uteaeack.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzvccneu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pbiydjnh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dvaqnxcx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kahnxanf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dkncteli.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iajiseoe.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vztgxjdu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2smnitjjr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ioznyeil.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rqdapiba.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2owowiruz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fjairify.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2emzrvaiv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bejtxxff.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2larybuur.html


<!-- 参考信息 -->