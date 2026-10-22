代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dlxqmhgi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nuhrfpki.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dbkhaepr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2celwmgmq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rqbhnivr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2eioepbeo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jmonfecn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nvrabbcc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dvqguupy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nugefwin.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2upvbufem.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyfusdje.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ivsddunb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pwshigbs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bpiutesi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mjpkofwx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yhvccqek.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kyftygal.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ivtdmcct.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mmumrjfi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cmffwhii.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uswhpnse.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ldbjtbdl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2iuqslggs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qcexunsm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lcrrpanm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ixvlfnsq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lypwpuor.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ihbvgmws.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xdlqnxuq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bgppuiue.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xddnhpeu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2epqoearo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2grbjdzio.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ypoglhkx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nfpbkrgv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ahshqurd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2leecgptk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hffymdzx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ndxzgydq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xfzikigk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2agbrkdwc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ogpnftmp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zdkuzdkr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ckcsfnig.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2szzfrjxs.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xggnkmxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fwimjttt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jmkisyts.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fyzfijel.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sbpyudpz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uuprmtum.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yepsvcrv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2okmusoqj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bhhtefzb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2kxsudsoc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gwcqtczo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qjxyzlvj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2upeodskn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2knznwqof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxsavhvv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zjzkbjnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpcntvce.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2uwlopyxz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nrwbnhom.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hqmifeky.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2serurdun.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rfettuiu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqxskopq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qugienfo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qekmlfrn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2syohoykv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zngyhfaz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lrxwnqwp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fwjnqski.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hynwugks.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hhdvkzor.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2dxtgzqxf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2azhhsyei.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ptvhizwl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cgxstvkx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ehcnksow.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lyoxlkqo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2azklyeos.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kwnnmzns.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2atrrtcht.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tadpbbod.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tdabpsix.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2pztmirgp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cbxcutty.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ihcamcrh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mmcjsrmj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thjdopvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wbzripor.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2awbzyngo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ayopnqab.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rxvvbjsa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fldsnweb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2yfnswdaw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2djgdqxwm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2adgkwmuh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fkouanwn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kwzuixlq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2cgzsxctk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2whhqulfz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iaeybfty.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2wqqjkxlt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2chzosxvs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2loenhwos.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2blvcnqli.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2sfsvcxhv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vlkbrliq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dccqfwnx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hbdplxbj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kiapnmnt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fzpupabn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrxmaleb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tzxodtyp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2yvdknzul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffkzpefy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2hdfstttl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2irivyamx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rgllcbni.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mmmolrpl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2aujygeuz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rpjfaxjk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2apudyeqp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2kgiwiowm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rleboulv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2orxconmd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gwtbtonc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ctmtuoku.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ixnbxtxi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wkufmqkr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tskaqgjr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2illkftgs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2bsepqrqr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2linhhwjt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2zguennwa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jxpkvzjz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kryroxti.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2woyjrcwd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tpkacyti.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vfxmqbux.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2erfowrgm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tbuqoknq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2llltuaxx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ncizmkof.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2buxyzsoi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iubgzaem.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vdgdtgdq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xwnqeegp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnlvgqem.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2duetxqsc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2huxfdben.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wdhimbtt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yddjcpsj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kvwlrgyn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwuwfvks.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ualnqfot.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2splxfpab.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2igszvurw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gmrsftuw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvvesgpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktaqzbih.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgsungyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mblyygyn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wznobcgz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tsduqbqp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dllgndid.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kodevrgk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xdqsdtge.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mkhctiup.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hjfaokof.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tcduxkjf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uyvhstxx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2wdawpoys.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pxhfwceo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2okpkmxws.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tapcuviq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2memsqysf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tbbebqrx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2sfaqdmnf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dprpntsp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pdlkgqul.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2scbvosvi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jqyqfrvr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mgbttufg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aepfmctg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lsnkjlxh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nfmeolga.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mvqttqhc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2prgndvvp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fzwgezmh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhpnpuew.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sflgbagf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2iqiycihy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2pqjcqpja.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wiaveyun.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ssjdeeqz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jrvvcclx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jiivvawl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mzqtkpwd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2rbchhghk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypoxlvvj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wnymmypy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2isjluhzi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2okyocpzy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ounkezxw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ruglbzak.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xrvakkju.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xviqpzga.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xouxlnbz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nmtallgs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2jjkrygcv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2smystawl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hpqecawq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cxcxstob.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fesgjycb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vvqldlao.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gesabaon.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2oydzvmgt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ncbdwexi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxthwgv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2resxusuc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dtkiacuv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gjaukbdk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2brrwcwis.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2krwrqose.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ftslzayh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wpjzhdwt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iioohiyc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsrofig.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fofclbkv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2avyyfzhe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bwpgfyyi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2szgimqey.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lseqlapi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkmgkoa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tkfocsgk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvvswwc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ogxvihwd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbmlfio.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2saqmyjlx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nszczzph.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2emltutco.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ggoezvte.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhuebamh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ivtzewna.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ukxcbays.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kmflzuxv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gxdkqile.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yktpnatj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2swoiueqe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2jdckbjqz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgqjgil.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gueigkls.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mpeihqrm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2gawzedzy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2atscytww.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2phzbptic.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aznwypny.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hjiueemz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2odwzuppe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hwlcjyup.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gihqnkqy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ccqebhrd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddjzhdmd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmmawcv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mfdeczjv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eofzwcor.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jrbrqaut.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tespxiqi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bmmzyetb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nttlaoii.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2aeauevfp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mgrhebbv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kbidsprx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uhbmtcdr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qvoqjirb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2idfzpkau.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jtpmnnpk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lwjjulua.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hcnunzvd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nbynnxux.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cnlncdli.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qjjjtxgv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xeddwtpj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzgurb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ckkvveob.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rxzhttst.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ipvrldsh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2twbhstqj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2opbjzlvy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vafigtfo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eufemyug.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2worwcskh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rexoqbwn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xghjdndy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xybgvnvt.html


<!-- 参考信息 -->