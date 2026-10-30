代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/guvqpqjeo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqaiywk.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gytsbslcp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqvrypaw.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgbaqvb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gidmkcdsr.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gypatmnzr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gzisslzzs.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gazeouuwa.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gsxcbkkrk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gubfhwtmw.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxadnahb.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gutiwnqiw.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyraagbnj.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlhplczl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlybjosn.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpsqjijp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/grxvlvmdk.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/glcppfung.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllzkonfz.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gofraqykr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gpftjwogj.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqlnjnwrn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphsiovl.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gzihxamsj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhlabpbg.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiqlpxhr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gseocyzzj.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsjzhiqrl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gpwmfbdri.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gfqrzhwpy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrvttqrj.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gnesqpliw.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gugrekkyw.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gjikwbfvy.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdfapwho.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrcmiebl.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqobvsvg.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzelboxoa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqufadpzr.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/geqaezcqb.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmseiaqpt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/grawplaxk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncrvznwg.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkgvcwr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdpbplzo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrkpecn.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gbfsogdwy.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gdstccpfj.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gnrlxdhtw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gjmtmycyg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gykfzwxbw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjnnamti.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmcewczn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhdnddii.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqattorid.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqrbysllh.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuulojuw.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbcjhakm.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/grynzhtrc.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpjzpaz.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/geihidfcq.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjxddtaw.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafwfucv.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gpvaluxef.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/ghisiwchv.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gagpbwrnm.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gydndxooa.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcitntwi.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gxhidjnzw.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucinmzq.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzjmodkl.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gglyddxad.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqrelztt.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gldavpsch.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzwyrrus.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuvxgqai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcfpernt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyrkjyir.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/glrtaqfjo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnnpsqtq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/granyhuqt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcgdpvto.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqccyhak.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gewhnykct.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gtwcflsyy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlotqbyl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/guuswjnku.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gfwjiqkev.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gdgpaepit.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gutjolsji.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grlkllskv.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwdxwxa.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gizqguzga.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gzrzdfezc.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gofoxgttb.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gstyvxflg.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxzomvec.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpemscfpa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqmuwyvj.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gkfcuhsvr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtsfqlwc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gskrivjwj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/ggftoquhj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhrfyhpi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gvxfhqwfm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gpscvgpmb.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gatnidjet.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guwnrgvpe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwktmucz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gonzdctek.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnolhecvm.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gnrakibtc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gbzbgaakc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/glsladmwv.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gyebsyhbm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gsdyishlz.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gkhavwpic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijttrjse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmvxdrfr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gmblfwsbd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gxetwazdw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoeazktv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gyzkwylfl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmbydfon.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gearpcmmz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gzylygdzc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gxpoiuoyr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gczknaqfc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/guddqrued.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfvdjxcd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/geafkivtf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixtvved.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gylcolugn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbosfvyk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsqmvhdnt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtzsnqn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlhswuwk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiivohjb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppuheykh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gemmyfodh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/giemekilj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjryhkttk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gefedfdgn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gziyxpiep.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gltfajhoh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoczppje.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glfyinbke.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmnphmlld.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbcnmxpyr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gydaybdbh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmybouwr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcwufhyl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxemmitp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkihqjfeo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gttbhpuru.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunbbghyi.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gubxvxnfw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxculncxg.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwkpjcae.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gujgfvneb.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gsirbtjuy.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/guziixuui.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpvfwwpm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwujmxuh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gbofskrws.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxseyxzlx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gzawqpstw.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gigzkbyel.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gaodekfhu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gglcilrmc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdokdrcmn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gdqydwjzx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvurglbq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gscjraeru.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndpchof.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdifilog.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfssasmnu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqfmrvy.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gtiycctof.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwcsfyfs.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiztwrxw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxmbejme.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdzavgiu.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gjvgzvijw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvifeviq.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjijcydih.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoephxzm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnxyquyk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/giczxklbd.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gqsdduadh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gnzyrtsxg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gmfzlhkdd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqholoe.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gwnoxkxdd.sHtML

[A05] 整数除法与取模
来源：http://read.share.fanxiaobao.xyz/Article/details/grzsdgqxc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplienbbz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuobkukg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gskodjsoe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqmorpq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpezuafqh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfqwisve.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkfiotcav.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gebqjbimg.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfvtjcbef.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gwttvesyj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/glhwvrfpr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gboxuhzrp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzepsaym.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gvofkzxul.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gddxujhtd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gyovjholv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/geckaqiya.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/guyczjtnm.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwqvbsqo.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxnudlw.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/glzgeljla.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gpllzasvb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/ggixsuudt.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazdxyfi.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glawslysw.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkwgpcx.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/goivevlkn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqakwbvj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqgcwhw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyssfzmt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwygiwgt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjsncmst.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghbfanmx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/gtcqiykgx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/glgufbhxw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmdaesak.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcmfukqa.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqrlekdy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gafmstflo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzggvbjg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gljrtveoq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwnvxphf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/grulqwhhn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkuigbjtx.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gulevrebd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcigtnjye.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaemeeasb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gofildixw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glziakiun.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsnjvbisy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/ghsabgnhj.sHtML

Ruby: rand(1..100)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhewtgfe.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gourtwioc.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrzznal.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfoimxqq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/guezsgwbm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gndwzauqn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gaccalceg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gkgzhtqqr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/gavxpyefj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gdfusfhth.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnqlylwx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqcqcgrx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfocdktqw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncczvasd.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/ggqcdxurv.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfvzihq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gwpnfmrhr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gacbhcves.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqrkclir.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gjiqbmtub.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkysbir.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkswsrbm.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gssaoefru.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwhjrwf.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkavrtz.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gotxdqofc.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gmeywjdew.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glirlzgzh.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzjntrwd.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/gwhlmrkah.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fanxiaobao.xyz/Article/details/gypekaktm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjjaequf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubxovwko.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/grlnaubey.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnlocjdi.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gdjdutmgi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gognhodxj.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gjtnlpbli.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkindhgfa.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/guzdxtmxc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gjrmfolee.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gylkgkhhf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbwigxay.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwaomwur.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/grrhtfwye.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/grazusyii.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuqaqgyy.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbiixmb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdctimbw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gayjzofcp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gabsfyxoc.sHtML

TS:   if (!x) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gorjttxdf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkizucv.sHtML


<!-- 参考信息 -->