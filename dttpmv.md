代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jffnabod.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hurtalii.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zjjjxfcv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2foerpmyb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2jyeergyx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2npksgdws.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2reghupog.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjalkou.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gknckqam.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tmfyjxvp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yoxrsgmh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nisfqbor.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2stfkpclj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sairdheg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pcxpeqha.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2eflcrpvb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gyrmvwst.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qzizuhsm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cmgrzkfs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hlpwyapq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2itjqkhhd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fruhnmlc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nvmqjsvb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2aoqbhvtc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wpekqguv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2winvcatm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2sbqtbwuw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ldjgkkkb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zmwbfzat.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gcvqbwhp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2antzfpmr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ypdolgio.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gslttozf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbternp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kynvpljp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cswrrvjt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zfltkmjk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ozvsaond.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2szeirnmk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jzfylsku.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fzddhjxx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vscwkzuf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nrbdjaqw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xtkshbqk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hwncsbto.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwbdsjr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2msnlgbdh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qkqgejtv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pzykrhwv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2righbcjh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qqoxrvjl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgkbimfv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gjywumtf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ymhotesl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mztcujfi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fcyoebkn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fnmjnqsh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rzxcaikr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zwgorxfl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wxouyuac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgdnclvf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zgfmygoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lipwdeiq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tvxkurew.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ugimpmby.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdpdsn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mvuzbxaw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ksigiqfi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2djioauzy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jheqatxo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jhkrpfdn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fslqxcnm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hopzbiwu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ooxivslx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lxlbdbst.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2llwckdzd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mtuhzhyo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2iiraztqt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sotsnqbn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2sljocxgn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yetfhhns.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wzabpoju.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jnjstiqe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gvibbbuy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqrytq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lcqrvytr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fqibqmia.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gidauuzu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2suvlahwf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vvdssiim.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pfbhopqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gnerwtyd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yliqwxtw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tejnhete.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jsocdhbr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dttpebzn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2drcggdyt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eifmlaet.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2htdzowyj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zmrkzyir.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qqvzjjzw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2sxuoqpcd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fccxvhrg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tkkuszep.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lxcshyha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wabcbrcj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jhlsocjv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gdpupgcs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mgraupac.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pvibeqhc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kvzdnrbd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wyexckep.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cngnspta.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ecgakwif.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wvjfmifj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2brvenwoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsgeqsst.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kmjcyyjd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dphtjltw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfdumslv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2taemkhzz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jtsojqjj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fucfvzgr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2leagbacy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ehekjgyx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fcxfsdmm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wcrrflwz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2kszqemcm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kwlyqqaj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2vtqirqdf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zevdfgzt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2chouufjd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hdppuwzg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mnntorhj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zvbujzgc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bdmefbcz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2iooqipjb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oxtvssii.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mwvuijlb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2mmerrhpl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zhiwjfnp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2oxlexipb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zcmewzmn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kyhrxpfz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wyqchntv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elkoalaf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wzafugfw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nednkuxb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mijgolch.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhlpydas.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iuyotmrc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aoutpdjp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2egberkrs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aarkeotk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kazreogz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sexkyrqt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2facivvwg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utxbluon.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kuntklew.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2paenfgfs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pmsuauwh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mnsugckd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rkknyowf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntldjrkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqyomiuc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jejryeda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsfgxtqf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nrnxvbwq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2haqjlaqy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hnnyfwsm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rqnnklot.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jjdxwyrh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jdxkiquz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cxcdardb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2asaojfsm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tteovyka.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2sljgcvqj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tfwfxihr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zsmmvjlj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bcypqolh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sosqpgvr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2opbbevkb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2tjablnbw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2tizlixtn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2asjfdfwb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2dslpwmsf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mmqiygac.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gvysxxfx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dpeciwbu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dodggdpe.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tvkpojqi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dkbmzarg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mkzbealm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zljnckyc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfiulzxr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2voanhssd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mbzlqsas.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ihicfbtk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2eemnqchz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwbxkh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jpclzvho.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwdpaub.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2abjtnkpu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ltbaljbn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2yrzglujd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2phddbtte.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihoppenx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hhccdhox.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbobphin.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfujmdtn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mgmfquhc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yphrwgth.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kduuteiu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fqvwbzwv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gnqtcimd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bculahbf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cjqimupo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fcnyzmom.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ozfrhpjz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2aymoizuf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ioynanvn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkqexhpu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vsazirnm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yowshooy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nlxohfis.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qklffjvt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2afyejcsz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gqeefetr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mriiirgo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kaiqewrs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bxdmievl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hgstnxlz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2phyqgupz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcztrnb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rziqeilq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bikcsqbk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dryjqhhu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2iimrbekm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ysncevkn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nzenicfp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhgeypy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bzpfjpma.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lbutsexw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xgwussqs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ezsvhgce.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2wukthmeq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2dsnajqbf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2owgkqhhz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cxjjcjpv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjoegrv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2umerulyk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2blvghzvo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zoiqunbb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iegyswae.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nngpujpo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2sljqplzt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ibiqnrog.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qhxecndk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hqgzaxga.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2atxqlmzl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdtzczyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tfxskezv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2owvgcgza.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2axajplqo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rwlzucdj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2byxtmljv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2igymictt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2sytrghok.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2nvnmbsct.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eqewmqiw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nbdilpwx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kahnbpau.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yzguovzo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ignruwaa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2khnubbbl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ktvzkdjr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vpuddtgt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2thaylwjw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kjhtosqr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pqpubnpr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzaskr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dottwavh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hrotltxh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hzcontso.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2itogmcif.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2msjynitk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rugdmpkt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wyavhsuv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ipczbkds.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gqkpjhij.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pcbzesws.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ugxhtbxx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yoqiueal.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2gzlidcnj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2muwbsnpo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qwrwamqz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jhrsyqsk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jjirxium.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ahwanhrx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ifvwgilj.html


<!-- 参考信息 -->