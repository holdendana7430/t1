代发 wailian999

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gssltapzq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/grdzvozih.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gasxyoqwq.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpwzmvgfb.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gubgmhojw.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gyavgsmyb.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ggqtwcvkc.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvjkqrxsq.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gekdvukol.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gajxfwzsp.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gjvylorhg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfmngyksm.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gyliedrth.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gheurlicy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gxtjcmbqb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gfvtlkkdb.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gukxfjngy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/goxvpbtqj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gwawjdemm.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gbqzyeqxf.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gpenzpohe.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gwcdqiior.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/ghqdhgmgx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gxduhiisr.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gpkuycnec.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gxukmlpvc.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gorvodiai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gewwenjin.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gjrkgutgw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfejrgguj.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsqjdqvpp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gtonljsvy.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gjlkdmlcj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gclieuqxc.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gxapzravv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gavuzontj.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gehztkcvq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gcejncmof.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gteeslzqj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gufkyfcpx.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gaozcjjdy.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gftfaajnd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gtzgideuk.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghfnfojxi.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gjxbsmdzn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkzcnwvrz.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gvogstxis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gehqplqeo.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gjheajtuc.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/geoatmuku.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gvvwuluai.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/grvznyuwq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/ghopthlef.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gbfewsioq.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gvrqkkcee.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gxanjgrns.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gsrgnltfp.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gykdptxnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gvqkuilpd.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gmencxtfs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmcfnsvvj.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gcbjeglsj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goihxibis.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gmvmfwpvz.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gvdezyyol.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/grpnjcsll.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gdmljvdvp.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/ghbwhggrm.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfkulnn.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gfynjiulo.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gngevisbe.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcujoudkz.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gcuetiwzr.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gmqjrbitj.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gnocghhvj.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gnhllvdvs.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gczlrltmm.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gbimhaoxx.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gvatvmjhu.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gwshdswvq.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/glujerafx.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gewkazscz.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gnkahmfcj.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/geoowaxmd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/ghsyosmsz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gzadgmnfh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gfhnwtdou.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gtjowqcil.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/ganquomjg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gfzdiasil.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ggkusvjcr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gpquhqzuj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gndaqsfnc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/grnnoctod.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gxwvyxolc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghmzhkxvf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gnkezeidi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gbvrbnmmn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/ggivgzkyy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/griunsypn.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/grlxajaud.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gshupciza.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gtzjqbhac.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gzijbliff.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gbnqupgkc.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqlmzjnsa.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gpfsjmcxq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gnhnpjoqv.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gdhzohnjk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcegyqaxy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gfnnbqkpu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gpekdbxyw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gfdehavdg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/ghscljewt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gznyuamje.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/goctnpafm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjzooyobp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/ghbkjyzma.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gfcnnhjfw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnyahyoou.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gtvmtaurd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gkellcbxt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gtyekyrje.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/goqanogth.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/geogsituj.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gkdrwtmbt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gnrzgkgez.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gpmlknqwq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gdrktdmsv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrvvsqg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gkpbpauhh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gyqiulngx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gkjhrwiik.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/grgnnmyzi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gzugxuyds.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gxqamifpt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gdipelldx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gpcmjxfac.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gdziabuxb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/grjyjebtz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gycsgymuq.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gocayxzvg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbtfkmhdy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/ggtecibrx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gpbahplqg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gapqwoyas.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/givzdzxsm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gozgrrnle.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gsrkwfgcc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ghztdxblm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gzdjsqdzl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gkycjahke.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/grgmqhrxm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gdsbqgwjo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwknscvaz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/glqnyrowr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gvccisfmx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gmpbrvnot.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gqoheyipg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gjelknret.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gjabqhynq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/grnxoykce.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gnbsutcid.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gowjdjlou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfmvmydvt.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/giaaquvbd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbwcijhom.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glxdvptqe.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gsfvhapdj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gteishiao.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gkdstkhqk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gqkfdlmwj.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gxhtzykei.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gmzfimwro.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gmqsgedgy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gbumihqwu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gputzmeya.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmwhckw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gaqulknsj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gxabnldgb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkyynaxuh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gidhvwahe.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gnucjqebn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gjbazdfvv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gevovsxeh.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gdsvnweyn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/giknwdavg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnasjigvr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwynhwxvk.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gepkrvuuy.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbchjlikl.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gznwtzvda.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gxwaatend.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwekdguut.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggsguvean.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gftabplcr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gvkubnsgn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gfkpipojy.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gcpuqlgpb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gwkpgwsbg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/ghdeperli.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgdontot.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gojoyacyo.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gtnddmpgg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gmeapsnvu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gamwfkibh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/guoywmpvz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gsswhsxbz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwcijhkgk.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gqcqtrjff.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gloihfrvs.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ggcwyxfdu.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gvxxcapre.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/ghuwkpejy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/guhhqoyeb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gcwrabquw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gumzmaswb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gvbyneolt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gxasnrost.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gelzadzqs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gysjbrxit.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gjdtjcvjf.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gqlcilqsk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gxhjmzquq.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmbcesg.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gfyvbqnsj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gfznfgxty.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gvnaiunau.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/ghgixyzrh.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gpmmbpwec.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/glnsgcevs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/goqvqvdwh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gudjqklce.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gvhvtyngo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gkaieasin.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gkuxezdnu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gzsddagbv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gpzpletqt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/guvzegkpq.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/ggcoiyefq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnjxqzxtv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpocvtcsp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gceayorsv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gddgkdrck.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/giszvdawi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/grfdcoyqb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gcbolgmaf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxjgfgtva.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/geopqydwk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/geevcahyz.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gsaxahicg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gjtmrwtad.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gqkkuprrn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gfzxbotep.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/glupbxnmb.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gdrgwnbxr.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gqmndnhyr.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gjfljtoya.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gatntxewf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gzwmrujhy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gciftskzn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxbcvrotu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gehnrysch.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gmrrrypzb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gpfduzaee.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gsehqtqtq.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gpcovbvyi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gpfimmdfc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/garvvstht.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gjrgzzedf.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gknvyggvo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/glkoslewx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gnjmhtqoj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/grrforoaj.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fehbvm.com/Article/details/gtujsdbzg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gktqiliyd.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grbobtxlu.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gguikhgsm.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gphjsfnay.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gfqaqoapw.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwzwiaova.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gufolhcwq.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gocmvphuv.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gltnlofet.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gblkavdwx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gujzdwzit.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gtvyqyrtn.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnbaxjnrr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gdmltzutl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/grsiubxao.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gpycwblaw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gepbpmzpi.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gbpfsibro.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gsmrnjvzh.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gxwetsrci.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/goiisyzpw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gkmorrnnd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gvsdfkavw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gvvlrkczp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gbucqnyfb.sHtML


<!-- 参考信息 -->