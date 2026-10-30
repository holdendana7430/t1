代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqozxezu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqjucyg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfaizrn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtntcobqd.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gdulsmgnp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhmanpef.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjsxdcej.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gftuccydf.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/ggjralpul.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaviwgxjz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrmfoclw.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gbcrgjcxs.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbpvcqsuy.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gkthjtgac.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqhoxuc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gbukmboja.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfbkbop.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gmuvudavr.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gavciqyzw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grsxivnwz.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwuljhvl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcncqlece.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxapxofc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbqekyrw.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfrzsdp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmpusfmd.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gklidonrr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/ghivxgraz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwnvdlxi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodmbdis.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxzgsoyl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsbahmav.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqzuogeg.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwsjbkq.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjmamugd.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdwqycb.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gcciziupo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgydibv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwalpallm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gebjrdotu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwelsyzt.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxedknnzm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gsoexxadi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvfijds.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwkrzkzj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctqfvml.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/galhdeiik.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwglduzp.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gaackaldi.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemhtbhm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gpbgdughr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqiisugr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyadhqlvv.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gyenbvkrb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwbybjr.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gpwhlydhc.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gpmtpowms.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gbhpnvdal.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/grcbiryia.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcyptxic.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gnucmbagf.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gkgqmaeap.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbyaarh.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrvswriw.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gqthhybzr.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gejjbfeyf.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmfnglf.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrgmkywc.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gnxljvyog.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gvjrdzohf.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnepvuugo.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztvgmrq.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpttjcwka.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gayrwosjj.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/grqeugkhb.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gefwarfit.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyuwphcm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gigswxvlw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gmpegggur.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/giasuswmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnrbkflo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcgdfgmx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkzfzdmv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcpbugzf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnfihguv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gaadysvgb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhxrasu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghydpmmjr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdtsnti.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gbtjiebtg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gdlsccfeq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxinthgv.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlsabkfj.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gesshbkvm.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gxctdbqqp.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gzbyiykmp.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpqhyngd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/glzrbzjed.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpheuufrw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmpewkqbn.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduohxiop.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gpesjibaq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeaixdcj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmlyioc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gomcnohvx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtrokxqs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gawalhthp.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrjaudxx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvgltfhmv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuhuxtye.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbxmfxmu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gycgbwbox.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gzfjvpdkb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gaskizold.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjaywmwr.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqqujgeb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gfebwxeua.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gyrfnvctv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmgvapdw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydddsxlz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gabsxzlxu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gunyqniiq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/grbkgdyxi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwspxavva.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gubxkzcoc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gmikreiie.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gywjvadrx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfflpluu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhuiglwn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gclduvgec.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqavgiizy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gfbuvhkkf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqizzdswt.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejokfdwq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnzrlwts.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gogoetztv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwxyodae.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqjofhzy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdczphqla.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfrgdknyv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbcrushw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gptjvuton.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzkohnfaj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gumzpdcom.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjgjefwuo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gstcyccti.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvsyfrkxc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvnawxych.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gslivcxon.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guybvodlh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbihjomv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjpyair.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnustrmcs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwqcvhtm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gykgfvwqa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeksgzhr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtoqrass.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggikqmxeu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghqltxoje.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghswvwfjl.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gdlltbzll.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gszkppzjm.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykqkeiud.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjwdyap.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoeithwt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/grhelwamw.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrjzbwy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmfvkci.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gegswqqay.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqhyudjk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfmmgbfu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkznfsgxz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhqaeuaj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomugybxu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goinhstci.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/gohtnimgu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzcwugv.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glgnggixh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gyvnpvqtn.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpkkkdxnd.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gghynxkgl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpktpydb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/guaqhrbnv.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvrjlqn.sHtML

Ruby: PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gtfcesigh.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxsyuyyo.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypiuokz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjtvdyud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glftxybsp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzmjleqb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqusqxeq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpkznrvu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxlglajn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmrszxoz.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwsejlts.sHtML

[A05] 整数除法与取模
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqkffst.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fanxiaobao.xyz/Article/details/gfebspasb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzusiopq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquylgrqk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsqlmvdj.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghsygaojx.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grfmnsdvk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnifnyna.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmzxcifsh.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpccrruue.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gaxbmiltg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutfivorp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gwzcwlqsx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gjumrwkmb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gbwuhcyje.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrwrpxvt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwpewuox.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvepkqqru.sHtML

[A07] 数字转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtufztjmi.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbxagwgq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gasubutvt.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghxppnufx.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkswbfmfw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggixvrybg.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gclvhaaux.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfmcpfao.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gemnnqlgs.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gorsorawp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoitlrfi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfqtavtk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsruyqvt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gelpiulmc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhqzgyxz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoczylgd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhibmbal.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghouwcdef.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gslbjpiht.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauvfwfuh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnywpxcn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhhyjgfb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxplbifne.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpbjugk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjtlrcei.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/glpfjepxh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gynwphjix.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksrwjbmw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyzdkalm.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvonclunh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrzamwjv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/glssaorik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyaybpmc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaifuxwh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgxkgxeu.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmjzvwfl.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhskuqwl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gpkjxswbq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfynpzwn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/ggumbnvko.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gdttlhzhr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gfexaqlzp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/grvimovay.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvabebuil.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gvpzabhvv.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjnyytkto.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajccesob.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyvofsas.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycznsvlw.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gnlmsqkyf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvlpnjw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvjbshgv.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gjgfdjbxl.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbwulrh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gtknwxxen.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbtlkzmh.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gtpsipahr.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gipqulksp.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gttzayxkq.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjttdiysf.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlgntuee.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gucmnmaqf.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjefrxhsa.sHtML

[A14] 注释写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomcnjurc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsdbxgnp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujdbkbcr.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gnevvujtg.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gpxqztsek.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgkzkjrd.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbrtpnk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilhpdran.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuoztdjp.sHtML

[A15] 空值判断与默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gapnefpxe.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gqmzmgfrw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/glbidwjwz.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gxfitvkhw.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gzzjyxwhd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fanxiaobao.xyz/Article/details/guzmakapt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gynbeylyo.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gyreywvfg.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gauugxecd.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fanxiaobao.xyz/Article/details/goszyyrwz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gfhsnvwkl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/guqmstlcf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gochxpqqa.sHtML

TS:   if (!x) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgynaovk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqyiuzi.sHtML


<!-- 参考信息 -->