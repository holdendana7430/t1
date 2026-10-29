代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxeqvtmpv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gsufgbqfz.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/glfgnprwi.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkixlyxho.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gjxiizyhs.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gviybuuhq.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gjjyvtgnk.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gprfaonvc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gobaraqev.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gzaoxagzm.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/goonnqsvw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/geblxrwss.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gqzypmxnp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gcgwslbct.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gjzbqyftj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gmxseaohq.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gjobymivw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/ggthqwcdj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gbhaoacfl.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gbgsdixfy.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gyiujewvi.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gipiowmqn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gtqvxqkcz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gmglclgyj.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gjphwhgsf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gbxzrvjse.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gvggmzigw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbnbmdngl.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gzrmwpxoz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggudlcuxi.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gpylkwlzs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gskftneyl.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/glhusutwc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gbcmuzcro.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbmddeiws.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gjmzgejxx.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gioiqvbeb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gujshuuzl.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gtfhjnooh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/ghqcrrxpw.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gkhawvfrb.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gbpxmbkeh.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gdudcnbht.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmcbcqdlt.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gnhlinmmz.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcmmbcsi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gxyqjnwju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/geigmhprh.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gsbqpqaho.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gshktvhjj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gwvvhixww.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gnvrcgffb.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/givbflgce.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gfuvlcuyi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gqdtsaels.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gprxfennw.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gricighae.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/ghxyvtbdd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gjawfwipd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gomyhqvbo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gekrwhmgb.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/guddgyulb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcyfzqofe.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/grqaeanox.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/glmpdplmk.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gryeanjtv.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gsudfvboo.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gvqqvfmkl.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gvgbgnjnp.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcyfvfxqv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gnsfgelgc.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/geynwhsgo.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gdkffnhvh.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/ggpwbsqqr.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/giszemnqz.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gxatfjwat.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gfewwcgmr.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gwnmlfxgf.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gogxgjvau.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gqympsbng.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gihwjdodq.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/guxitcjpy.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gunbhwidr.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gwzexamhd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gkvzsloqp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjlcsgkvw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gaprflkap.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gngjxjgix.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gmzgyoclx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gletfvshd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gwxtenluk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/glvyyfdeu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gccmgiazv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gftvknbci.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwofwosgv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gsajwzpop.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/grzdtlfss.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggetosree.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gcqdefqet.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjkufkwgd.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gveqwuysg.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gflgrcsty.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/ghjmbriws.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/glzvkjchn.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gjggtyvrb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/giplocljr.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gwagiafki.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gpuhadaug.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gzbmewgdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gtvdkeldw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gbkfwaimm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/guxdtigrj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gexuiioji.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/grfsjivwu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gwxyrfpjj.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gzqcubvay.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glplarymj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/glgwojpdo.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gpwnxehja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gohzcikhg.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gheriydbh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gqckhhkoq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gexdbicqt.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/grbhntlhc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gkcpcdqao.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gtuwgjgkg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gmcxmmedt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/ggkuuhori.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gjhzjqnga.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gqdieatam.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gsvzlwuby.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gmeizkldu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gnsdfnrwp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gubjmqcbn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gfixtskap.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/giyldfztc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/ghdfekujm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gdfefadvn.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gummfiwvz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gvgwscxca.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gylmsnxiu.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/ggcddglto.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqlhchzqp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnaratjfa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzfccan.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwemzamdo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gfhqdmwkn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gwxrvecrg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gaicdgabd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbyhxburh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gckbtzzoq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvxxatqta.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gvinfhgcl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gimuqksko.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gwdfeeifu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnadvxjou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glfpzpcds.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gqrdmyzff.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gobohqiuf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/guighfexc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gcfxukkgv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gxpvfkjki.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfjhoipvn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gpxqucyee.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtznazmtp.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/grqbzymac.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvxywshmg.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/glzulxfls.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/guddhcllj.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gnxzaptnw.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gnwmjtsmp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/ghpwjyqjc.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gcyifgwbp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gjcvyylfz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gdagioili.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/grczcpevt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gglwtnypu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gxdzifyzf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gqkhdrfgn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gancexmms.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gocaoeswf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gzznurbhv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gzbceyumv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gujpejkwh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gznnguxps.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gxlcqdked.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gowlonqcq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glaydjtwe.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gstwvnwra.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqbhgwzpg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/golrliaxq.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/ghezqltxw.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gjayoptgp.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpicafszk.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gbczfsvbr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gitbnetae.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gnnauprfp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gzgiyzqbp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gpdhveddh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gfqpjjxoh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gtcgmlfjq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/guxuqcdzj.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gshhtqttl.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gsyfzfrtq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gzktjhniu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gshavrfet.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gslrvttcz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gyuywhaui.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gtesdjiyl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gkxhfyuhp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gfypelbaw.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/glkzamrzh.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/grwptbiwt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gdtapkiys.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gsamchapv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gvuelduup.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gtskhkjcw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/goivypuqy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gfqywzdkq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gjufqjdlo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/goqiqherd.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gmefsstat.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gokqugszh.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gggjubwgo.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/grmynobeu.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/guxaexbvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gfsekiqcx.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gmqaftpwi.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gjlgzozls.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gynicamxa.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gbjkwrntk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gpxbiuklm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gvekvjaaq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gnrnftfsl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gsxjjzrrk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdpconozg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gjywtbowz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/ggsgfupef.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gpbqzuysh.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gnfdehoyf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gosbyvsxw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ghioowrmb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/groxtrbaq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gimwybdzl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gdyxychfb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gddlppprr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gjpcqhsnq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gbknxkqjg.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gvpwadlkc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gzsbiwwlu.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/glisxijym.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gfgsxlyis.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gkeosngbn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gkvntxvih.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gvrspzaby.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/greljmbjx.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/ggiprxjfp.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gzevwjfgi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gynyaeawd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/grmjtclkv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/ghojbenof.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gngvjdgsr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/ghifrwtsh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gzrhdklho.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gbjxvmril.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gjijnredq.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gkjqxfqwl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gurbtebsb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gzzjaqrre.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gcpxgivwg.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/ghqnhuiug.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gkkzobcph.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gzbmhyqpl.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gktgnzesd.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gngvzwqte.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gzpdqvbdm.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjpmjec.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/ggmvtwmeh.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/guitjubtn.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gxbsiooms.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/glclhkuqs.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gkneonbwk.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghwvxlkpj.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gudrpxrul.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gacuiqwwj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gtjatakvk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gepgazntb.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gyfbgacqa.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gwcqqcdss.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gbzeyemwa.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/galtjwtdf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gtjfaimlq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gqsruccof.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gfufwgpsn.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gdpqnlqha.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gxqmqnaxi.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/grvhhpzld.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gqqnwvkrk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gwpivmkqg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gncqlqgtw.sHtML


<!-- 参考信息 -->