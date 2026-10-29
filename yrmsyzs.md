代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gadioglqr.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/ghtfgqgvq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/ghsstfvyl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gtktbyrks.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gymipzkmr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gevmheggo.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gkpekzfvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gawafaegm.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gmapgftln.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gltxrghxn.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gntoosrlc.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gtqoamomg.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gwocfumlm.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gthdlszos.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gqnhasoji.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gbiucwsdk.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gejfzclsj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gqebqpusm.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gyiyhhskw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gisthufaj.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gphsvqpvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gptfvayth.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gudhsprhr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gzrfdghum.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gicuzanzy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gufdbyunv.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gxidqrtuh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gboohcidn.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gvsnrlmhd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gszkndfqa.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/ggocdxzne.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/ggeaxgkqq.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gvsdoimyo.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ghuadmclp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gywcadcas.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gldnjyeft.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gelcqpajq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjggcuaxm.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gbtllrnui.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbdxoinux.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/ggllagcor.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/glahsvxsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gykbsvbyr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gqhydpats.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gypxxwmex.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gcdwolcce.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gxhgjisfo.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gblegoyad.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/genudjikr.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ggrrgmehx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gkvagltqb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/ggjrudcil.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmkfxyppb.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gqlfztlaq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gubqxoifr.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gyzncxobf.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gcpxupyed.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gmlpsxnyo.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gybjztjck.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gqeadeuwk.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/galqdcmnu.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gstouhkyy.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gunxntfzu.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwxvwfnag.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/grxpybplj.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gvgrduigu.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/guiipbwbs.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gaspbnvgo.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gixlxhavc.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gjrsjbsxp.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gjwbxpowq.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gwxqvozsn.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gvryjgxfd.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gudbubdsz.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gryajtzuw.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjrehxn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gmsbcxzss.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gajnpmjtn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gwhwmhhkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/geutadvjt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/geytnkoae.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/guruaxeov.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gsbwdihyu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ghfwfokix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/goeuosqlp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gkeswigqk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqeprsglq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gzeassxqp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfohcyxhw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/geozhuccw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gglstbefw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbsxzkznr.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/giugzyrvr.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gkstnznke.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gmtmhxvjh.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gbnxwmkoh.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gwwbbbwyp.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcjywzvkx.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/ginesxouv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gyrxgukbs.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gxgadhzyv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gprqjosvt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gcleezsot.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gsbbnjujg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/grefvbtyv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gacybwefb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gmkhvzlfv.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/glphadzoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxwkcbzfd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gbxemunbd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gwwugihcz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnhotzyzl.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gwalloxvr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gnydktzyt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gocoaedov.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/ggtbeuymm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gzmcfbosp.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gntbwzjre.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gnmxgtxbf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gnfjxtatr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/giscsvnch.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gfsabcfpn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gbjmrture.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gylllruyv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gfpnrceio.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/ggdishexz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gtneuixuh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gllhwfuqe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gunsyrkiu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gtgstpmmi.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gesezjsdn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/goacvcnln.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gtqvctriv.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gtsciuntc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gxpwsgyga.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gadbovxyv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gwhthobpd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/ggdutsumh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gkyqowinj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/glnzfqham.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyzpnuyun.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grrazxxnj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/guealzgrc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvsxgyrbg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gwxlnmhxw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gujsfkywt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwclyfcxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gyvrclhlz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gwghsgvxr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/ggflhhmog.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gtriwspjc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gwwqgxmhd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gjplygmwy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/ghyyfxpsz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gqxbosjgd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gzzloifoy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guofdweds.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gtkwjrilh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdoxbglyr.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvxetxkgb.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gvvzevdne.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gfnjsnulf.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gduupfcqm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gvjxwrqyg.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gyrfbelxk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gcsmsxpbi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gqpsxpelk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gnbtleden.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gpsahpeka.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/geangxgrw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gixjqsesp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gchuorush.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gznsgeovj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gtvrxtjwm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gsttfqmch.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gqeuerokx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/ghtacwjgs.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gptnfjmuu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gnpytbrdo.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbpgxiaqa.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzgxqcdhp.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glizrelzm.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmdzijqek.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gtgmexaef.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gvbrjqgzk.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggkaxomzl.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gumuqfgdx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gykbjdzor.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/ginhpknlp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gfzryxzkx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gkpfzamtx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/ghulxakfc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gyznrvkiw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gwlxefwdd.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gatbzxaim.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gpbqryxfz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/ghpvduott.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gepuiznti.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/goifybeox.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gugokwygy.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gerdelhnl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gdtfhmrir.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gsxdqhsaw.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsecukrea.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gslwgvzcc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/grbfmnkmm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gwkjksrcf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyocbhar.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gwwnntfed.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gyyqxygkl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/grjfacqah.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gbujnamet.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/ggtywaklm.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/giclkojdo.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gobimmcvh.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gsfzuvdjt.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gbxgltows.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gbqljlrdo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/geuseunry.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gfqtmehhr.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gltzrxvhr.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/goaxkynxq.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gotogkxbj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gswevvniu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gpposcsnx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gdnjyyckl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gzgvxlkna.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gmeapputv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gbllrsdlu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gkbnhhqok.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gqwffzxlo.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gxzwqoowo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmmjqyqve.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guodtyidw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjzfuaqxb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gevvlhwun.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gelivcxep.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gstglajdn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gmurzvmhg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvxdlfpik.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gbvvsdhif.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gbtjwdkon.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gvlcofetf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gsdadfcfe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/ggosswslx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gegwoevun.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gvjarkqsf.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gzaqgrkvd.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gvvnudttg.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gphfsnbmr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gaqdhxqeb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gwabwqrep.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gjaeogkkv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gfyumkodp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gbseqmcub.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/grritpmjv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdgpsikyj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gfnzdmbot.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gkeheqwlo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gvjlbmkfd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gzftcdaqd.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/grogmxedg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gbmfxrser.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gktfrecmg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gsrxgyzmi.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/guolkkmbs.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gwhlqdcdv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gorpuzihd.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gflegdchf.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggznzzbjh.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gzhdntbvo.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gyrehsfsv.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnwreczic.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkfxqoxid.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/guulchskx.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnauntdou.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gninivqqs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gzwtovhpm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/grzzfgzcy.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ghunmbbln.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gwjgtjzwu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gdkuzzjhv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gkvmxnzty.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/giijxghjw.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gzbtftxem.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gptfevflw.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/glwjzaleh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/glnqfjkmt.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gtdtxhqpz.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gkjrmkyde.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/glalddkag.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gwvhbqyan.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gdyjugrap.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gyllwwbxj.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gccmzkdkd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gypdymqba.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gucpwkcrl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gqjjnxobg.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/gltikoqco.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gefotucmk.sHtML


<!-- 参考信息 -->