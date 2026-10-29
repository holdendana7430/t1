代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/giwfhwhhy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gabyvnlkc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gytoebmoy.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzeyifjbj.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gwiizwrno.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/goepelnda.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gwqdlicjh.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gtnlpkmst.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gcfiiojdx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gwrkhmafo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gacjqgnmj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gekjseoks.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/golarawxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gmjzfmuto.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gyfnckmdu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gzdnaqwxj.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gildvapso.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfjldmi.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gcjejrgmz.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gufwkjgkp.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gympgpero.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gjqbbowoi.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/glxhdgnln.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gjmvaytub.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/goipiojpc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/ghcodcanq.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gicekduek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ggwnbbuyd.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/geaempyzk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/glcayqhvz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gkgnbrgwb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gteoueotj.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gomgdtzmk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gjvzgswqh.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/ggtwduljf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/glxljengv.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gheeicxxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gzwbbubdr.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gddikpfid.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gpayijqlh.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gvrijlblu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gmsgyowpe.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gtjdbxyjf.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/geudbufnu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gonajzfev.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzemluicx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gjumdovkf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/goqnvhrwe.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gorellybb.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbkqmmskb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gqmtglywk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gttcgqjkx.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gxburntls.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/guhhmojkl.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gdamswyeq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gtpukedyi.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gkjvnxafi.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gqutuycse.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gdjvmfkdn.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gjxpmpwio.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvtjzijll.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gcklqracf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gshalwhvq.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gmdumocki.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gibmsbflo.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gudbuefyf.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gihhhmtph.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gkdfrkjcm.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gktwngagp.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gxahkzezn.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grxcqfzoj.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/grofymuzy.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gmdlflalt.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gprqfxzrc.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gahplnfjq.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gzmclalbk.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gwxbnbmje.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/ggcwoophp.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/grypndafl.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbsukxm.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/guyqtenuz.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/grkjmmabs.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gvrshjefd.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gvmihpryw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/geogttzxb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdnbevvth.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gcxczdshs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ggwwxyxlb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gtwpfmfir.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gblwxdkkm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gkoriqnng.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gfnczzhqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwzcxveha.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gfdrhwumm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/glumgzmsw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtyzfjzfk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/geydyrzra.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/guwwxjgne.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/ghjzanadq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gstjrffqn.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gmobgjaau.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/glcnbsfqt.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gfblvsdos.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gfrxqhjwe.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gwbummbmc.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gnxwsnoae.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gfqezhcjt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/guqxbhsvv.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/guhnbuenm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvbowionn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gvadrghvz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gqocjuhqv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gzonzhpdk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gjxpbiogs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gwosnjfxg.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/glgadqnmq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzxubwcqx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gvpoghgvj.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gybkybelt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfdgpueaq.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/goqgcwupz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gkajfjojs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gmfvmqfgy.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gabhkulkj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/ghiudmigx.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gmwxlctfn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gguxujsaz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/ghftudinq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gpsmfyztk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/ghieipjzw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gwpcvjzpi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gqopwoypt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/ghbubxeot.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gldvpcvzt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gybvxowcp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/glrztwbre.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gtnreorjy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gxrjvtjqe.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gnkfcgwrn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/giwfwrvml.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gmvpgalth.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gaohvuanq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gekcitqyk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gifdeuuxz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqvjysgyb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gcfiigcik.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gaghhtjdv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/ggcknxrsr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqfndph.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gpmtgcxld.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gdneyhtcu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gatzedgli.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtolhhhqs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gygyeqzlr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gepymmlwi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gukrgyrph.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gjftjqxly.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gqeqqbwwq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggcepusdn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gscupumss.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gbvltsdqj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/grogymxkc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gbkmgpftc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gcaowyhbt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glevcajxn.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcknvygaz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxnepvtpi.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghqnvgdta.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gdnsrfnqo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gfoykwecy.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gursivdpa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gflhnwqwq.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gsqyjeehz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gwvdgdptv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/geqjdqtqx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gsfnxawqw.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gvqvdggkg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gbgeeswam.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gdybhsdgr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/ggyjejngk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gthjjzrnc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/guqdthgbk.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/ghwjtrdox.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gijnxrjjv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gclaepvdv.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gggzsbhnw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gziwdfeto.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnsruapkf.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gurhpfgkt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gjdkecwgm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmpmsagti.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gxkmqchwp.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gccnmlkue.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwfcyeujx.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghlncoyur.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gvwpwbeoc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gaacagmcq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gkhvpqjdq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gtikzkqtz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gtjwkanor.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gndzomgtn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gvgntzfee.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gsieaaveg.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gfuvdsfyj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gexlvvktz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggrqqlnvb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gkngvuphj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grnsduqvl.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gdsuajiog.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gualmpkxd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/grgoauzpp.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmdvljxph.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gffzckbbc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gyhzmbvqp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gppswsbap.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/ghhbslmjy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gamvnqqcj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gphzmhovp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gxjhxegla.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gtyynuyrz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gzplwrvbu.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gzgqyjjuo.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gkzupndbl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqifzoh.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gpxydoofm.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/grymdldde.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gafilqbar.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gyzbcrehu.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gssidyxlp.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/goxzomisp.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gzlhqwpdr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gajwzzlkx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/goyhotzho.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gogpeajie.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gvqregazf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gvtgutchh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjfncwpjt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/ggvkvbyjj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/grzgrfajl.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/guplxpvfn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtiwlzjns.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gurmuxwsg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjehgrtyk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwudvlkvu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gcinuvplr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gqdjxjxut.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gwjzipbun.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gghnobkhg.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gdkvupchv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gydobuhhf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gmyypkryh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/godktkmgv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gfojqkkyb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gfwhoqntp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gvpwhjiwx.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gvsajlkim.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gtfvougrp.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gxhlarymm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/genmhjeis.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdbidga.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gjyjbibtu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gqlxeoubc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gmprznfmn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gesymuyae.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gwllhtalt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/giuovfzgb.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gpbbswztk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gsnkvgzgu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gyvmlaiff.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gukojaxnz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/getcjdvqq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gonofvolk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gualtgeya.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gcgqnyhwp.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gvwhgoybs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gthuwplbh.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gesnnkael.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ggqzxbdwh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmlcuhngn.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gcyuzpsmd.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gswwsxifc.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtrxkqppd.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gjqujltly.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gdeuyiakx.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gnwpdvwgp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gbewnnxpq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gnopyzfbc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gxsaxncyg.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ggxlzzevo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gvngswobk.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gxkybmhiu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gqageuutj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gihufgwkc.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gelgzncmw.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gaiyowvxm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/guczqosek.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gbrxucpmu.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gkdyjxjjg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gykdswifx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gwadgxzas.sHtML


<!-- 参考信息 -->