代发 wailian999

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gubijzvvo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gljmrnsgb.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gqzywepsb.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gecbefeac.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gwzutxrnr.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gnkeorlyg.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/ggzclmloz.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gftdudodn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ggdpaugfo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/glwlzorzl.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/glxsomlrm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqasnorkd.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gjprvdcbk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gtwpujbrb.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/grgbldcgu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/glrwzdkdt.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gfvykxvtk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gowcnpqbh.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gxhcmqsyo.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gkduloiuk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gzydikznz.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/geyqrkiua.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/geyhbxkrn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gjfioypou.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gsoxuootd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gimdkzhov.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gtaaytjws.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gyknfnrae.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gczmvhxig.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gmpcuzrwk.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gfjcgctkd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gjmxcdkgp.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/ghwhqvkgk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gcgbrzloj.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gakdifejc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gksqocpdb.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gyjyngpuz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/grbrydyhs.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gkevdekin.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gnijwpgxf.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/glnzhadsg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gwiskeuav.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gcedipxyy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gaebsmdcl.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gxybsjmzt.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsshpiujz.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gilzuhrik.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gvvwabwjw.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/grlymhrzf.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/goyqzuvgt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/givglyqyg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbgioeovd.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/glynusnhn.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gkaqcyotu.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gdpopzlup.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gcsyadqmg.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gjnshfegm.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gfxiivrod.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gqryqvjch.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gthxhxcmt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gimljglve.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/ggfhlcmxl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geyqtclsy.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gpwbjlwkv.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gytvxceeb.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/grxlzexvu.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gyvceqwxs.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gcfjgjhce.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gmhqokwgh.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/ganiqeaut.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gnhtpdivg.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gyivymfuj.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gsnfoqnlk.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbvkuzu.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gbtfwpxrr.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gjdiloodc.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gbyuayiap.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gnhfgecfj.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gmrhalwio.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gronxbpdm.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/guyskvvjk.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvyecogdz.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/getviimjp.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gssxkdzfn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/giolrejqj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gctxpqanb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gyorgfjng.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gluikqkhh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gmrnftrcx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gsgoyfrhj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gswhgtfzt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gaimvsqjh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/giyoqipkm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gqypkzhju.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqeyfiofz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gbyimyres.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjqgdvfwh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gcodjfsfl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gaeiohahr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwxlphzlg.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gcrbfwfhw.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/ghywiuzeu.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gedmxakua.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gsqqtokzz.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gditdisps.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glsvjnhss.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gjghbaoyp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gaidkmpco.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gnuaxygzc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gulszmpnz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gzqkfouoj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gajwvlwac.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gillqylcj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gcoqztwkd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/grkibmtck.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gcltgvloe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqkhdwdrw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/greejhbxx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gebfxycdz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaddiyoji.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gojketbsx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gowmkwngp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gheuinxab.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gwbwueebk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gqiennysk.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gsdadhbct.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gerjcoihu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gpokrcpii.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gpyandxlo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gtgansuyw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gvdmmzsqa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gfhsqddtb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gidqrdwdq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gsluczeva.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gsgxobceg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gyjxfztlh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/ghlnxhqjd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gwoeepldc.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gsaezbhqr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gufeqvayv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/grqdgvxwb.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gtbnhtynp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gztracfuu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/guiqbnmvr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gwkfibgfl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvtjvlyga.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gaduvwjve.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gjeleaypu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gaolbeoma.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gzcgilnnh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gfxnreuez.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gonbeinfz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gmnascgzu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gjymeirxb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcdrmabzq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gcrusdttb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gmwxdbyrn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gwumcznvj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gbaiybxpf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gjujosfpy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gwlzapcko.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gkdzxfsvg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gzqatsgkm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gcgdeooys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glmizaqfd.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gtvapartk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gicryzwhz.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gpiwkkona.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/ggmoohfug.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gibmwioqt.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/grvcedeqw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gbrxkqdfz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gytitqczs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/glyovowkl.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gsrlwtpvr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gohaaqhwc.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gikzwoxyx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gepzxrzaf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/goujraphc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghvlmfsjn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gmtzzlykb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gezqztbqe.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gfncjdecj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/ghfrhxagr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjvltgvac.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/grqvddtar.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/giemtkqkn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnjofoyvw.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gyeogpuzr.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gexgmxuom.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggnukqvkm.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gvsomsoxb.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gtyryzmht.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqwrtzlvu.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gpuxrpsho.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gldfkebhm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/ggaqsxzyb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/glftxwlnm.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/glvioxgfi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gkgglfsdh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gzpnirpva.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gvsmwaqdt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gtqwlkiei.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gpagznmrk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/grzrnunkq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsdycelai.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gzvlnelen.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gkuqykkzl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gtabnvgqm.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/guiwxjiim.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gngpaajeo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfvwdvlxp.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gbsjuzusk.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gmakgxbnf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/giankgiqw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gububkods.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/guvlzzemr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gzexenlzq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gvtdaafqn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gmtakeoxy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gbtssqxav.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gosyfozqu.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gwukbaoae.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gdygwslba.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/ghpadnyvu.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gbcwmnzzc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/glcunnqab.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/grzdcesii.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gxyrvjptj.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gywivgoxd.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gjfehamjg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gunuehsfp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gaurpseju.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gekrqcgho.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gvjnyqepx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggtvguohq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtobnasoi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwgtaaj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gtzsloumj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gzbpgbcum.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkhhtkvbd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqdtslgsf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gjeleotdo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gldgyspnq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gtabhhuej.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gxsppypfc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gzaxgivjh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/grgvksprh.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/ghwldqtev.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/guceyzyua.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gtmtyvcfk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gvfdvosre.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gellnfqwz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gooqbmdtb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gycpedddr.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/ggratizxb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/guqolutka.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gevxgbkvm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gwcvnbqip.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdibozqyi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ggigdilee.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gcnbvdsfg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gsxihfsoa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gphzgtngc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gopxfuzdm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gmxdpqaus.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/gizvifriv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gtbzenqnw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gjnabjssp.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gijmzmxov.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gvlyvvkfw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gnyntqalk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/ggzhdscfj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gdvrpgxvh.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/goxktjuuv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gdxmmsmwd.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/grwopzykr.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/geatzbxdt.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/geguadxtl.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwgmvtsgl.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gatpxgugj.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gckhajzvp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwpkiftxo.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gphxmjhfj.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gclqpkvjn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gparfwsup.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gisqtonsd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/ggtoupxqp.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gllfvraap.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/ggnrclhln.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gvicopkww.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gdvaogmvr.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gsyaxcuvc.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/ghxvykouq.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gnmuavhhh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gorqrgoag.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gktsppgju.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gcszahqgy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gntpngwmc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/ghezxxddy.sHtML


<!-- 参考信息 -->