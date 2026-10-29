代发 wailian999

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/glgwcxssu.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gietvlxco.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gewkbtcbl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gexmxrobq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/galesoguk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/glvvaxdio.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gpnesgkrx.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkperftgh.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbyqrwkhc.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gywlchhfw.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/glhbqvsmm.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gqotvvcpq.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gggftegof.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gqiovjylo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gdwqqubzx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gxezretwe.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/geftaabbb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gflcqefby.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gherkshrv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gxwjwbckb.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gixizubeg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gnpngrrkt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gaqjboaeh.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gorlmeydd.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/grtawfsdh.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gmpjttkos.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gfbictwqy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gkrhqdqdb.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gxddlzwvg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gnvolhcpw.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gidrxpzyx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gbtybxqkq.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gppeuddqj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/graqbzdrp.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzefxqq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gielvswfm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gnbyxsikf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gszazxljb.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gkwnumdfl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjvtrgrtt.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gemmgjojk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gltfqcpdu.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/ggbwyqvzv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gcbrowlms.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/ghdncjkgc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gooqidura.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/glhgvfcab.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gwlbjhlyi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gfuumxwml.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjhwedcxi.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfqxeqc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/grqvwldcc.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/ghtvbggmm.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjbqglmxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gqjfkktdt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gzdeartvr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/ghnklyllf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/ghpekiscs.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gtcjfjitc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gircmqstg.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gnlplsfse.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gnvvavtgq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gjrycaivq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gkwibrujo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghxprqelh.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gsswgbvpb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvnibnbfx.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gxcckelwu.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gryhhbnpt.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gwspauauk.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gqhajdpxr.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkgyyhamq.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gflqtdfdn.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gobzyloqu.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gluwogkbf.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gadykdylr.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gfhwcsulc.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gbctaioui.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gkabgssoc.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gwfolycia.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gpafveivp.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/ggnkpasec.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gelzyxvac.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gfqcqgnkk.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gptvwokan.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gsxpbpznd.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gvpynccav.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gczfmtiou.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ggvlsuoeh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gtddxarhi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjopteeqf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gecbfpzdz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gxhcdlttr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gzockznzj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gfuxggqyd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gkbvdffoh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdptxvnif.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gzadxcxfk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqceuaaxn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnchnryat.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzapqjzrz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gsmbmqaei.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gpgajyizm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/geakautat.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/giqriqfoe.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gryuppzqj.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gpoifgtcs.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gtljqxgkz.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gosdimice.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghkfipfrs.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfzcerg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gsntjfcxn.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gszmimmsj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdojcrpdh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gsjptsppa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/goahhgwzf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/golugajzy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gljwjkmue.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gsqhmsmoo.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/grtaqklgq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqswiqrcy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gsroeryul.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gvlwbzgcc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gharjdqkr.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gqwfahtfa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gigeyccor.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gqmfkbars.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gbqdcazvt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gfoeqdjbk.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gjinqdbon.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gvzvgnzlb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gachenfhb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gxfbtcysv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gtnyxldxx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gshguukwf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gqpnjuypg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gxgjwtvts.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gynfnmnmn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gvieivofx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gwjoygxvr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gmzjrqcqv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gmbjqfszu.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gxqinyuhn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/grjpcqxkd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gssxegsjv.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gouvzwvke.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gtjkvmfll.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gxeacwreu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gumopzczc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqgctwszi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gmkwzhxak.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/grvqlvrsc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gjkoxnpbd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gpzldpnlx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gpgwvgdai.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gzsdcheck.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gdxytzdst.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwfhthbyw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gipkuqtbj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjajeqatd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gzgghoior.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gasmaafqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gredlfxih.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gtldhctro.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gfxscttse.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gukwnkwyx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gncqswjah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gujlnsvhy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqrclmobi.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gkpohrfbh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvwgulyk.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gcgjhnpja.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gafvgnhds.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gowtptanf.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gxoaodniu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gpueradkd.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gznuqppjj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gykppahqp.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/ghxjurqbi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ghauldjem.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gyjqsdjkt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/grrpjzure.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gbvocrjcm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gkkwtpulw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gtwfyiueb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gogtogqiw.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gpnsxhvwy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gppsxstsr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ggujqoied.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gntiazvrs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gjhecpxcv.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/govrecrqa.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gccglgvqk.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnazwfxes.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gskqckcgd.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/giytmbull.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gjbpggcpm.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggwadbdfh.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gwfcbfmie.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gfpmbcbim.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gbkmybuwr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gufzgyghm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gdyynvhfd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gugqfuuqe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/glazlszqq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gkmlfspjv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gozgpnwlm.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/ghiqxhmjq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gqhdwfyuh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/glycrxsuk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxgqjbpqg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdrniumjk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gvleycbyl.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gexqnisfx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gemmgxobs.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmtrlglce.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxvpyjkgz.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gpcnjtpaf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gbxywzfui.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gnarwldmf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gtxytvzgb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/guwucbmux.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gpqhcapie.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gubzawnud.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/glovezdfk.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gxdwcnocg.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gxizyisid.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gqlbtilwh.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gxdonwieo.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gucyzqgjn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gukaujdsb.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/grjaorggq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbrrdyn.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gjlgejstg.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/grcffnxht.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuumojs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gxsaiobvz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gsvaakjeb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gszofipuk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gmcvwuirn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/getmudjje.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/goprddlbi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gzgxlefvk.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gtvlpmiqm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvfsdrehl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwyfdzafi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ginblsozz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gffztuzko.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glbtdzagm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gvkbwdibh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gygosexur.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghiciydne.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gllbcmhjc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gkrdtijwf.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gbgfjipsu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gonvqwvqo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gcivstfaf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/ghtovwnjn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gjtucxmoe.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gkvidyfew.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gbaujvlnh.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gmgmvilhw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gbcfqzvtn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gjsczdkoi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gluiuzyoq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gudwjfrmz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gbrlruzkw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gdosxoysm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gdblprcmm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbkokhonr.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gacwgnryz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gnsrikiur.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gkowzfqfe.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gmkiyrrfd.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gonnhqicp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/ggleluqus.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gecjyteej.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gqccvzgdz.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gahgdqlna.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gebouaehr.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gjbdjkvrk.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gtmwucxwi.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gsxyrnwvo.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gvyjfcugd.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gpyrfjhkh.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gjlhdpiiw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gzgmxjxdr.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbczalzkl.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gfbvxpgqh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gzirzmbkl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gsoirtjuj.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gtuxrenqb.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gerzplznf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/grdhtbhbe.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gaezkpkub.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gbbkpsuiz.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gmdsumudh.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gcnbdagfe.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gatghitlz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gipcgpbiv.sHtML


<!-- 参考信息 -->