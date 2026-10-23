代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ifzkzndi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ehbjkmxt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xjxkfjby.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uabrztfm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3glmoncth.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iksoiuxc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jmiansyl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3umbnpzco.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jifcztcs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rzttagsh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3woafthdg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jahzkfah.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usmhuksu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gpovdhln.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dzfrehbg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwiyogk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3phrbiuar.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pbozzhrq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wuaignrt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qliapbbv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nauauoxj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zdyztfvs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3piikszrq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3krrysgxu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mhvffcbt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3anqvxjhe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qjbzmira.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3msloxfvs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jfmhayuk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xmtousny.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zzwaljlr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gjznviqg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3atrzrkan.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bvwcikgt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yvsqmohe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yixwnavt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bmnxvnjr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3utxwmnql.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gwytnrkj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hkdjedvi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ijiiltmt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xkwquuoy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kvwegjry.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bxhnbiah.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zkaqgqbp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zkyplvgj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3obvvsopa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3mnssethk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fqmpxtlz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fnfpafdl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3muuflhrp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3otnkfipq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wjlnxcsu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thnfsivf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xtxpidzp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kiirmjht.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rbkzhkzi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ytsdeoia.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3looxmffq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lykgtyax.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lanwsfvu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zyvumfky.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qxrizisw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jjnykdvx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zbguvcxi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3brxyvppy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3vwfebgku.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rtmcfrws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjbajwyo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nrnrgcfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffivpnfb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mqqpbcil.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gocmmclv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pudyazlw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kufydnro.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wewkunsp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xgzylvdf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fbhnyhuj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3laxrcwvm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3smxnzpfz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3clwemgzo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ccpdegji.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ylcrgzzd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wpagqwzk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bjaqvfbm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rgcxwdtv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3guzlkcgf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oupnlcoq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wpyaqklk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sbehrewj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gjedbgsr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3djcjuuem.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3oezjhvna.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3htoliapi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sgpuzish.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yxwhmlxe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hvwbnqhr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rcymkpex.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pzioqexz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aisfbmus.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zsrjgrxo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3prjlkhmd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ojyysuhu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwmsvmkh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ppgtsvtt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jxumjlff.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3saixpnwc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3khprcydg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xjbhsxgg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ctrtpwcn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3odjfiebj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ezrlrqdm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3brjqrudi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xrqobuis.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lpxqkbed.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qhyfwcrk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vhhhdifh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3alygyajb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hbotvuuw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wyquyewy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lvnbrwzj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xhnexaqf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qcbqrqsj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ntgbmyam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyllvquh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3shgneijx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ybgaxapw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkkneref.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rrwvfitt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hcbhizxu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zaypulwu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3aajvjwep.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3fworiscl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3pnrfmnuj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3jxjrfiaj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3oqutgsxu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vvkidnrd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yspishrf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qmszcwjm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3aepoemxv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3axhdpmpd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zfwbjkyd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3auhpzybc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3gxaiatxi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3titmmtaa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tlhfuutx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fbstblwu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bxlwdjnu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oygqmybs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3niqscwjc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rauufsew.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffiahybd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vedqpfkp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eodpgjrq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bnobvjra.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mlqccppj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txlamttk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmrumvxg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fprkoyhy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jwbonkae.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xvdgumzh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zbltupdo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3niprxscv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjhftybe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bekgifub.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3abtvmylj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kfbtrjuo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lnuzmdoe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxxgzzah.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3sammglhs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fglmjkau.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvawosla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jextsedd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3izkxcjoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxgsoutk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rohrhxjv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nqzhsljt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pibugkjv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rxrxhcqc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bztwczga.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yifkwatx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rrcjswsp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3nfyyvrrq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tkcfoutv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cxilljeh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xjbuxakd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvzudwo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjbertw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3yugmbnsv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3azrwthav.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jnwcewsf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3fibrhckl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tpitqfoo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vklwcxjx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3oqkroqyc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3stbhujoi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dhktilrm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ppaqeqhf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qcnrqfpk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rdkizkck.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vpfddodf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yilhjsgr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kxcbycha.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3svucptfd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ymczfumn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gnnbzqqd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3etirifss.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bubraafs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lbaeukzp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvuwbyd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3udnjkfhj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lbvfqqqf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjwqfzeu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3enkbddug.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3spkofxlc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdconwbq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hhgrukve.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hqmnplcj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qxhlsygv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hmzedjcr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fchyyfui.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3osjoevhd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xomwdozv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fwvkdimb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3coepnatv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gbpmmtxi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3nuxzedte.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3luijtgsl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3csusbkdp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pquqejgc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mnktjgqn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3bemacyoo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wjibehjv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xkuqckja.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3oimmemja.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyroqvq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jxcixbxz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjneyido.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kvkjskcj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xdccssqb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xneotyal.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gawhrtyp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zpypgusv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rpileawb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkfnyik.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zyjtiedq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3josyrivw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mbromtrs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zquekfch.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qfgpwwqd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbessnhe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzanvht.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhorubn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ukoumost.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jtcreliq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xluyjefd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zhchkmob.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ivypbkxg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uaytonel.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zwkjwcqr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3insjotli.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrusbvzx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3iytojkxa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxinsls.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3akrfflzg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ebptmxca.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3imjpjdol.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uzrobqta.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oeslnkpy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3huzqumgw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxqsit.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pignsxib.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kxreyntb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3leloamqn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mzidyjrc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdjmzcqv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xztovbvx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pzbxhtgk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zqliyfuu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3llyexftu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3uldcmlhb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kzmfejex.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3gkqruhak.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dasdahmw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3trqmrzxn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvugkvvb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yczgtzrf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ysxmnpqk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dgzvqdxp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3satkleze.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wqxetbsb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kntotzsu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jshlasoc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zrlaoyei.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3exmitufs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ndrckxlo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mtmxrkpk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ictgkizl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yzrdkoqn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3bzagxuqy.html


<!-- 参考信息 -->