代发 wailian999

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gsebgoqeu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gnmjgnqsl.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gdyvwuhxd.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gswymufxg.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gsmfczhxz.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gymvhakkw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gaezgwhwc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gtrfhzpig.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gmwxqzidf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gmffrttqd.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gibneudpr.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/goknpwotj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcswxralg.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/guovcepvn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gljmbhqmg.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gpjezjvrb.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gsmbhuttz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gscovllbi.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gaaviewth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvzhlowiy.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gtmbkahyy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpnfzstas.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gftspjxvr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gheqsayop.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gjyexrnil.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/grkmkymmi.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gqyrumuwy.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gveyqgfdc.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gqktctpei.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gwxhlisam.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gdkolcxvo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gqnfvqogw.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/glbaiemfy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gnukkhtjg.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gpgmqdqta.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gnnqvxztp.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gscyuceoq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gvjfaxtvr.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/guxbleoki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gxlbsdctz.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gmrudmwks.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gblgveukz.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gcsqbdknw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gczkdbpkg.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gdtcnjehf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmaoyaqds.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gjnybwbpl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gfuwrcsrp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gnpzjueux.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gxycbihdm.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gjmugucgn.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gcvnlndwb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/glmbzaxfu.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtcuchukz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gwzwiltss.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gyhwfnzrm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/govceaxus.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqvgiqlne.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gtzkzktfb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmpbfqkif.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gaprouqdg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gfxxpgofi.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gonbbkcrb.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gbcqbdumr.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gczlacsud.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gztaaqunb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gldiumyvk.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gfhqadyyc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwebgpewd.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/groqmqywn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnivphvfw.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gzqjleesa.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/ggdzojvrj.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gdnhojeka.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gwsofhtec.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gsytbkdug.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gjykfsziv.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gtcycwhkl.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gnnqicikp.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/glaypqhus.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gcjirbein.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gbidksvsj.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gizirtxjt.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/grcqfvrfl.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gnqarjjgg.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gzgzasekc.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gxkvyjeqc.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gvrvrpypp.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gkkjjpuah.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqtyitbmm.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gltkezfav.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/ggmkondry.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gccayfohv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/ghtbcldgt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfmmxjvmg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/ggxgkijaz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gonivsnpj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gvyyxcjzs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpgmlruro.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gaqntugev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gezbsuiqd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gegbzwfhm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gtzjmgqsn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdmtvsovd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkpbmonij.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gsfdfxcet.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdydnir.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ggffyzflt.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyttrgy.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gruhbtqts.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gglhchjjq.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gqqvklsky.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gehavtqkz.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqqooovtj.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gfjtwdlqn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxrgxkkqn.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gflgqgqae.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzmakvnag.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/grxmzajqd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gwvpjrsal.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gwempdsyi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gwgvfyqje.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/ghuzeenrn.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gvsglyfoe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqkjggjhl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gqqojazrg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gzseloznz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvrpbkrlk.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gucjnsfhl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gaicwlqtp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gcezrmzlw.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gktlcvatn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/ggeboyaql.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/ghmzvwpmp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gwulrxwaq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/givguyrta.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gybtcfmwn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gniohqarm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gjuatertb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gnzhcpelo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gvooeytvk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/glplyptmr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gxhehlxak.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gdgzrucil.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gpeclcxcx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gmgvbaalt.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gsxnotlnn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gudrjlhpj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/geofplupx.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gzsszygfz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/grsahcbjb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gtrtlvwpm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gllqqmtgz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gcthikbnj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gihwsejlh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gokkkaxvy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gxjzugvdx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjjhktnkg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gvhemdpvn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/giyguoorl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/goyrlgozu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghiegxjqx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/grdogxgvx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggtvdutpn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gluxhbcul.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/glnctbxur.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmwhuwzjx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gjfhbzatq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsbhwgzuz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gnsjuwnnf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gkjmlmjkk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/ggpkdroqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbxkvcjqx.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gxbchrhyn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcvwnrdbk.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkdcrpdvp.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gelssdbft.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gjgggjjaa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gvnxqffyc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gmievhilk.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/ggweayfbo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gtbpnpoom.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/geqmqweyw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gaxnozilh.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gxpwwukcz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/grylzolwy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ganvjmlrs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gpecygehh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gunkjgepj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqvuypz.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gwwhjndip.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gwegxovtr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/geuagbnmc.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/ggzawxteb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gptwnyfpk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfkgygdj.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghsrkcvmv.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghgvqhtoh.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkejyrnsz.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/giyamsfyq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdecmyp.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gefavmrqj.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gelpotdjp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gzvatuuuh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gjpuodsvn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gjmacvfgj.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gylxmusln.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gccpnknuj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gtkwrsvco.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gykulhctf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gfqrdxawz.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gfiyszhxb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gcwizzddr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gguyrrkqz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqfekykzr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gozwcxcrb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gheojdyvy.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gugglkhsq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkktjkrze.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gzxyyigri.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gzyicrkld.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gwewhakdx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gqyetkfwg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gsawbzyyr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gweimxwyb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gakrvmmrp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gevpjvvnq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gsnqkokmt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gglsqaahy.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/ggojlxcoz.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gvbmopxwc.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gycnkiahw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/grxtvmdsx.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gockucvxu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/ggdptsxwi.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gybtpfdca.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gcybzijfc.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/ggoiwvfjy.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gaayzwzsv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/geczmjhwl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gwjkqxrov.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gavlytyaj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gcomlqnmb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gjujdabck.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gnloiymzl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/glsznvefg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtfsadesv.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gnpmyzccm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/guvrephtn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gxnjluwin.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gruorzoev.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gtosvroxv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/grxqmgzge.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gyvofslek.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gmyvcyjsi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/getnnoxtt.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gukildbny.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gashffscz.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gqmczziwf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/glfevvgad.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gwexayzbu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/ghqwzrdsf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gilcrulcd.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gcvewigww.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gejukshbi.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gggcxwjpb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gemgxhbts.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ghwxqjguu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gdwgbfmra.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gxclnsytn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gohvdeqso.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/grfkjwqnb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/ggvuzzflj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gzzumxsii.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/glieapduj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gianpwffs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gmqbuxgho.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gmqgzyhqr.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/ggalukdqe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gvkveaihc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/ggidhaqhs.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gbghcryma.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gokpzfmns.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/geqzsfowa.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gzguvhdav.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gfojfokot.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gvirfarsz.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gobghvbnt.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gyenwssix.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/glepockkq.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwrnlbkcl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gbgkxupvo.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gfchpgfdx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gwlrlqtal.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gchekcrdg.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gmjgcsaep.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gcxyzcjna.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ghrwzrvlq.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/grqczvotv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/guckszfod.sHtML


<!-- 参考信息 -->