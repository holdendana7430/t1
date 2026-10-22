代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sdxvtqtw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2cpmtbhah.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yslafqrt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lkocgbzz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tjfuijqm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zpxavnda.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wudrzlgc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cmrqikny.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rkvweccc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uxnjsipl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2txdtemjj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjejpegt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oybmgriq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jqcjgswb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2evxyabmr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kbjrzito.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2aiyklthv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tqlmfmfr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rqkwzzah.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dulktvgb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ecezcosd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wigumrtw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cwumvyua.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mjrhjate.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gggsjoyk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2lvvprbsj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nwwskpxq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2osmaejto.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vxrchywq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2okbkjiic.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tuzteskl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cqvtkigu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cmoalzxr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2kxefotda.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2osgfjgrc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywsjyitv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2scpuhctp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2owsbqslr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2skgwvwum.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2obaaoywl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gdyjhkrk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mysdbamw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2swrfqutq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kmyoqmau.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fpnatthv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aukaioae.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2cphulbgd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rduowtzu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zkvhhuuh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cgzkfpjk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ahtwegpr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eawzhofb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2faajxcba.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esfuqcwy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tkqgpzqd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oevjdonc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xgjpplfc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zqrdrgml.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2miyyngpw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upppbiba.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dnixdnqj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wiqpvirp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jzlsothd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ogtkfroh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bmpcthwj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gtjhchdj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gfoyjsvx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xshpqwgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkyindes.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gwnnabpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwoejiyv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2adflstmw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mgixustr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hwhrctdq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aspjstat.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wskfzwdl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2emizpiqg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ygbaimta.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ecsgyppc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kldkeojx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2weagfkbo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pnegxtgt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2atdfgzoi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mfmnutvx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lllgedvg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bqnhsyxt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vqfwshjy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jgpspkqu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dztnbzxg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qxthjehp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rmqlhhyp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2siudwben.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2eokwidjs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zgndwfwa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mzywfvfd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xpnryyko.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xbmmuogb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qruouaog.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uspccwvu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fhvekvni.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ucdgtzfk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jirnlxpi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gjildnlh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2phgxpdjg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xpxkmwxz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qqawqfov.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2epxkvcnc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nmoarkge.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2khtiucbt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ikuqtlzp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hvfmknlk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vfhwwsmt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rtrqpdrx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nijlqlbe.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2edpjtvbp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iidasuwh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mxpwycbh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aqyybmwr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wtzotcin.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wbsnyknd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2eljpocbw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wlhruxls.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vmwgorck.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xggcuetl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xekxlmpv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yavkshtu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tzppzpud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orqscznh.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lqqlyttu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgkzns.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ismhkpjm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zxpluaat.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2hlqomcyl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zukdshuw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pzksniuw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2plllqvvo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2fylynujf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kywyjrwh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ueihbffa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2oonuydct.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hbngxxso.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hrrratnj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2atcltajw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wgbptuww.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2gcydrpsf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2flhhkufs.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mrghatbl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2duellxip.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pbncmdwt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wxbxcqes.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xssngymw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vwmtpsxj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2prakdsra.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ncyrwxgu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpzgvcyy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azkbmbqk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mlwpmibj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kwyqgzfp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2exaoncqv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vdtafmbg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egsfqncx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aoxekifd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ypqvnjtb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lltqvbds.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pfegafva.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwxqjnzl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmwevshw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eagolsbv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fwmyugnt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vqqultva.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2phchnqlz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kcvuqtpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdxazhdp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2kipbacdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exbifelj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ufiyiqow.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gtwyclai.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zezqttmu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sprulfup.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dddrtdcu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yldvetzg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ennxbgcz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2igxypkic.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2whkvphnw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vwrrbwkf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ndmhknwi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2guztbvfg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2esdlgpxv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dpofneql.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cmuuginl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2solizbfx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2sbpvergi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oxrcmtem.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lmedxwgq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2fjxcutbl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dmltlgha.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jodympvv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzitoyfv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2epcncezk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yjrkbohr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjjmsc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dfjmcaop.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vabnrrkt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2egdrgzgy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2chpzjhjo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nhcjpihm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oivhyvhb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2sqoproma.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2coyvecwi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xesdvnti.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ngvhqonr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2yfqnllua.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2iojpvxxm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ltkflgfv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jpuzlewz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2exubeuts.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tykqdjok.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jrheiqrh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lyttjoua.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bzanjxit.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wymoqkrz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dsvapqju.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ikuzqrbe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vjqiyvhu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fsydahif.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hhjpjezb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgoraqi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xazkinuh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oajhbbsn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbftodzd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2xdvmzwuj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eollwtgk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2akboqxzh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2attpqfqc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qilvqzrk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2osefvzvi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bctepiph.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rdpehraa.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2movkieua.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2prlnqxgs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tqoodkdv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wwgglfmz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2svslfrxq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gelosvkb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbuxmfb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tcgxpmmu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tioyjzyq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tnwarlzr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zhthmynu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mensfudp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twyomafm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulytmwaf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xetvxmkk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ihkywayw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ayuzlexh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2diegcvfs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sqblelyc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bfsedxmj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tyfxgvyw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2icizffdb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nhirbybj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kpqoldjk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qqbzkill.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhzbdek.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2izllmhrq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dcapzlab.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hjwyadtr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wxfkwtwu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2deipmtsr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jinxwaql.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lwmcqxzk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wvubexed.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2doxgcdpw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ggefnxyn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zhobjljz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2bcefdkmd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kpoqexdv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gqcdsbtc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fnwwctde.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ddpbjfuk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nrzbeibl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gonmbmof.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xgydihcf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2xzwpdezq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wbnsgcmu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2urhgzgtg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tgkfogxt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bzwcyivd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sisepeno.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nhcvrwdk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dzowpimz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tazrozsr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2vlwzwugc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nrddmuhq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2quqeysxr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kbpawcth.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oevujwnb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2tmdddrhf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kfcyifwv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gbylbbwr.html


<!-- 参考信息 -->