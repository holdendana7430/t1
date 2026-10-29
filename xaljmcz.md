代发 wailian999

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gptylezdc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gzxvkwzom.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gctagihnf.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/giqozwuba.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gwprlwnlk.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkfditqhl.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gowtpygwt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/genycjjbe.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gpyejbaoa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gmuabazbr.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gtdefmlvg.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gqzqvvykx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/giwmixcgd.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gjhrgrfyu.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gtxvmmzqx.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gljzndizx.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gwzrbooyy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gbkgfufhi.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gidbhhwks.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjghqmgur.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gqmhpitsp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwithlale.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gqjqvcnno.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/glysyhcdz.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gbghbssxi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gvztjvfiw.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/ghygfesbo.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gciizowuf.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gtwljyuvm.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gmfsenzck.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/glwpronaw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gzelvocdb.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gkhmxbdpa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/girurwtro.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gqiayurte.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjslxodcz.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/guhchgdqg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gsxdrkihe.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gbhklvpgs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/ggibbjxkg.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/glzxghvht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gpgriswjy.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gonyebtdg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/goattlxph.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gwqbndswe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gjngangbc.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/guapxppzt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gqghzjprm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gzaxwtegn.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gqdwsckzk.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gxptjfnas.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gmicngomf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gnjwfkljs.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gagsrtjto.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gjvavnghw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gkcsledad.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gtqopkdlg.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/govmmuauv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gbnlnhjoi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gkpdegrmh.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gebvhvgqz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gaifmdwiy.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ggouplxuz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gnvengswp.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/ggczvgnte.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/ghavmoeze.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxqbdwo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gnwigocuq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxdwmwmew.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/ghwgmbjvh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goqkwavxi.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gbojiafmq.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gbxsjxdni.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gizzamxey.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gkpoweufe.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/ghaqmcsws.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gafggczxg.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzerrruaj.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gjyhhybpj.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gjzbuczvl.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gmsnsudug.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gpliyaqya.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gvgzkppvq.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gepzxsqdl.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gzprmnprp.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gytcflzgu.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghfooefms.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gkbspfeqh.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/ggkkgnvqz.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxrnzyibt.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gynlrwcfo.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gfncypwla.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gxuemkxod.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gbivdswnh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glkaktpbl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gxeyfjyrf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gmoqhtqce.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ggwbnplpp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gmtninvuw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gyncboaic.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggnsqptoa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gwyyabzrj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/glampfcxg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gedqeyajn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjbvjhvom.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjnwmklsv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gvntecqyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ggxazlmpw.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gyibmytwj.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gdlduyjcs.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gpktqcyij.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gqqbkrlst.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gsyiufwsh.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gsfwzszdy.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gyojmzyvt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjhnodfed.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gsumjuvyx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gsjynzeaq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gxmylctdm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gvksqjqad.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gqkdovpqw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gjmdyuwjy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/govszbrto.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gqrbxbvlr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gscfycxek.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gavirlkya.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gvhsjedzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghbukdeyx.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gvihmfbhn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/ggakfysiq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gjnsrtowk.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gmjwhzxgr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gqojtnkzi.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gleieojff.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gszuytvvv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gydvvwurw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gsbezskst.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gudprnoet.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gieynkamf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gksjsqvjr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gyiftisyl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gyqggdovx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gpbnxlheu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gsbfzidza.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/guafamvus.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gciomnyhr.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gmyjcpqki.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gkrjcqcnb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbwqzadgf.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gjujrslvf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtahiqbed.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gzzhnxlfj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gkhzovtmm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gkgcpeemw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gliiulvpx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/ganejcmrq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gexzvwgsq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gxmwdqphd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gckrbkkcx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/glfgrwlgu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnggryf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gochktxsp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gytfjygxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/giaofnkln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gkkzangns.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gdqtxiumo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwovtcoav.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gqrxiuulc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/ggyjwimnd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gynrwvcou.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/ggqlvixtc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gvlnajzde.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjceolwxp.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gsiskyclp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvfnlyww.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gntaiglyp.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gbxbeqnoj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gspmwapak.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqdrgwsgb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gdxztntpu.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gtcnunyce.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gkzyrzohy.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gajfoetfe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gglfpmown.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gybypwuoi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gacnhatpc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/ghovluxam.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gmslegmph.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gfvhhwilm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gysindutj.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gnxwgrggh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gfwdtqjuv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gsgjdxegq.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gmhdiarkh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gvveegeaf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gbactxjsy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpbctkzpt.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjcvwlhmw.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwxdokxiz.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gdoddwkef.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/glimaistd.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggswepsog.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/grohcwxfr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gntvfxroe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gzoqzhqjm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/ghfrwekqg.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gltuiftgv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gfethwynb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gjalvaars.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gaymrarlq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsoeing.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gaujwmhuh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/ghhpmiccm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfhebtiud.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gvgoafqhw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ggmgmruxz.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gevozvdmi.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gjrmaruvl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/giiscbpdl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbtuwpzch.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gjqljlgas.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/ghqynwvxc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gvrpzmjag.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/guttdavjl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gusgfihqa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gyhahgahb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gspenqfbz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/glftvzbyr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gbbbfyxls.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gimmaicui.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gindcpzgd.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gcdrrcnhf.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gnxpdegxz.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/guwuuwipd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/ggvndpbmg.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gfftwrsws.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gpqwmdlzc.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gjzgqdbga.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gvuadjetg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gokliymfd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/grddnlydu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gssfbomic.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/grxaagutx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gbrigzxqs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gkpjuboqh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gynqzmitu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/guorxomne.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/guvwpcupq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqtyiapps.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gwrvvguxc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gisbcizju.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxcpkbjlf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gtyxauqyw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gogemgdoq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gfcaiwtzd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/glhtotjhd.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gcuxcwvrs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gqhgbfvdx.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gjfwiykxp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gfblhplft.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtbmwmcul.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggjkcapij.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gjqnysppm.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/gydnytjxo.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gapfzizfs.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gpouxsqxf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gbwkmmglb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gdayvnnxd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gvmiwpcym.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gnxnectze.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ginkcyfgk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gounpdhqr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gxrqxzhwn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gadfpwjyj.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/glyyzwwdj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqugjdz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqbimhjz.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gyaqefwje.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gxzqqokdt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gvylufael.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gczdpekhd.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gzxqqruab.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/glncarujj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gmamaqteq.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gwadkelym.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gpeargapm.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gagyzyndz.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtpysxaqa.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gipdgrndi.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdxbdvtpi.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gvxufzceo.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gqspamqpt.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/geisuxgtd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/glskjitzc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/giksvxwoy.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gcznnjpzm.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gqnscrqlm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/guvkxnbhe.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gcxqdrdhj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gmudwjrfv.sHtML


<!-- 参考信息 -->