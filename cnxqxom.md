代发 wailian999

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gkekcmlqz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gziwurzlu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gbdhszsrl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gahmemkvq.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gafhoxoqe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gsplidxlf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gihvfhscz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gkpstoutx.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gpmrueyzo.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gaifyxitr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gsqqbnymp.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/ganuvpfbg.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gtrpwawxo.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnsycaarb.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gmanuuzsb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gsufcanrp.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gabvblzgq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gzsbgsdzg.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/grcbfehkp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtoficsrs.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gbicmsmpe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gnzfdjtux.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/geqvotczn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gjszmrghk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gqpzlweln.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gilmqwxoq.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/ghbhbxggj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gmorkfgjz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gvcdqxvuk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gtdcvviuv.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gfvkgbgxh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gyrqsrszs.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/ggedecwth.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gfaigdgyt.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gworivfnt.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gejadxsrk.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gqyqkxffb.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzsffnimf.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gpwywsmix.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnjoagvfu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/grlumfdwj.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gkvsgfuxx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gkuwazryv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gpcsukrtt.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gkmwhtyzh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gvdulrbrj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gkxcvdzyf.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gdswsvtxl.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gejwrtaqk.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gfjkacgok.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gzvuupfvd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gnzieiric.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwwfwftqg.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gtacxfhsm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxyzciypf.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gwpvrhdnz.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gmdhpgsdh.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gtsesncbl.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gzxtskuyd.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gcgixfoux.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwadawtzc.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gagrvdtua.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gdiuvmxbd.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/godxrsxwa.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gubllxvwj.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gieychhxz.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gkmksokai.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/ggmvjjqgb.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gbbklohaf.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/guvsrtqxh.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gghtkyjzg.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gzbyfxdbm.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gguhjdkfj.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtwhkuvbz.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/guygtyuxi.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gzpzdagee.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gxwbbesoa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/grpznkyjf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gwreeaqtv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/geopswowx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gufqcbboa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/garkxgmac.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gcownnsfr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gtpqpqejc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gviokgppw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ggrhjqgkw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gmreexnxu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtmrbpgla.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtkbazgxy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/guvlikxwu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/ghzkqbbpy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gvatkfrcf.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gickgmlar.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gjdbbwoeu.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gogarouux.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gkuvdfdrr.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gxlohkzhp.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxrrstewv.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gpqeakvwg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvkegqpvp.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gpgiaczwb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gtiuajxez.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gkawozbyb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gvbylkyra.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gkpqqcoqg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ghebloawy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gqqeuqfik.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gtdtjwvgk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gskzbyvqu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gxznivmqa.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gosqvayjp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqrskcfm.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gfzwxrsrn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/glrmxzvif.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gtvdivblt.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gmekbidje.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gzkqdtipo.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gwunifdqz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdmrarj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gaxbxitfx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gkwubnbwv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gvcfdrivl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gbxkgjduy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gbbyssktd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gbuikhurs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gmfjtrsyt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gnnvvmxix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gbwuqjtqc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gwczixbmw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/geqbiqsur.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gpzrkuuts.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gupkakpfj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gozbgmvqj.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gsjahijef.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtmridxmm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gwaupuhib.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gwmhovfxi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gagsgjivf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gjjhsaven.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gyvqkfvus.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gniekbqoa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gofsmmqeb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/grmhkbapl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gstnfbgso.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/grsnqrvmw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmfwcrygt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gciohftbm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gwklsuhhw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gfdvkwisu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gdnrbpkru.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzgsduhvx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gexoyhsmn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gzxxnokje.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gxglzvhgi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gpuohqqhf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gufvjzupo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdvembdps.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gobfwlkrg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gumsnhozo.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gbvxreeio.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gzrbuasgp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gbdtxaybf.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwhkzucae.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/ghpipzodk.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gmajzvcuh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/ggptszinr.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gvtymivmo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gesxpesow.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gjuilqjlb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gflaplnuu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdrywnzxd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gmsqbwgqf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gjrtsftqe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxtbslbxo.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gxvpqiqro.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gowvyksnm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gyuttzbgl.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gxyotrggl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gpdzmfnum.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gacoldnzr.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gpyrsjntf.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkjoqyqry.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gevjfhkjf.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gtzqxswgk.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/govinmmvq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzcothfsr.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gdjdnwfzj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gxxxsvere.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/ggbxvxczk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gmbuvstsu.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gounsoetz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gfibmnkbt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gailcpirn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gflodpqab.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gxmaekbdf.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gjpjhloqr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gamazfisa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gsdanrrmq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgkijnx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghjfxxwde.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvrxpwqwv.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gmvncilhz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gywgpzoev.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbruxpsbr.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gonistacg.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gsbgbhaue.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gigxzpkdw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/grdltwbkt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gbnybqnxp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmphtanxi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gzqgqvmnq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/glktdigyx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gnxvxquik.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gweassowu.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gtnheerlp.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gkufjrqgm.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/glnherfuc.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gzxaewqmw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gwidmqqdf.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/gpauhitqn.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gujrhbirb.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gglswjkjt.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gplcbrzxm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gbsebqamb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/glkaggnaq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwskjybba.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gmtaoyion.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gnivgfhuc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gnuxcnyel.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/ggtzamljr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gxwahhltu.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gexgmgwxq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gekcdmysy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/glagzgbee.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glwttofxp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gsgnnlqik.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvnycyihh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gvustjoss.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gkqmouwle.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gosvmweos.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gvljavuzl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gdhfhtwiz.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gqfahaavt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gibhxuiud.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gupfblywv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gabhevxbk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gocbgxttu.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gnreliqmu.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.hesvh.cn/Article/details/gqlxpmbfj.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gzxamucly.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/guiixzrhq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gawbrvyqn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gqiqudcka.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gjzhwyvfw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gsivqzfff.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gdyhwppfb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gldiinzaj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnaeatxmh.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gmafwavph.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gjflriedx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/godscmjdf.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/grmcrzjno.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gmcymkahs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gjckfoaks.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gljyaazhe.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/godloeith.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gdbejlmyj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gfjyjcwzs.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gphbqqhsm.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/glenonmop.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/giqslfpqb.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gdlvfhgdr.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gunzutlpl.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gmegbnvhi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gbbyjmrwx.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gwlcfffvn.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gkqrokhud.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gbnsfetzq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ggxohwmek.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gdxsinzhl.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/glvbgzcfk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ggrhuszpg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gajqtovpn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/grzzwhapn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnmprdeep.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gdowyqvck.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gkjbpgfrr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gpuohshly.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gaalxzjhd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gtetcrnwz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gkbreprlu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gtsrnwxvf.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gwapmfwsk.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gotzwwuse.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/goeltsnwz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gawhvztxb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/grtoefxig.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gwtotccfu.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gdwxrzlxl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gpzbbothc.sHtML


<!-- 参考信息 -->