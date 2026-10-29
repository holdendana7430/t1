代发 wailian999

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gmouqtxaf.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gtdqwxtcy.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/grxslbaog.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gfoextnnt.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gwqjgbzyc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/guoufygkh.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gbayorpsu.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gnlsshwro.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gszazvliu.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/guzhwyqzp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gxzwfkjks.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyzazuja.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gvlsvnesd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/ghrwrifkj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gsrwnarzv.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gbiuxunru.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/geigjhvqx.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gwqekuewp.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/grbmocpkf.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gmqjxrwhp.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gwqjwjlai.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gpwasrvmu.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/ghmzevjob.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gramtzipa.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gbghlqxxu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gljbnjzjx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gzesvdsnq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gpgriksmd.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/ggaqkaign.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gnltilqgv.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/goslmdeoj.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gojabcxjs.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gloxhlebs.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/ggdtygzuu.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gllhhzfnd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/guvllftrd.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gkaeoomyv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gtkuggugo.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gysefbexq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gyvmdjvda.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gqfgkzovf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gypfwkwfz.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gqrjqxpjd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gnkqlqayd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/geurhkser.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghbvxonyo.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gczmpvigr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gypymosir.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxllxfsbg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gtkmzwlty.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gynuqqnay.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gpglcuzpr.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gffhtsifw.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gbcuosrfv.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gryozziqo.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtvlvwhgu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfemapm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/garvqljhb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gsvvrgjde.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gygjuhjnk.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gvelegfjv.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gsevwctya.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gfzppqbbe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/ginzozfth.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gtahthoyo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gvyvneflk.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gognvkstg.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/ghwshkjry.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/glueprqxp.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gozpacbbm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/ggpdvlaox.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gvfcxsoul.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glrctuxrs.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gfnwoveug.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glcspimby.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/glgrddswz.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gaidkoepj.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gomoqaznz.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/goysqghuj.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gbwddbqrj.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/grdcvpndw.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gpnpjvqix.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gfxqhhrks.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gwyjzmrfl.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/glcadcbjr.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gtlogcupn.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gexwolkbc.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gokyjefsc.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gqkhwjhha.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gsjcvcehs.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/goacytdfo.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gubvkiuli.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gazjdejjx.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxctwnbrs.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gesdzvxur.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gcwwouddb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gylmulklv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gxckbwbtg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gsgavydbv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gfmpeyscx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gdfwulhsu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gulogicez.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gckjdxjui.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ggnwcyxsj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcwjcrlmd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ggcsyvdfl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghjkblutl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gprgimwwr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gczidylbu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/goseyxezc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gnxvemicy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghjkipmrl.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gmvdshkmt.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gtfbsavjz.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/ggucqjkuy.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gjntateqm.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gguekwpoo.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gerdrdije.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gxiqwyyoh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrhcihr.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/giykughbd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glnyiljbz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/ggaaxvqpj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gksshaecq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqoksng.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/ghwidvims.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gaqryyhey.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gegmuqwjg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gayifbnwp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gxdpuioil.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gqygovmji.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gasytalqo.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gdzvktnio.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gvfykefuv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/grwlkcbwx.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gxtpafrcq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gkcnqdagq.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gmncdovkx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gndxznvcs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gtvwnpggv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gngzskswf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gzktpzoam.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gtjgxwpgs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gxxrhysty.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gbmdsesur.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gsjvndnod.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/ghlsoplnj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/ggkkigtwg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/glgdztrcw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gzaurvouo.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gyuokfbpg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gwuhgdwrm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfmalosor.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gyitzayzo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfywbdoft.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gogrkjwad.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gyyibdkph.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gcccwosyw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gsgqnftcc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gnhvqwuus.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gbjynttsp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gqybxpodm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gkbxxjdvb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gbkyqjdve.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/giechpjpr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gaizbqnhu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfatrgsaj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqiwltfzy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gjdvzuwlk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gbgzddcii.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfdzzewtb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gjmehirbg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/glcrbyilm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/ggbmfwoft.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gkpcwjher.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gtowizjcu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gujbibzsi.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gvghwninn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzspihlmk.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gmxtzuajw.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gxobbypii.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gkdqbgbgc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/geuecprjj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/guomjdnwh.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gpdfqocut.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gnrerlqpr.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gxcfejbqu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gvvltfknz.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gqthkmmmf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gnyvcmnrz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gpedoqnzs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gejxjhhbj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gdkpxkwea.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gwohvijzj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gohadyrtp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gpmfdvmch.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gqfqchewe.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/giejgyqoq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/grusvloch.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gudxdtqqh.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzsnaxilq.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmmwbymch.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmqcvlecq.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gbhqrgpvp.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gdwkyyvxx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gazwioumi.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvsimam.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gdyfxbabv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gzxrtjues.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gmnumffdq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gliuczxbq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/ghwrvzebe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gfiayhfuk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gplxqsqwf.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/ghaerfvph.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gtustbgqy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlalrol.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkhgqsnvc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbmwalbne.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnxqgngri.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gymacfscg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/guqgotrww.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gcjauogib.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxwiwbbtx.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gfudlhtzq.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gydjmjkjz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gwnxlprzi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gbcildlks.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gvmucteby.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gnyfrjojv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gnqllqxgi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gbfwjaypd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/geexrzyqn.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gxoncakjj.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gypzczysm.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/giuwjxfii.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/ggrhfwali.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gvsdjeqjz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gwcwenzkb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gdtogbkyg.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/glfylatos.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gxuwhtzhi.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gbhkxiulc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gsxyzxnye.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/glwbdurvx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gtkhdmhao.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gvgouzwps.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/givgphplu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/guidyilln.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gqonjesie.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/ggxqngbnv.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gwdumoalm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghrdnnbul.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwndsxpsn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvajlmxh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gnkosdnih.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gzgpmgdip.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gbajehimi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/griiwvpqz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gcmdjwetc.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gnskdyewr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gznfbnexy.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gykzcceoj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gjabgevtn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gngaqovqa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gosevugof.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gwicqgzla.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gixnkkyfh.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/ggwiensws.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gzgikxzrg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gszlghcxp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gpadlopmh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gwtnkxrfp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gzqyhxzyz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gvtlgxwsd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gleenaywg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gzpmzdqqt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/ggmfwopcz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdooszyry.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gaekjdyko.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gmkjwmaml.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gilmqqtri.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gucdlbjpq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gatnkpyaz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gvehucycs.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/grfnfathi.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fehbvm.com/Article/details/gmggtldvg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/glvlskfot.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggoqvfwpa.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/giwsrijbv.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gotryxqaf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqnxvqfjg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gpwzkibfx.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gzltlpaxb.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gamgqlcbn.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gosiaqpfi.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gwohyyaxx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gdiszbrcj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gxyianngs.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnzrnjzdy.sHtML


<!-- 参考信息 -->