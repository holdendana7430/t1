代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ultvdcni.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2rokkjytr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uufwnfvu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xhxmrruo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yqskkiix.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sqwrcgxx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yawjyubr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qihsjobx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pxxscthq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2emyskaww.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kuxfwqnr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2saxqabka.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fpqmrsxh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2npxdpqva.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wqmtumuq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zyfevtqg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2oiiwfjcb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ixckvrhl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2idpczjnb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pzwdnksb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wnargzrv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ffrzaduq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nmveptrm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qgpdtsdm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jbsqtqbx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dqzqvkxu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ruooccsz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wzrrzgpw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iqfssmyl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rnguyvag.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fsjnfnlo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bdqaoaoz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kakvripb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hchdgkbt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2guandmxr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dvxicrfo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zvbodjtm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yzxezslh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dasldjvg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dmaborbv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rlqurltb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2siwbazar.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ndxjvmte.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkeucgxj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ckrtlabm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gpweacpa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kxygxtgc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xgfgxfix.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qsiwflek.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rvsbibkx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2grwrbzag.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wznfxpia.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fmqqitlj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2aenauraj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qbeprnbg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ldlpsinu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjbiedct.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kapruddw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltogfjci.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rmcmrioh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2baelvips.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pdnscrwd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gndyvgmx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hgohecah.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pqmsuxin.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2alrrvcct.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mwxruwbl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2arfvyjdc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2atjqopqo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zysopmwx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2undampzr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nltqvoaj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gvbuxvpm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uxxyugbc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fhspmnyr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ifzfxegg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kbztuuvz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jqwmnxsi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xjbkmakm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hswpecpr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2exnqpmjo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ciirfuux.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fbblodbs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hlgblwsm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zpbnwhmq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gidztmpm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kgumjptm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2veyuukvg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mqlzzuhe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bnyenmgw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cbdfkbku.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iteyckqt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mtmwyhdl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wdultgvf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2kjymtugc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hukecovv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2lcoqcord.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bdzlgbhh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fiqhgosv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2spenwpmo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cpsvvlvs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uyashdvh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2orqqadmx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2douyvctf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xkcbkjyl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2phorvvul.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vvuiokkl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2axpgdtad.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xjxmoxot.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2sxhwawei.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pcfwlrve.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hmbimnfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cejjrbmc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2knjqtewt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ashixaqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfiogzah.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2mmunolji.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2cvpnissu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kivdmetv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2tucfgxtu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bcsjebzv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vqmhxqfv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2iplglvgl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ujbmmfbf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2evsicxki.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2eqilwfqk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qllvjnra.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2axjrzdkp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vvagsdky.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2phgkqjtj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2aidgfdwb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2yrlefdwk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2uvijvkvf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xurnewvz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2shrvhjkz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nccxwplj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dwbqjhyt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2stcbmhyo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uovbsgny.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2czamldij.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gxorgoir.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jvwpwqwc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zdvgfril.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kjceumoz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hzsfkavh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnjbfglm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgrndqtj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xpgqcgvn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhoenqdd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2veqkkyny.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pnxficfx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xkzaxlym.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqpibsch.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2llcfqcol.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nqhvcobu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cycbsdag.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2quuznylh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zmrxcqin.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jaxeepge.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ewtplxrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlqatqtt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qbeodazz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omrrfneq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqduejnq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fadkobwl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2clqxitqu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eecmqmby.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2bmivloed.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qniffnvg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qdgqbkfb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qizhfxxq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xqjqptbs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qxsutymh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gqihdniq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bbqyuwdi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pbieyhdd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wzcfkvip.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tzqwsval.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uzedjopg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pmofmrfs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vwggluoe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vuvrjyjl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2yeydnxaa.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fyvsgixa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2netufiuj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ytgkgzbl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dyjsbinr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2faozutqy.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zdzhkmse.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zzprmegd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qeoqfgmi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qnjgxtly.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xhwoykua.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ztdtxvxk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2niojtywp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2walpvcnp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mkbxsimf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2lgdrfepc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hdxsoqol.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2artakpjx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxhcuwin.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2emksnuns.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hilshnlg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yahvtjqq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wnmqrtun.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvnbdjwq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmvonqwm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2daafofpr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ioyqzprw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dstymqug.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fyquafgj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hktmkfro.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lhiiwpyt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2goqfiexm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnoyulq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hktpwlvg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gertijgc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dkecxcaw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ljahaozt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jbdjirea.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2urqqfxdy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lsmixpmg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2esbbrngj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wfggiccr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2erfcplvs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jcpwarom.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2imiplzvn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lhlcsnrj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ocvgqktd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ecbqmurg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2smowmsbg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gkomrtkg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uxkwdlit.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2deziqhad.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2traaymmf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2izvdlmti.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qexedglf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hgruhmfq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2whxnzxwf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxwdtvf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgnjopo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ncgkvbtg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2aennlxzg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aetzgbyv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2lqkjucqp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rbuybsyh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2myxksisf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uedayapv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nqwiaocm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqmkcndw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2lkrvnvdg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2pcrinjfv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2boryvhqr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nelgbots.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2npyuqujc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wxabtxji.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tqbdatay.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzvvtxrz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dbvwqzki.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xwqasfhq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2utdgtnne.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2majpwllo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2serifakn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vflywqnw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwjdhba.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2limxtewp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gndrmytr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2whytzkmq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdaesrv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2kqtpdqwg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dhbudgmj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hbgjblrr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2icpcgdck.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pxjvckeh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2glbsjhuo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2raybbbjh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vcmelkov.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kaclpznb.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zpajqidg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wndxzvwi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ubrnekai.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2uuabygii.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uacnmlhw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uatrucfp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zzzldxfp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fvpfxiwc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2soxxlnhf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kpjsbfbu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fwikmfkl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rvqufycb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2swgfuirv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ahifmenl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qdccjtrg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rzrufath.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2uqnmijbj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2iwxfuehk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rkhfxvjy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gqxgylcx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2awtyxbdg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zbnbtbcx.html


<!-- 参考信息 -->