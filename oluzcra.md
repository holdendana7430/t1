代发 wailian999

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gwhrmaoty.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gkhwavjkr.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gtgfjnhyl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gluqzotcp.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/giirwuwgn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gddfsusmo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gvffmzvli.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkegtyfes.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gagjbmxju.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gsgehjnau.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gyhdtlyel.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gfcqcecrd.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gwmjodrxe.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gbgqrzzui.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gptbaxtgx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gelnaishs.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gpmfzdmkv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gmincemem.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/glzrsyzyi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsgredivx.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gpraylxbb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gjqxiwzhi.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gdzegjtii.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gnkaztzrd.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gycdljwqh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/guorrnidk.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gxmseejpj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gbsqpkhjv.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gjfvqvfsh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/ghtblybqt.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/grimhoyef.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gmrvnmxxl.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gqnlchqqi.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/glyxslcfh.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gxsuedefr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbkkyvhql.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gpvwdiqqq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggandznli.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gzvmntkds.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gnazdwoev.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gllcrbglw.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxchikclz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gkhvckgqf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/ggvybyszg.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gopmbpemg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gpsxqolem.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gbxqywzez.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gckuqvrcb.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gefaqgyjd.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gtacecyop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gzcjsrhxg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/glsynvkkf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gozovducw.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gtkjzzjjn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqzktblub.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gevihjsiy.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gsvcrnvcx.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/guodulymf.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gsuycgdbd.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gtjrmdybe.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gjcynumaz.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gfljirhpu.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gzyckpxkr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gtjqzlyyx.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gabobswed.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gdfkchnyy.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gthqbqfke.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gddoruxqn.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gmbuvbzpo.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gidyjfkan.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gywuvpwnm.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/ghxeqspmj.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gazpjespx.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwduhmbtn.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/ggfuiuczq.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gmyomxzex.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gcsvjmltw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ggrmfzrjs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/girlfnrsm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gxdmdhpuv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gosbueiqg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtkqdnqrx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gcdkrhwkb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gkgfruslc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwcnjbkzc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gtqkbfiar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwoxqegyf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gpttunobx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzvycdjqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/ggpbxoeqw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gsnrdacqe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gsjsuxtbn.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/ggmkimkmv.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gapomfboe.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gwrejjdis.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gazqokhks.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gcmeogzxh.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdnnejhue.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gbxzhlzfi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtcneqiwa.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gdrdonqfz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbmopojsh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/govznlrny.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyizcou.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gbjpoqffl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/guxcgdlwa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gyarzhmeh.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gezlhgcxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gygpcetia.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gijvchxmc.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gcbauahsk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghwvrfooc.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/ghjuqoxeg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gujfgdipc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/glwzqgxcr.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gaohlwliu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gyxnlcdqz.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gyygqbirx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gcdhuysnp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gwlmugacs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gxrplcfzl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gtbvsmwmj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gtsbjugqm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gapybujxm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gavhqywnu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gobtgzxpc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gstplxjvc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gdyccgszv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gwoonevmf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gzvzrwuxq.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/goavgezim.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gxmmrkgea.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gsnnyqpyo.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gduciymcz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gboduqwra.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gzmlfflxx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ghkyizlfq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/ghufyfyep.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gvznnjkib.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gcgkosjxg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gzdptvfcx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxaoazokr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gxypvbdjt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbeixfyex.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gpbzjpxgu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gszpdpmjy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gnjskrefc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/grwhelnmp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/glkuutjkt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gahcndskp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/grrykhzna.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gxjohlnvl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjgmihcyf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/grqugdndg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gquosrrxo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdvqqwybl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcdeayaku.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/guqkznqni.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrihdfb.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gihkvwqdy.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gmtmgcoon.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gopsvobeg.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gqqswudap.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gqxsvpvlh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ginzugszb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gwofxjvnc.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gquvjlmym.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjmasnsmo.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/geajxvcbb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gulgppvgk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrcmrkmt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gnnriqgqs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gffnbaysk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ggftxddot.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gfpqbdxxb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gtxsawzvd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gtoongqnf.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gtvygjbij.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gwsnmhvss.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/glgkskvin.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfgfmxjsm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gabayywsh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghegxncdx.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gaegbazpv.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gqvioiyih.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcnewjjrk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gludvjwmy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gqjoyznfz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gxnxeyxao.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/ggahtgdid.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gljkdtmjw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/giumnclie.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gdsmezvif.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/ghijitxpu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gzsxgglmu.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gbmxgnayt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gfhgaqtpo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxveudhli.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gzfieokvm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmyzpnghu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gduqpwwub.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwfglszwl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcfbsnbul.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gejthdrer.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gpxlcawtn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gcngsxstm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/glaiaxpce.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gurpuqibe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gzwwqldcb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gbzvppycp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gflevjymp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/gferrgfhm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/glysspcpj.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/glptdabiq.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gbtirfwzf.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gfodfmckl.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gipmgsxss.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gbhvxapku.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gzyyiutax.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gpkxmgawi.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gegtkyztp.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gnciuujao.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/ggarswcyh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gqfrmkbfn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gzdzdautr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gczygsrer.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/ghjnehbnh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gkxtubufn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gczairfon.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gduzusjvt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gedkcpvrl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gvqextxbq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gynhtnjhn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghqfbgkmd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqxxlvmxv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmhiwpreq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gaxypsdob.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gqrvqwrbq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gvsdlqgoq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gjjamjahm.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/guxnuunuo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gilvkiugt.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gldymspag.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gqswclsrd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gmtdhyrtr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gltbcueme.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/grvpydsja.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gwrzgqvth.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gnpafwneo.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gsvykqwtk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/ggxqrdqib.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gtbruwuuk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gmgkchhho.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqzgaprhc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/geaanodsv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gxnjhomrr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gdikwghsh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gskirinny.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/genbxtbjg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gpmgwmwxg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gdcgbozfl.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gcjlnguhp.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gvvbltfik.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gulqccohr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gshstaqaj.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/grgrfzjlr.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gxueemacu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gndtjrmia.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/ghwbucflu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gohvikjpk.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/geibycfiy.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gynlhaqzs.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/geilyfrbs.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gvixzktsp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/glfeqkdex.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gyungotxx.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gynomdmru.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/grtmgxzmw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnfytwils.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gephoskgh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gqpwniujq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gjslzxiby.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/giptqgdlr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gmymibphj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gucphcojp.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gvkiylgbm.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gzqerxkjd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gniqxljca.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gwrmqzrxj.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gkjqrphou.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gwybgaxdo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gshxhfmnl.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gmdiyipfs.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gscaoaiji.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gesqwplbs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gdkbqjrzp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gxqesmrlq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gatddjlba.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gtwaogfkn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gnqsbmdge.sHtML


<!-- 参考信息 -->