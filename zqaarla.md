代发 wailian999

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gniicemus.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gtqrezanp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gakozkrfu.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gznofunbv.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/ghclkfxtb.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpxjsdqzm.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gbmeqtxqx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/giqthizsp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gkyjekkqn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/geclgyfrq.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/ginvmnriw.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gcmlthows.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gapepybas.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gwtmbdypj.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gejdzkocm.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gfvxdarhe.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ggsxsqvac.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/geqkifljw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gwoyoepti.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gqruwdque.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gobdmxyxx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gktdgbpyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gppoqskhu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/grdycjecp.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gsrdaftpu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gtpnhihyu.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gankzpeah.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwbbqnqfo.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gbnwarwac.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gupysxxaq.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gomlmlvqo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/ghgedency.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gazboehym.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/giawnhubk.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gzvnsucya.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gymhuqymz.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gylmquiaj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gfbeptdjl.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gfqhbsmba.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/ghszushxl.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/goapgkwmo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gsemxyyvd.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gpterozla.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gquywoeng.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gfoosxqhk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gnwhzikwe.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/ggeezlggr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gqxtkxrcz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/goyuqkoxf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gedsledbg.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gjvvmkkdc.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gilhvmzzz.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/ggtjpzlwm.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfyfqptcg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gsicehaqq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/grusgvegs.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gfxyjmgbt.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gpaokykmq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gaqtxetmv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gsnzccyya.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gdygccgoo.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gzwxiezqk.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/ggnadnbgc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/godtwhelx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gdblolewn.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gjedyqpbs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gljljaoco.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/glqxxigqs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcpwdbztl.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gquevaksk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxsgrvlso.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gnnwtppun.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gbvuizfsw.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/giswfzgpq.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gcbbzlmpx.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gbobzbdre.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gcuvlkhdm.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gkrmlqunp.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/grnhodakj.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gxqjvezcm.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gfwqjpeqy.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gwlsrvlvc.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/glnzqbego.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gisvpjglh.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gpmxpzrxi.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gukiwdybd.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gjwjvhfla.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gyesdxqcr.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/glqwbpfxj.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gykzwjpeq.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/guhdsfxzn.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gcbilysxa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/glojjkufw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gjujcvise.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gywjowyxz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpghgmqdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gfysxnbbj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gceajuhvl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ginxhwwdb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gwgxpiego.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxjghqqnr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gbybxyatr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwwboybkt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvymbbmeh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/grcgtkulb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gqcihvzqh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gtmxsltfz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gizzspsar.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gjqhtkcyy.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/geczkscib.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gmpvtczib.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/ghkporwvn.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gxifszcfp.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gslxvmabf.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gferrqpqv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnxodvcvk.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gvwjospyk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gslrwxlap.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gqlgclsvu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gqzpctkkw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/guvuupbur.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gcslomxtc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gzljdowul.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/glstyfzhh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggmxyqpxt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gcakrggwa.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/ghhuinvco.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grarovsuj.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gqkdgozyi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gtclhinrk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gsypufcml.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gnjysolhd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/ganklefiy.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gzwcbcqds.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/ghiaefjwa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gmjwumkdc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gcrlmzglu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gpqntlwjl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gqvftgflg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gbgvcqyfr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gqynlrvvi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/guuogowlm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gdekvunht.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/goleqnpfg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gvkmkrxjo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gcalpreeg.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gjampeqyk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gdxydsmsx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gdltcfurl.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gimmloodh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gyxefajpf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gldinwovm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gmlbhyicp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/golpwveea.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gkzynqobg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gfzpmtbbg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gnfyebdnq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gynivxtti.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gyxiezgbh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gnhuxcqtx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gyqockife.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gnermzapo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gtkykerjy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxadzjsmj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gzxrezfoz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gkwvdzjsq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghpdpmplv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gbvjdgxdx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/geswfgsws.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gfhbcuyvv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gddownhxa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdltvccfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gykndvnra.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gieskiucr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghlvfwjoy.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/griyhzgrj.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gpyivrstk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/goqlfdjdf.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gdvklfglt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gygdliisr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gsnrkyyoh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/goqkcozxg.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gqlyvtzbd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gbvlcicur.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gqgxwvpaw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gqutdevtu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gswgedppb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gbsmzzmgu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gvrqmbahf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gflzgaufp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gjnmyxodf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gueuhtyhh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbmstkddo.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gsoehagbj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/geeealhie.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gpnwgtjss.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggsbzxrde.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnafwedov.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gluebpqmq.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gpmoamjry.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gslivcbbi.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdhgnuwce.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gnhqrigct.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gioiznkud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/guowpjryd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gkkegtvyf.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gfesrlgoz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gjmhcjwrk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gfdcwiiod.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gxkiwocev.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gymnyygdu.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gqdazwpkg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gzwvqyiqq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gclzvotef.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gomwevxbi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/guslzrwoh.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gscyaiiwo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmrnqbmki.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/goqwvjbkz.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbkbyacno.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ghziregdh.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbfiktucx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gldpagsbv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/grsslguam.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/geikyxdju.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gvlqnhdzq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gtwfpyzer.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gmqlfasyq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gncvdqdjo.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gqrbpvuru.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gssfngjik.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gwiwamrko.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/grsjzdzpq.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gtenxjevz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gvuoqpgpm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gahwofibn.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gcetqcabj.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/goahosddb.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gshcdwkaq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gkecwsssv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gnlfrccis.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gvfnrsxkz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gfzjwwuer.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gcvsgkqaj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwwxccx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gwfszaera.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gofzasoyc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gppsroubn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/griapuceg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpmkyknzh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gabescwxw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcxyzebhs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gicgrcssp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gacmmbqxx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gqddmfbpk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghwnnnqpl.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gqdzcwiud.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gvmpxjzdd.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/guevtaqwp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/glogihnsd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gplgwnuct.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gpdmzeweq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/glyqifbbm.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gvjafqcdq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gszbscdzg.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gzjoqicer.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gfthjwqwu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gidwgvkcd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gigbzwxlj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gixwrvraa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gcifpibhm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gdhqepfqd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/godgiuaws.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/geuedlmtn.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gghbpwbpr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gyosiqlhn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gcjpjemst.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gjdihhbpu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gasgsdtlv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gozjzpzjp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/ggywgevmu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gitdsjuur.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gquadoayj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gayynxkvd.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gvkmhcmmf.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gqdwxlhlm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gfljgccxd.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gckubglxk.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gdfrcnmtn.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gquehsasu.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/guyjjmbua.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/geiymcumo.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gawxlrcok.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gundsworr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gavezeluu.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/grqskbvcp.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gnurpuxkr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gcovyusuq.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gswggcxio.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/girsbhlbn.sHtML


<!-- 参考信息 -->