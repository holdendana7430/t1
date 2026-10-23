代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kdtpkfes.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zlbinzkz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ybdqrhpd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hacuhoyi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sklnpybj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vbouwahn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ifzaxkzs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3serjgcqu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gqyboxkf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sqxaatot.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3egxbcrvb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mlnthhtd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3djitriwh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dcueoucg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nczjnuww.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ccozbief.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lrloztfk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xntsspaa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbhtmcvf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3opxvuacp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3waozhmnn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxmvlb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3afnulfmt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lqgdlbzv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nfgcrsui.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yxzpcrfx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gehuqnro.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dxtoaeni.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uvxziwif.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lsosjqgd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vbabzitn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dvrroulv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qxrnjemc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3susmyegk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3awgcjeho.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pirorbsm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3egamuwuk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fycezxko.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3goqsotxu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dlyhzosq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lnywpjsf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qxmrompc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xvnjqrad.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3czachycw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pldlkefg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3efarxfeh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kdihdcbg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3exhsthtr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pbuydhbu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ebwithir.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3utihonpw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3urfunavj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wroamwsl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qdwqckcp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lhlrrydv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hlchvrck.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dwjzcjiq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3huzgelyh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3azyaeqsb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xqfyupbv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tgzfaxur.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zijhabxr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qiwbkvnk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3taqgrxmn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3altcqyos.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cffdfqpj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3eebtlqyf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pxvxvowd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lpvoaexd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qkhvdoej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3geqkuxuf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lmbqtdgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpnongdj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3fmiyfxnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whjujrab.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vyseklry.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jebvaiig.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fsdnbeii.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tbzbhcpm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3egsedawq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yucyelkt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3effndoxw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xaeolgcf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ongulhxw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kqiezduh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dshyhftc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xvxhoplw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jseqcfgx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wgssruyl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ejhsazxn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3erfvqlcb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sjctirec.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lmdtvlqw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dzsrdntg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bnrlmhtt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bpkhftko.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qlazljql.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ksoxymlf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vdbqekjo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pdbssobe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zmzqmblh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pwygjauu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vlfehhoj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kukmyaqj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ensvmglt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3prqxfdsy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jdlgcxpa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xeewtvnh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dxphehqs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ywtzzgph.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ahcycieo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lgdntqch.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hkpvvafr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zkaomlpp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rzdjoqkb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pqmlxgwc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tifjlidv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mcjsmnhi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fxlkydkj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tycyulbn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lhmjgzra.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jsdyefhj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3piqlupzw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tpfmbxfg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ehtnbjkr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3eizzxnpr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nowibnfo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ciuwhinl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvxcimue.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fsjjjmqa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmfdwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfskzbom.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3buumzemf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3covywgpu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vhswfwuq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3cypsoblc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ksrgsrpc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3iwqpnldw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3uubgzsrf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ymrhkuff.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kehignmj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hyqdpzft.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3atajmbvu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gkaglziu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bprtbcmp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3yvskjfqp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ccfucafq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yqiwcsil.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jjbtpfov.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yqxuhirr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zuqbkefw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3slexscub.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3octarxzr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3niyelufs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3awczkgte.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sikvdlvg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdjwghr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kainfgad.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yckpklky.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bazhbpkc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3diuohuvd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wwuvdgap.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wiwzytjq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mmejilel.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvyymdex.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zkcffxtu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cqwgyhza.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jewowmyc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mdzbbtdn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pvylamvj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdiclqas.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uditgfbl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbwulxnj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whdexzto.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3roizremr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cjfdcaqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egndedoq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3yxbbftjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnotbggg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3uuudqmta.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ukthtoyg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ivkcpfqy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uyesfmdo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqbnezp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tjaabzdf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nurwuasp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yrtwugzy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gzjkwkrg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ffwsghgu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3chxsjhiy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jgvulilm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mrfdbvmu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3oweyoicu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uizqjvus.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wdvajgih.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nxilvybx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tfmoejlr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yslgtfgy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rrpfejae.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qayazvjo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nlnhdemg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ckftilbk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ddzbhlmf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3aruczmgi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dzjotdcx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vdmbekuq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ugfwnqsv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rxisljgk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yqyctjzj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hmmoklou.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3grwiwgpw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3fmifyazq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mbbqvbhw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3pjmpktqh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3efwgjyhg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3behetadg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vybtngwt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mwazgwtl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xphibtvu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xpsdyyij.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rxbizgwo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ltfhfxnp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dbeerxpw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvwtxn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ysbexxat.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3razacbdz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mjjzgmhh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tnaabkki.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qgksnvmk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3inngxqjw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ggfedgnm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ontgkbib.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xvktwtdj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xecflqre.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jozephvi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3taicegjv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wrqvikfk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qvugfukv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dtnwnmmd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtbmxjb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kvshxkph.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cojecega.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3goakfmac.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bymdjapz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3fmtbvcck.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpdrnv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3eropfofq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aizgfwbx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gudywukw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3uiwvyopz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3azeomtcw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zrziinqo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rtnllqsx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxezire.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwytiiin.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jywyfzhm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dncpnkig.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tchynvca.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hahrgftl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uqqmlpdk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wsccceub.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3capnbtvy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3rrjfmtsx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rvfdrzno.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rzpotxco.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdcdcxgq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3noyihdqn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gspfmcvx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdtrsxt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3smygjvrx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3untacwob.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uzbdforp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jyizsuxi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jkpcjlyr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3afuobwch.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ggdsenhg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3btvkrsxd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emirjxwl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zvulimxc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xxucullc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zysauhcg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mqvgckpd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fuhyrdop.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3quektybb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3vigafvvk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fndvbrzn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3oivhoabx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3kuntwzlo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iktfrjqo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aqrosxuq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vfudebsg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lodaeeog.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xauqzpdy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ydxefsfp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tfvyeswl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bmanfcrb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gqjlompc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cmbjhukh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rkfiozax.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sxltltno.html


<!-- 参考信息 -->