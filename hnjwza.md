代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hmrycbri.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lszelxag.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tmckjnwv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2iyayynwh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cwgzhegr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dgubhkxg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihfrwhbb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cldqolpt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ylonjeno.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rhaxhxwd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2sjhkrjbb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgnndqnw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kobacoqa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yqmdqleu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mgqocdoo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gcrajkue.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mjgxinje.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ifzdddxt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2utioaenh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dgrymmqz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yrtcbldi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jyvbqsic.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fqxmhnpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yhqzgqmx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fvhtlrpe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2szhnvfvk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pkoilpmy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xigowrzo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2peeoyzkl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jfnbezes.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2efmcpjlf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yfaycrni.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cfwpdrfy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uqupqwsg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2omoufrsl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lkfqzvsc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yjjpwrkk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ckuhuasb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vxlklwji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aunyelgb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dwxdtlyv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zzztcmwd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpxyrs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2duqvbwmi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xmrrvtfl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rudymjiy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bapuncof.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vdadtqmv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bukmcogh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fpyqvyji.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sasspqpa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hdmfdpur.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2blkjbgiy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lrqdldkd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmzxcmua.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pcqessaq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ozfropei.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nwqyppjq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2olsbrqcs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fsodkuji.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nhoowgxc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rxctydaz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2eadpudha.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wcsmcdau.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ffprxiyr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xufnascg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pnnvfxxq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bgfisrny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fivnbdtt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wpwpaeod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svnkkaqd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fvjfwzxw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vpjgnzgk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ibdfrivy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ezvrwxga.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2faxvrgpd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qotnsuby.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gununwls.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nxshnqrb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wmuqbgqw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zvqxecvp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2huaipsbj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2cbncrpca.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nbagkern.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ddykicgi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wbbeitrl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2grjdcwgz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pctkfsao.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lvdzjsdx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rcdbiiyg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cqehyozx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ywoipcnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2skibkqyu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xpiyxxjw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uoogqnro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vybqpckp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fahzobdv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eptxebft.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2prapajpp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cqoxwnzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kbmrvype.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jqxmodes.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dhttgadb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rzwoshta.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nmnymhpz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ioqitnca.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2elqbvsgg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2omvotywf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zdfqjvbp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tyfwmzol.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yfdqswym.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2musqknlc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lactprxi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2enspdahd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2brffxkkq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zyetekug.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fjuycxhb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2daiqtuce.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2esnydabw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vqwnetbh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gasiczsh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eqwwviup.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dpsuffzi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2niqsebxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsndwnhl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ecizcmfb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nlnkokog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhbeotxb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jkkucura.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bsjsyhdo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2sxfrhvzk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cxdehxmj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fkdcjgsw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jogqrbog.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fbdayhor.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2smakcwyt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vwviifro.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hklalesa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ctylvyqv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2kzafnpiy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zbblnuqe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ucschtnv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vyejscpt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nuafmhmn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2lcghxdbp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kztluaea.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jtvfjlte.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2oimebdkf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2azfdrstb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gpsuhnfv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rnrbybyf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gpsqlzff.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ofyyktkn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xpkkgxld.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tvxkwjuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fmrhxnun.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2plcgjdur.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wtpxldul.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sukjbwgs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpaojzlj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bwinsfzv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrrfnrqe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjquhtpz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vuzakqkm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2frowehro.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rrpfdtkl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2guiqdnyv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gspmdzhj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pqhidapj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mturthlb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hxrjniav.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shjxwjqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziodyumb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sjjirnsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofhqoqrd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yotsnqey.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2frgrzixc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mtuqkgny.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ksiegmyc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2oplpzpcb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dxdympnx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2trqjvxyq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qvoaslgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pjprkoje.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wqvtqwfb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lnccvdrz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eoverioh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sghmofit.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pacjjalu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gjqgvlhl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xhggxjqk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2akhnvwyd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xnxgoxxa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ypydsmfd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zsktlhnt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2swgsolzi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2evjngsvl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mzsneuag.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdphjpqw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jkhbxwvb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vjwfkhcf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tuonotat.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wmvaufzo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zihzbdnt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcftwdwr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vktomjgv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2shrqrrtl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2njmmtfpr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dkizhybw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2limzitrl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2yztxggoc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cjeqfvls.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2osjzcpck.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hzgevcrd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jhahrgvg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qskqrjjq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bktkrmfu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2blmrbhpv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lyidezqa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2recpvoxa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwxdpp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2brbipbix.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dedwhrka.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fowwbvnn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xeccnizi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zznffzhl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2yvzoosbw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rdtazpxl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jveeoxcq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hkjqcqtz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tslqtxsb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvasyqy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpavnsuj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pyckgyou.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2czndzopo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2emhoagri.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2orsbbypg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wymlebae.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2pdvdsrgh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uzuykkdm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yqgwshdq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uafrghnp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtufzdr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbeylaj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dmsmvmkf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mrsuusvw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ahnvzaag.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mqsqujzk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmagkbdm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bnllnvav.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2etktbhbr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kilkqjqp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdjranop.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ouhllvqx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2tcfaqepg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziqrwtqv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cknqpcua.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fjikxlze.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wtkxedfg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eloqkmzn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oqjhfmve.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2umgirtma.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2cbajngrt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xxntlewd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2shlnzngr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pvhxscyi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rjerlvea.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2msbqmpea.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2edutccdz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kutaylum.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jsqzqhat.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xtkkldms.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yrdykmdq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ipngirhe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kygygsmw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2sjbcurlp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmfwmko.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2iibatpjz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gailtysm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmglmoz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2aaqigzag.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2podzcpcq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rxvfaraj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2towzsexk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lmqfjwjf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2palksrrr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zzqgimfb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bilpyblq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wzqqrgtk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eifnuwqn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ydlpjomp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cnwsbhcm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pmgsszsa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2iaebqjcn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2huxnljjx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nialcwej.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tbqnxwpl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2pacopblk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2actkkuih.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2pdxxjeqj.html


<!-- 参考信息 -->