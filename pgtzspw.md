代发 wailian999

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gitohhdte.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gipnqjtih.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gfguzomyp.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gwpoxczoj.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gmtnbqvfy.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsdiobxau.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gaeibhbdq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjtswoaum.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/ghnrksdpx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gqkauuxlz.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gbzyegsqy.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gprhinatf.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxmvvyqwt.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gneykzlzw.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gjalbuhfl.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gdmfbaewx.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gxrffnebv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gkirhfqwu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/ghsnzdnri.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gmslhzlpo.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/ghxxahuwt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbzmymgfd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmxauzlur.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gakbqpyyc.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gmjclaxzz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gmkqdrjxf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gnhcbvszx.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gbaumztdc.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gvyvotfqd.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/giyeqaalf.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gawbxjdqm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/ghbzcpcey.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gyvclxegj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gaunpzkwh.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gjuxkpwyn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gimikgclf.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gfwyxiwzg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gzazdlvhc.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjwtwmwcz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gzfnccwib.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gwdjnaesv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gxhbtmvns.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/grxklhjqc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gxshpnsns.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gglebprqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gzzjwwoly.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gqvyzopec.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/ghpbwgyoy.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/ggzeyzfwr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gifvrplal.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gjvnabmuy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwymppjti.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gtfdqezpr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gllajoevb.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gycivslpw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gpoapwcaj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gzsmegdcs.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtxriqicm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/ghdtxylez.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gshzrorik.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gtvpmfmlp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/goystzpkx.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gsackfvfz.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gfvknpmez.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gbwynumml.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gntxtejqr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gzhqsndzs.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/getcyzyxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqkxrlauu.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/ggqvzyjtw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzozydxrv.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gmnuoaycd.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gppwnpdhe.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gqshlrbnj.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gbfvshqlj.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/ggxkkihxy.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gnjagxaxb.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/giqepjxtf.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gtncfqavm.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gupdrkmer.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gxzcwbozr.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gkjfassur.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/goltdswvk.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gywkepsgs.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gsehldraf.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gclczwcaj.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/grfkaklct.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gezmotnmd.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gtgjydghd.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gwgzjnjil.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gaswfiarx.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/grtiwwfch.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gnoimhjuj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gqrdorfgc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gurhltaqc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/ghylmcxar.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/guedmrayu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfnuhyose.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdmdcsdqt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gikqtdzec.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkgzlnmfb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gjlzjsvzw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gyrgrlzco.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbzktqbqb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwzhvzdxs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gieleiczk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gusdqmnlt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gawbdhbui.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gvafbwbno.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gxffjvtol.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gicclyusz.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gxpnpmmgx.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gsbgvsosz.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gytvzumpw.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gksobyosn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjxiqgvuy.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gykoolzqo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gffztdbdd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gobpsskyb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gptyqocbe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/govzrzwyt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gohsxnzxd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gczmbcomd.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gjcyvplsf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/girgekfpe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gtfcvzodt.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gwppdylus.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggczdswri.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gmhrympdr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gcwljsvdd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gmiwppsoa.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gzoiyplkl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gmoyqkiqj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gxlmktctm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gjvzeztfz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gwgmtpznb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gxfjvhioy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gcyyahrha.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gxmfospxb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gjgjnwrrd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/guafkalxj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/ghqkhzrgg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/ghtaagsyb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/ggvcjkwea.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gigdsxmch.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gyecuzzft.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/guqtemved.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/giygozrrr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gohcryufn.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/guknqexfo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbzeiyefn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gvcpjhyoz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmuehbben.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gtpeihgya.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrqsyigu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gylbuxkad.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkpeqilfk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gcltldxjh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gvavkwtko.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gojcwnfrr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcndsemwq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ghhxhcaeh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpcooosrt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gnveoubjt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/grgjwjkum.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/ghzbihgym.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmwntwbxv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gqnjuhvma.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gtblgapvp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkoqxtrzc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gkyogugwt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvcmboixs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gneidgywa.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gaovthbxk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjydhxwme.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/giwsqzxeg.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjafudj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gxlaishwy.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/grzslthdx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/grzrflvbn.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkqsemieh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/grgwnoxmu.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gocrrqjww.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gmmfczkki.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gnnrsroec.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gvfiagxdi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/ghjqolbda.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gmivwzmdd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gchstemdl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/glseucpek.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gyrntjjqa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gbqjywmxa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/grrvkuend.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gnlkmjutc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gfwlymbkb.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwvrayesn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gstuiccay.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpynfpoli.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsxlfaqrq.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gkpamytky.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gvkmafbvq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvyjhzqfd.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/ghlqsgflo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gmvariorx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gvbbyukam.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqdntdr.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gasqzqwgb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/glreoxspk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gltowsbrq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gtkpiruzt.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/guhbftsxq.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gdiqhcstl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gmzopkgsh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gzfympesc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gskvyqrks.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqycizjnb.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjgawmoml.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbyimqnhv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpmdtlrfa.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gdnejvxaq.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gqkpzwegh.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gmikyygec.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gpntwinpg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gxkflgnfc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/geacxhjlp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gnnwpevox.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gzlvkmojx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gtxsbxqzy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gsocyaiwr.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gnleacbpq.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gjvahhcyk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbyvppllt.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gyxtqkqpj.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/geiycrfmk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gqqwzvzto.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gfwmrpsci.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gyowvqkal.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/ggrqilzwp.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gbiddmife.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gdfwiaqtl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gnmsjpghk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gfrmxzevh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gcpnsxxwb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfimyztuc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmayyiwhq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gsebldnqq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxbuzyzlp.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gfmoiaaji.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gbvpenifu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqekrrboc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwpeqcsjr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggfjaxixc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gaxxusaet.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gjzkvjsxp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gylphqxqv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqxctyadg.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gqjbukpst.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/glwonrjns.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gmiijlkfy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gdgrvabjv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/ggiqipsma.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gzuksrwgo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gfkiduojm.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gpfmclxzv.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gsccfcbph.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gbtnosarw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gkypjtmds.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ggcwbtvzz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gutohuiiy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gmknrwtmp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/geczvabnt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gibybrdzz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvajlekbn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/giycedpys.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsvbnladc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/grwovuqty.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gwmnaloqd.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gopuqixnf.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gyhkwptio.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gpqomlgjt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gxyqkqere.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gsgbbfxxk.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gnkvdcela.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gixrcymoi.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gesfjtiez.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gawhjohtq.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ghlhkqqkd.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gmzzqdeau.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gdaazstzf.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guabnpnzm.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gfmcilcle.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gquhsmlhe.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gyezqmevm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gtpvmhhus.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gogijtqex.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/ggthfrgoz.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gpcpfcgfd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gzehzunqc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gclnueojg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gherqapzr.sHtML


<!-- 参考信息 -->