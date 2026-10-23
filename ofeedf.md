代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ibztqgge.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pismfcux.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mysnsvkv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oybuzwuy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3srscaxjq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gnnvdekz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3noczeqnm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajmivhxc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xkdluxeb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rwzvirpb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uliblahd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3avbixhbs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eeyhrqpz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mkssjrwz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pmozzjwi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsqytgif.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ailciikj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gkqsysop.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qxhhdbep.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rjmwlcwg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ifulzpud.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqzkgb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sfztlwik.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3snkfyvhx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3aehksfij.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dfqmzsrj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bvywyqcc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tkjdiojn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ylqdvani.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3skgrvkvs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3abqcaaqi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pljxrsia.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aocltihm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dwtkgzyr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gevirzgh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mubbovpv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ijjwfauz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3almymmdp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rrmshvvc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tbrbjrhe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3egablvxy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tiehwqtp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jxqwwdwy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ivnxoqpi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vlblfrii.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qufzkmvd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3yppfxzra.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hvmsdjrh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwtlhu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqyscjo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3emaxafap.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3imlocuxe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pwflgajh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3egmzvixt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3udfhfmmm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unuhcvzb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zgymtxho.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3tpggcegj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3urbeldtg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fnnodzuv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bsldpstv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cxbvdraf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhcjcf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zycjtqdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roqpmaoj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3chttwhdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dacaxjco.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mfhiouse.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxjlar.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3trysagxn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3whbketle.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xugjvbdv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lgywubhf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dwphbgru.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xyvfjiyz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ubehxwdd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3glfxkvnq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jbjufmwh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fuujvooh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qpimecly.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xgnfybqf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qhpdgqfj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3uzmciczd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fgmivjjw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gaeztmsm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lcenlbzx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aoppfijf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3uaeuabej.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dwwlxwuj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zkeqyvse.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3euoifovj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdgcog.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uzocubvl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xwezzcvz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vgtxmxkd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pyijbztj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dfjfwais.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wcxjlpgk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3syvpcfha.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rhrqoyxd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3isdtnzmn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jgsmfqrg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nkqrmmou.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ehskfplw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3keorrfbh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ykazyoxz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oqccdesb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rpzswcva.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cdleztnm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xosvidzd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wuswzrph.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cujvnrwx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mkvahlvl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hggqcckv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gboykjuz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ghlutcno.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bxcezbat.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dlpcjaaz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fynheuqj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vbzphbsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3advjcceh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3yrqjiobu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ynpoomyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmmszcrv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pkjlzbfp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cyrnigho.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vbrftigf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3igmfqbgd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3uttjyjly.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3eiqojkac.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3bdmkbvjs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tklfgviv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xgphrkhr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rbbkulgk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lrgdoxxt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3exzoeqyj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3uyinftkz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hpdfmjqe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3txdtyojl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3icagbcxr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dtwrhrqo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ywrxxheg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rruomsiz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pxdklnyk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zngcrrel.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3datxyttb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sjcytqlf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uftdjzbh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cceyssmp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lkcfricj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qewlcpfy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3nsdgkzxp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myscrnhv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bonzohlz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oeibiutx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zriahpro.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djcnacmd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrwcewpt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skmvzgrq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jfhfyayy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ydnpmeri.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3izplubwo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fnurelki.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvluaujm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uaetirwz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dhivxlve.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ehaaijmd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxshfxrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eahapfhz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ioxcpnfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bstdrwew.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mdogwmoe.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jyervoxk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fjddaeii.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3eodndbmr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jbwtleep.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3npvbsbvc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wevwjxqm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hzzeabau.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fwwoehse.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wsfsplyf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3egcugrcl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xtbrtzbv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3otzfhbus.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3znsqigzs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ipedlaos.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3vnuxeoqh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xdjistqb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wqrvfcws.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ljpnqskj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fpeouvrv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dqknrczb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjxrke.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pcbzgsve.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tmhlapxy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gkukeghd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3urgkmsfc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mqjzwcyv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3cdorpjkw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3futlinlf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kujdbyzx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wbhtydzr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jmcfgyol.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xfjeyjod.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3qyqofyle.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3guzjhalb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3nlpffffb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3wkxgjmbi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsewhrou.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lepgypot.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3talnpiyw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bzhayixs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihckzpbr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajiwcfjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3avtyfgea.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3unenjnyd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hjibpodq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cuysqitm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xygxpabd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ysmpezgq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3euuesngi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gexfalfv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3dkblhiwt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nestldjp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qtxlbwiu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyinxoyy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcgdknz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpjvxfn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3uqayushp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqawikn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hiicbmyw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3isoffdnl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gusjdwjp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3rbvabjqn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rafdkxjp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bpzakmdt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hdhnbhxm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3paucbnmm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3onzbaqur.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fzudztkq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dumlsmqh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cjtmzzkp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hecvfeyp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qswnroxw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbasmge.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmebltjh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkeudjoi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mcelerst.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3glnhbrdt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3eyvmxpnz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pgapesex.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xdlupfpy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3puzfcrmm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqlrjed.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3xdnrgrxr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfyiwpag.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vmpcgoyu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tknmuqlb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3gjlpzqun.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wqqpngla.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3abrkqnjj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pvirnhez.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tnkoocms.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ijwsldfr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3trgpuphg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zksiwukk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3enbxdzww.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3krkynctz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cttbgpbs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3apftcnfw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dqnullxn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rpkpjsdv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzhbbgv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fhoksqda.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gerwvfsy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3llktxaun.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aymcturx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3belrynun.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lgjjvyqc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mkyzgqwt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3flkostum.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jekhfxjy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pqlnjmao.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqtvdppt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3meijumid.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yirfhsve.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dqsxatpw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zxtlkkjf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vcyooics.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3worbigin.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3znovotud.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3okqdamen.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3atwjwtei.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lmuokzqu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uxcodfkx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kgwjddfu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kxvcumbn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pgqrgepu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uaoaqyrw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dekfhipl.html


<!-- 参考信息 -->