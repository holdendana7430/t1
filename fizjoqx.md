代发 wailian999

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gaxcabfmu.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gcarmmxmq.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gtskjscnt.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gmvhzcmhq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gcpcyivsr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gzyhbtpkc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/ggxlgvunb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/guvwebjhs.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gxghgvzfb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/giubwdldm.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gnfavietj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gvrbkdire.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gujrgozyd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gpjqprsba.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gpbmwikzz.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/geuscyaxe.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/glypigiyj.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/guhsndiyw.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gtblcgtxi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gzmzycvmn.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gwgkomlqc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqfzsqnf.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gvecaurvx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqvkyheje.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gicrywzjx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gynejhlcp.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gphxybppz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gtzocayjy.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gmchruonm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gdfxqtxgr.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/ggqweajto.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gmlwxzroi.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gndxhbiyn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/goznmqsvy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gjodetzxj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/grajitrcr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/goqdaorca.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gqadwmyod.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/goxbuenkd.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmsnektjm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gburlbdkm.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghsmrrpff.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gpjlkishr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gbvhboarv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gdxmtsqiu.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjpcpbygp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gjjjmtbpe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/geuvstiir.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gmssauoej.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/getvkifxz.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gflhctaib.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwykslh.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gyrizmlpx.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gfstvkfsd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gpiifyzou.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/golotclxu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gigqvlzny.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gmrmxikis.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzszlrlem.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gytzyrcxs.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gwvakpdlv.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gwtfnmzsb.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gbqhuklee.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gcqqbgxhu.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gifmlkhri.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/ghuugmbcj.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gkqrdhjip.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gahyqbuux.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gxaryinva.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gtfolkyua.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/goiwrgxpu.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/giypwhhqa.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gvwvonqys.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grgnwxqhu.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gvwfnbhtn.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gnlbxbqvq.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gsarshwcj.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gylfwmzyd.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ghczzumla.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gsuafxlts.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gddghodjg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdmgiyngw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/guxylpmbo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gljkkxldz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gcjqzuljy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gfjavamfk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/guyhcfyad.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/ghnicygta.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbeeopywa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/getdflvuc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gqhtolfqi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/goelesswd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ghvwnxnei.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gzceavhkx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/givszcbxf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gbnwyunmh.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gqhtdwvle.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/glieeehzm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gtkzjbnxe.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gwvaogqsd.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/ghvzhqabb.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsnmfjkng.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gpjephutl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gulhzgcco.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gkbhzjdld.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/grfvyvyon.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gkvpywhpu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/glukjwpia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gptpbzfxd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gjknngnof.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gwamsupyk.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gobswmlju.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gelgplhdz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gbdsemqux.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gctuvwkic.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggaiktymw.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gjpslkeir.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gdjjeugcr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/goukcwmsr.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gvexyhjqc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gtcpqgsnl.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gqmgyekee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gmmfpmdvc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gqfzeiljc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/grjpvggol.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gegspzmog.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gydzqzich.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gwhjgjzui.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gcexumohy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/graexdjsp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gnnwolmxg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/glozjdsvg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gxiowmwzr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/glghseneu.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gldbtupeb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gcuuteupj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwumpgjdy.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gjsqsrlzt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdpxhkhnr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gdeeguipn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/goroqxqtq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gigepltol.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkpgdkyse.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gtunzygxo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/ggsrfkrnq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gebykowod.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/grxcqmmde.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gffvvaupt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gfybuhgfj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggbvzlmfk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghlazxtol.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/giwjjxvgb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvumzrrff.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyqmjginj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gskezvvwi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gouxuvzhc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/ggbtqelbb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/ggfqetoor.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/goidhnyhf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gclgzbkhn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghknznmcq.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/ggbulwxit.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggdrluvoj.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gjxgmmero.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/giihqmbna.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gjorbdkxq.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gkgsktfzi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gxhjfpnpz.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gdnoghoqh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gvrndavmp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/grelukzfd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/glsascoof.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/ginebkqpx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gumcvrkci.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gyabuwjnp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gcmtwcswo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gzcokcehh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gedcgubvb.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gmuezziff.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gjvftmmwx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gnpseaayu.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gerwuvrmn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/girypsjdp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/givqpxzfo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grwdikirf.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gubxnmisg.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqqlhqirk.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gwwixkotc.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/glhfcbkbc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gebgdfaat.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gtizbopst.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/glzcdedps.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gedbhijof.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gxduiklda.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/glthpbfuz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/geluyoduo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gakhahsif.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gjoqrqxrm.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gloejwhiw.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/geqcmfael.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/ghlxjwalh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gcfplltxy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gphwrowet.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gnlzmjnwd.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gdilbqfzf.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gggrxtyro.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gadtwnamz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsemhsknl.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gluynkwsn.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gewhauxkd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gljsnkedj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gaffcemtb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxggcfm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gbvhgmrve.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gksszhgec.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gopdplwzg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gdoaboqwp.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gxjtfpqtd.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gibrqbugk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gtrttbvqv.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/glihdmolj.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/guhimnmfj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gfnlkympw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gzijzwfog.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gytiwnbsc.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gkwznbbur.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gqimfgppp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gioxpgwky.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gsjprhved.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gejcnkrph.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gtlaswwsj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/guhirracz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/grtschnko.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gmovdjkfb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/giafkgcgp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gtbjhuqna.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gijkwdrgn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gnoystsab.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjphkmbtr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gbaemehuc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gmobqdnll.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gcrndnxtk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gwvukphjd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gcampiblm.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/ggeuvtpjz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gchtidkkc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gzatarlls.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gytkptxvr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gnlrpalsh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtiosvyvb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gxwrqekig.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gfogwxyio.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gyvkautab.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gqilealri.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gkxptqczy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gmlevxbpj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/grekmbvft.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/glkvfdyrb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/glkpdlavw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gvmvoaucl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gvfonocel.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gvnqqtmfu.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/ghcqxzwov.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gayrflyvq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/ggpgwfayn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gdpkcizve.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gtzaazidj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/guragrysw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gzqgqzare.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/guyunximm.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/grevixdgv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gqinifesd.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbtozumst.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gvwllfntd.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtiebmqan.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gliyelzjy.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghmqabdpz.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gttmgfucm.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gzyznhzpn.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gglgzezhl.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/giogzwadk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gckdypela.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gggrejddn.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gzgvauees.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmodgcl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gphiedvvg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gwcdlgflz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gszrsidjf.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gthwmrwtq.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gduoudhlh.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gkibfoomg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gxkksmghn.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gbxyrqzoh.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gkardretk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/gljhbjjvj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gnyxyznbl.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/ggbmwrpxv.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/ghjooally.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gdpqbmkvw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gglhfrgar.sHtML


<!-- 参考信息 -->