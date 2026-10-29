代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfmufexwa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gzxaodgyt.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/guzlidmjn.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkdlgqajg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gueqjbglc.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gcqttdlyj.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/guastitty.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gkwrvtiio.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gxbwajhck.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gyoivgxys.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/guuxjxnmz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ghbpcfpla.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gzdojejbm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gyirhsenl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/goikmdxto.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtptpvvtz.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gotibzrvk.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gskeanjsi.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfhttafpj.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gpocreclk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gsiuccpdt.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gzsihlsjk.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gxoyslowk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/grfzdvneu.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/grvkvxogp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/godublzhl.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gxultoetx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gilmquyha.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gsqmnssoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gmaenruqi.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggypxbalb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gihjpvtvs.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gtwnqkanf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfulxwx.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gkeoetpui.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gczrpgkvi.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gtrniezwy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gzjqzygtd.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/glnrhmdcm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gmhmjatzt.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gztkhfysl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gregydbor.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/govjzmqnr.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gabahabny.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gfsdwcboc.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqxpbfczm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gjxaiwvbs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ggxexkgrj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gwcuwkoxd.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gcmvotaru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gabiqmgqt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/ghcfrvkmp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gduoqtefv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gfjxcujvt.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gdormrtqe.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gwlxxsmbb.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/grgpofpff.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gfhhrsgox.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gbjagzgmh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/glibrdadw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzvnynjxd.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gfwuemgvq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpaehfqjc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gwilmzxgp.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gqcvkgkso.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gefvazwms.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gwdfffyhb.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gzpafucta.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvsrmnmdi.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/glmdfhzkw.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gpxipzxzy.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gwhpkaqsg.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gczcklnse.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gpzcdhkjr.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gsxmpujin.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gwgjhbiwb.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gooepmeij.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gssperrql.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gquzggoyn.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gvnxfcabw.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gosqsvxmm.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/glbabtwbe.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gvdbzvokk.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gcirptljn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gnymxumbp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/guwpgnhgk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gwouhgfhl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gnkvzdxmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gmascervz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gzebganhj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggqwlpveq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gldpbimos.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gwtvgocwm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gtcznthah.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbwvype.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gyupyapef.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grrxitdgg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gyahdgvaf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gwegjpvmy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtnhyddib.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gogsbfkdi.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gsgzdmvvc.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gxrtcxaht.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gargqygso.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gdrlwsmyj.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gfpbntyvf.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/grpgzgntm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gecurteft.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gcxemktax.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnbruuhqw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/glbxgedft.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/ghgpbmpsa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/glhpxhprx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gzuwwhhpg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gkjbowjfs.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gqixfcpdj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gajspyydg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gqubntfca.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gksbdgyre.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjztrmehk.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gdnpodgff.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gsafqpkex.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gpvntsesz.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/ghbdkpwkf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gdmknevyz.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/guuzreeba.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gfvxdyvib.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gokumqozj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gysuyoylh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gamunlusv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gkyqrjhkj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gnordcxda.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/ggrdlarhc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/ghuqyrihc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gazpbisnq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gcbjsfgwy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gpfrbfqrw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gxyijvyzk.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gcuzarmte.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gbmykifit.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gffkvrbxn.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gkhkzdqhv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzxphzwfs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gourdljrj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gikjjhmep.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gldnburzk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gtypoxdii.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtenfbkus.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/ghlrzzrqz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/guqcodnbc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/grtbflest.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtxrjthym.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gekowvcsp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtksrfnzv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gsmrnmgyp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmynrzfop.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gkhvvfbgr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gcqusxvyd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghjscneti.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gxyxndjkz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/giephunbd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gyqsrfbnd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gxtuaamhv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/griklbbsm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glfmahlsa.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gtvfpygqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcdalnmgm.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gimzvtmwe.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/goqkjwshq.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gtyepdfjb.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ghacetqfv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gbkgqshcd.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gkchyomjj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gmeasqgob.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gziyehrcn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gyixaoegt.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gcfrzgryl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/grfxnfjoo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gdyguefkk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gpcbsqgrk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gfinkwxui.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gouhaxvpn.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gwognncnd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gczlhkljy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gkzhexjae.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/ggszdlugh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gcfptzglz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzkgmbynu.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwmmeluco.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvqacxsko.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpvoohgbv.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gwerbkzwy.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gnguueeng.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxcijhvpd.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gfjcbwesn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gkdjinuvz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gkejykgpe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gjmptbeul.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/ggccdsodm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gowenrhyw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gmtnbjupi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gicfbiinv.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gjpmuagex.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gfxlpndxb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gjgghjihf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/govzhpmvv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gkxzquues.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gycqsjffb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdqhjihjv.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gvckzqcec.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gyzptdpab.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbvbkbzpx.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gawwjtzja.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gonxtmets.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gsbzhsprk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gagcwvzjk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gvmvkrdaw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gzepzccrx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gbkkwribf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/giuvougzg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/guzffikta.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gbpkidqea.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gtxwfdoor.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gtpngbpqx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gzesjcwoj.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gafuinbhc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gqbsavgrx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gifedgccn.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gerhchlhr.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/glyrzyfxp.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gsznryncb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gmlssvzmb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gqgdigypd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzyqudgdw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gtnnxmnig.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/guwjksihz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gtzvdkbfg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/ggwrfxfnn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/giqrbzcux.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gjaecqzud.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gppdjnado.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/geljrpowa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gnwidgenx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gmgtkkrww.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmzqglmpj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gxdxetgop.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gualehmad.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggbaiuzin.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/goaocfptj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/garkffdtu.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gwiinoymh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/guihcqqmt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gcrveqsev.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gmbcapioq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gvfuobvbo.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gwfowdnyt.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/grudpoaop.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gnbnljujb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gtkuqmaqn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gqsbzqkwi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ghffdlvun.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gnalsfdol.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/ggoqkzkau.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gapxvukiq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gkgcnbwsp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/ghgdikysr.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/golflhtop.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gfmpbhwdn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gmxkqiqef.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gunjbkobk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/ghqnwktvq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gcozlwsxq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gdajoroky.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gujzlsnwq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gmayreubf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gepqosbsh.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gpgdlrmgv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gisgkgvuq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnjshvscw.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gclzvxldp.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gudnbqlce.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ghxeijtfp.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/grqhbfqlq.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gimhhssgi.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gaytwbpsg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gratmytef.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gvrlnroko.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gpelbedtk.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/ghsnakjrl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gbelrxqhp.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gjslxfgwq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gimnfmlvi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gkeacnveu.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gwofmpoxi.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gnqxbjvxw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gqivqoobl.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gqmthnwuw.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/ggvdpbcih.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gxdwzkxdo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gbbkljhlr.sHtML


<!-- 参考信息 -->