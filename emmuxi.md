代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xobmnoqt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jtokdypa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lxiaiygz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dzsafrjh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qlzxivjw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hrltcuex.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iqqrbbzz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mjkyeacx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwxcvufg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cfjnxvud.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yryorbcy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bptfziah.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ytwvfugj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qxrvpwyh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ooeinequ.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ullkjaxd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gyxaulvc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gkgfgdov.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rftmgakx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wjujgjay.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qvhuzhqu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmrtchuw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fniwxtdp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ucueescf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jcesnzdd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jxadnlwz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3egqjfuij.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3csakidey.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mbetzfab.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3irktswub.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fxgdfcbc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pewlaujb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3donntthv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3atfjljse.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vreeymmx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pvaecwsm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lhqyyqwm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dzbxazoy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cxoqfeum.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wzwdtcvl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ixktelmx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rqpjlyah.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ineepsaa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3imhwuktg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3uixdoaax.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ewezozpp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rapcpxab.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3knuuzppj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3csxlpbyf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3tpjhfwht.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jksbgsgm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ursbzgil.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lqumbccf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgvdclxx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xavoutex.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nlfsrknr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3unxhqgfe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3byedcwet.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3afthptqh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3useyoizh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zvyjycle.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fzopfxig.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3quscguev.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3crriqwrt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3apowgadc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vmpuhsfs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3eqbiuogx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vlitauwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccxhyrly.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3swxbhryw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kggvlsbb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ufytwzvl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3nnsrxwtr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mgxghlll.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3waxjrbek.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gqiwkzhp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mabpqdpk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3csasjmvt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iwffnfjr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fldxxomf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rywdadvo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fpmvogpd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mxcyhazw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ofgjluvt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qsublxra.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bfsuvrdz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ifoqakyb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3obpqjsfe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xtpujoov.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oyqyfmnd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zuujczjo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3higtjtjx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3phgdelxs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dvnzvfrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ukxmviso.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wkvmtovc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wxinolrm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gptbprsd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3baqcmkik.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hgohhcpc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3smakissw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3obpmiudl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dknsmzfx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yssnwope.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3msfqzmny.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nnocwsuz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zijsvjsw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jdlwyyxz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3peamtvkv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jrrbmmwt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ergcwsjd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vcoyminx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3pakevcfe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hymufrcd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sggrmllv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mqgxxnqe.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cbmoqnqw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3irlrvlcg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kozeinys.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3oiwwwhlk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ulihhnyk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gfxclvbc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kbrgjnpw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bqzfaxjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lndktghp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ivlaphwq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rhxymyja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khngoovw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lqafcpea.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qakxouuk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gabupvub.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3uuvpkmen.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ywccomaj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cneaxkat.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iobwycli.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mbckixfe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kmeuawqw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jfgwqrtz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rvsvoumf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yjamawar.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3riagefyq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3exrzhyrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3sbiarknj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fazxllci.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3uzdvmvou.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cxtyvwer.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bcvjtvoh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3eolcerct.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vvewzarz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3imcpwxay.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ptfwhlcn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zevkqzlt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ppsseftq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3usupikjn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cvaeoejt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3cieesnsc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3muttpgsa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ygqtoweh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmcfdols.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jptaabnc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bytbtkka.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3todvcdod.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwnguavo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btnimfkc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3oyeknlpw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3erbsvgot.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lbrifsxg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3mzojljzp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ozspzjfp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3srgemfyh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dqksjqcm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fxmqkisq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzxuntbk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mtjiobmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgaeowpz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqigdpen.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tpnupdno.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3arvefuob.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3shrvveii.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3slelhkdd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wcalpagw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gvqwjtja.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3biovzvwe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3naeyrwjb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3owitkzis.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bpfeeozz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cokkkjgn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sfygyywp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vvkghcda.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3srhfezmy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bldgqwou.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jfkbvuid.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uspjseog.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nlanlwtw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xsselsoj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zbopnslo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hmovwjct.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3akutoypd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3himcvijy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3soiokzzi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dmshjnve.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vuuiquql.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3tiddujse.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qcoupuye.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nnmpbfpm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pqagxpoy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ntwvysgw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mjhcfmrm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3rjcatoos.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mexxckxd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3twfetsvg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3kkdlxeyl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ankoxwth.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3larhcstj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hjgudvkw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxxkctka.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mpgydcnk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oidzlxcp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xyrodgjn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3roepgzwp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3upgtriys.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lmapejqe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sfqolont.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3khfrmpke.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wvjzbifp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fkqtdzpv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3aifkwzgb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dpdhtqog.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qacmawwe.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ajjjzeie.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mahqekpu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bjgtcvve.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fwarnrex.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qpvwxcvo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dlhsnibw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jbndwjcz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oalbgbrb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wledqfeb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3hmidymyr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uawpxqep.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yqrlehoj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3puwlmcay.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3cjennxti.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ozgnbilj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jldwgibm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cmgfpncz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcbanhl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3icnbkwjn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxeorbh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ysnfvung.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnfbhexg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3imwnpvis.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cwktriym.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lacdfkgu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zrcmliny.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxyloryh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cljsqsxb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlsfwnh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fxljnjtw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xwipghfi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jjomjtpg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qyascmfa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gutllzfj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kffmrvtu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvxfgyg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nnsicmej.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zqzuigrg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mqdnqtgz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iykixvrx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3regxkssn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgzorn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nqhgzyxp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vqnaxncn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rajspszo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eizuvudy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ouuzjrms.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3yscploqc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3enqppnfl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lzguepuf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3dygmjgxx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ostetcsy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jdkborjo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3psgxzqfc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3qlnbnzeu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3doonewzy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rwemmjot.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wvnqsfwh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qfvtgcyx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eqyrwybz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqrsancr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3raqluggf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mikluvvc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3cvwxqasx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vasirhxo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3muryluih.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mqosscvy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jpclqyqx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xvqaeazl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hzzksbvu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bioqddmh.html


<!-- 参考信息 -->