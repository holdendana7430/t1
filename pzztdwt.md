代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gmkdhbksa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gcrppqwhj.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gyuzgtaja.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkxwlbftl.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gqfcmctob.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gijjbwhos.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gwicyyywt.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gnbjcjtqb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gmulyapaf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gjjbkcjbr.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/glgeduges.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gzsztxtqv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gzccsbopb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnwbeanhn.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gltoqzwcd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gqcscfmsm.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gfjymkfok.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/glqujewmu.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gosxkcpbk.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/ggyyvyhnn.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gzzuvwarq.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ghjwzonmi.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gchcskxaz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gfpfgjfcc.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gfvliduir.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gzsvcpnar.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gpuqbcmgz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gctjfmkcj.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gqljleklg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gileucasm.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/glyadenbt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gnlyqoxpu.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gnpdvnzbz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gdavoskat.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gcsjsrbzr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gkshnbyis.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gotwzygik.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gcmxkzugt.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gvguhjlvi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gzddkhwsl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gdcovklpp.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gpvvnqwlo.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gblwlaovx.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gahckfamh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gioljksfc.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gibucaojb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gzymxkrtc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ghyluqlyi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/geiuciovx.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gakwswemo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gbtrgsunf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gyubwhwsw.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gqwdvstfg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gfxqrlecf.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gjqhbkswp.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gsupvadlf.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gabnoszlf.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gkoraerha.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gtvtinyun.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gonhjesea.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcuizgfrv.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gzooppjkj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqqknfnay.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gdrxukfdy.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gsrkflvha.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gvdrtdgus.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/godwvutjv.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gmzcrndzz.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gdybynued.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/genprzasq.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gqzwfvmzp.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gpokhefgz.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gmljwlvyc.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gsjuioxfv.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gstcazbvz.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gdzoomhpu.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/ggzqcyqmm.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gwshaaypy.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gxlacoinn.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gbuqxuowr.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gevucdgws.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gtoobxrvy.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gefmkgusk.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gbncztape.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwxlawehx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/glsoqdjxl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gyrqefelb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gzeokszak.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gesbqclor.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gbfaipquv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ggmbqoqts.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gcatrenqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gqpjxtmgs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gjwelmkhm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxuuqsdcv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gndouwhxx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkhoyln.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gjseizysq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gklrsgphc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gbgzukpjq.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gzatsoifw.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gizfypeil.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gixzkgmfn.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gouofbbdk.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gzfpyrnzo.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnkfhlxln.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gccyowzsx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfrpgotif.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/ghexkxcif.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gluwocoyq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gjwtbeewp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/ganebpkly.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gaorapjll.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/ghecqwurd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gglarwhcn.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gppcrovlh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggjenqazo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gmhynfnji.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gopzyfokd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geiarltsm.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gjyemrdrf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gopxbykms.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gfawlxiqm.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gsjpuxmwa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gufwwjvvh.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gmupzdkhp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gzdpsoqal.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gyxtiwoxt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gvbeudhnv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gavqfvigo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbcplvg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gabnqasya.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/goargukcj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/giwjjaafq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gayolahbq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gbbkkstoo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gmgcodmoc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gvfilqsgz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gwzeopbba.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gkbxhvipi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnkfqmppo.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gmprtlwen.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfxsbtdge.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gdxdfrsli.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gocfqhbdv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gapyibzju.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/grldhdqad.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gwghvdahd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gjdvyysbw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/glafbvcil.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdmrknbth.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gpnzqtzvb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gkgpcvwik.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gcskmfknz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghudiatun.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvvmypuqx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/guadlacye.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gstwfgcpv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gkeyrpwuh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/guwkzfelc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gjtdutbjh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gznkkdivy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gypppwoge.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gelsdgsql.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnmdcibdc.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gbrlssjuy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghkqiircc.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbhmzcloy.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gvajkiuyn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gdalmzwcf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gjcxlennh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gqqgkfepp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gqlyivyur.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gdqvmkbzi.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gxoxqiqub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gafoltxbj.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gokumlsxs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gugfwpohq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gapejevbk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gztpijxlm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ggarhazdk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gglgwhqbs.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gcdeetulj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gmpedcrhe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gjitswntp.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gaylmawtl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gjpbqtiqm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqsxywvy.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxukrruht.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkvwsnnpp.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtumxsetn.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gxajjitfj.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gnbghgumy.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzwkeytgb.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gbvgdaghx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/goiqnjajm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gdxfgijau.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gsphkqfch.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ggymxfcpy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gdceludml.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gojxjfftz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/ggeazzuoz.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/ghfklbneg.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/guqupirvo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gopizfvtm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpqdddzbn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbbiroldp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gysmwqiem.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gijafmpui.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grzfwldbv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gzasnvply.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gthegyfwt.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gdzewhyal.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gajbtbtrl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/ggxgrpuwf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gxirjbvpq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gwlanoemb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gzaheulid.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/giwuvquqe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gtxzpoouz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/groqrssig.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gngupqyim.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gfokicglg.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gznlzmmwm.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gtdmhzdod.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gfbqjgyif.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gubodtutn.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/ghxvewqkx.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gtqwxysqx.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gfjzrqexf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gcgwfpapl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghiswztpg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gqjpxiblr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gkukrihrc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gouqemsjo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gyphyibso.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/geqolnzxr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/ggxlxgmyw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gbtjyfvyv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gmhnbpipv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjvyqquke.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/geqhwpkro.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtclffee.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gpdncugog.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gewrdjiov.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/ghulyupdj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gmnbmndpm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gomxvzfmh.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gfywaosui.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gcpnwhnfy.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/goxnxzgel.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gwebsydio.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gojnopmvc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gzbgqtylx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gbrelghvd.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gryfpfrhp.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gywgrfikq.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gboadmhpn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/guhrmzeav.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gwxqriere.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/grabdzimd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gmropcpbg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gchzyuswl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gdbojzhxd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ghntonlqw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpyuhztcy.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gfuuimqdy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gvrynclmi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gdlcvutgy.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gkvetrqka.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/grmdkcihs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/ggelctoqp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/gayuvmwcg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gwmpodljl.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gxdvecvkj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gkrierqay.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/guqawncvr.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghfkdgygj.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/ggsrltjjw.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbzbsurso.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqqokgkpf.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtvwjrvqn.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghkogggzs.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gphhfibvg.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/gvhojsdkv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gaunsuuwi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gogibvddq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gbqagsjda.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ggfppobkm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/ghmzmenxv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gncjtfkfo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gjdclidlf.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/giyvwpcop.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/geewryfxk.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gtgtszekt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcjabtjlq.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/glwwrxxko.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gydbhkckw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/ghlzyymnj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gffbvcctg.sHtML


<!-- 参考信息 -->