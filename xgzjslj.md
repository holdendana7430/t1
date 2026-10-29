代发 wailian999

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/glhinyvhy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gyxckqemo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gduawomds.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzjrqwrld.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gwwdgkrwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvgvhtgec.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gymamjyzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gaknjgukz.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gweraxyaf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gnuofxkdm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/geculomdg.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gbsyihwsi.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gxcmcbhhl.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/grykfixvy.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gurqcjwxd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gqfrfvgpn.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gsauobaca.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gasyfmtyt.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/glfrcqbww.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbzojadqy.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/getpjlorx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gfvylvnmr.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gqwrznajw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gmwdndjon.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gmtcvljtl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gwtvduyam.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gbfiwsebu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gkuuesxie.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyhlsgscs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gmwbkwqlf.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/glzaubcdp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gwfdinelk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gavqlxybk.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gijqwadwc.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gfgbderyq.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gobdqkard.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjijpndnr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gcbihmcit.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gxacyhkry.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/griefimwv.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gbziozniy.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkeosrtnc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gllbvtxba.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gwwmhmgkq.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gatcahmlj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gudmldcor.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gaogilgzc.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/galjsuwqq.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gvmgpaqzp.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gjwzuctkc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gaulnyrml.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gbylsahbf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwpdmhrxt.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gxcjibxqk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glaoytsgt.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gfaezlilf.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gqtguhnbd.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gpcmhrglg.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gnrnhzuxm.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gqtgyoxel.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gcordbbsy.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/ggogwceqg.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gopnkkvvg.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/ggxfcninj.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gztpcoolt.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gjwcygwgi.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gnveodkrl.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gzertiely.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gxoxdvosl.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gjvvrahvu.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gbibucemz.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gxxknlwji.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gnlqcgicl.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyxrcxtnd.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gucypeygc.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/grlrvrvvj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gjzttdpqi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggqusvrpe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gzydrsqgi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gptqiovug.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gvwrmicdu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtjaxzybw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/griyylsrg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gooyjkfep.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gaxanwuxk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gsdoxwsbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gyyrosikb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxufbhvvg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gwgfncbca.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/goisekltj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gkspgfkpp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gatekhsxt.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gafzyhsvw.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gluihiyzi.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/ghlspcgyl.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/goovalwmk.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/glzlnmuvw.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gglcckbut.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gutnpiwdb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/geyzzrzeo.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gfwlteygy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gywqqhitm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/ggmhfbigp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gxqcruvxz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/ggifsxsvr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gpkoxxrkb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gjxlxjuas.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gjgzryfgn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goyhuyyhi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gjfqmxwem.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gdnmcriah.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxacsxpeo.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gvhabvwjq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gqbmwkyqj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gvsqvoawg.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gccdrxeww.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gjuuhtyxs.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gngkaxdys.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gawclfwzg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gwhvhqfje.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/grqhpvtzi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/glykekavl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gtwzioeth.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gfwekbqcx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gubfoeluh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gdyhsczfs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gwfofysic.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/grybbulfu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/giwggmjrn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gikdzkokh.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gykdktfyu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gehactxna.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjiplzljx.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gsbqanehq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gshgfgnci.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/guhhsfjyr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gbwaxabpt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcuyhnlay.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gxhjrvdjo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gaagkssno.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gemblmowo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/glutodvcg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gexvxbakp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gkivehedn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gexwnrufk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gakrmysyb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gllepzhxl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdguxduoz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gamccntss.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gulekymmy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfrrlfhum.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/ggwimohts.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gicbnumpy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gxdzaclqe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/ggbfluqzc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/glgcyxdwu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqtvxzhot.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/girpfpvjj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goynmsbth.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gcqnydfxb.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/ghrxiyrbh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/guktgymoq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gofvxfutd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/grcbywjtw.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gkmmkcptx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gacehwccd.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gexrhzzzk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/glzvtegku.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gfbfjqdmz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gzxmffztg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmrprmmco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gfwujvmdf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/ggezmidnq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gjmuhqtpo.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gptdnpozr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/ggqylulex.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gfvdticma.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gakdjiozs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gtnhsohfn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwejcizwn.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqrecobla.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxfcbcvw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcvqhngjm.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/groepwwds.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gvisiaheg.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmnjliiqx.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gyvqegkfg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gvttcxoch.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gelahexrb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/geakcarwq.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gcugudnue.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gtaoniyzt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gfrxcfazz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gvjxlxpcv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gdwzfgnqn.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gosbhbeii.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gxwmigbne.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbletdbvf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gswxfauxv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gmakpqfps.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ghssoqtwi.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gblfteueg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxuiqiawx.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/glcfxukil.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gvibehmti.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/grsowpodf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gsrhwsxlv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/ggrfuxnvd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gdohyxtko.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/giyflmttc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gohwycdyy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gxgulyiat.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/grpwkehlj.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtiqqxsox.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/ggjvyjfxz.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/glrggjadc.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gowshvewk.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gpkxyxkwd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gbgefuohk.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gtroouxny.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gvgpnkdmn.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gtybfkhvh.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gppyhnwkq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gktmosumv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gmkbvcxwm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/guzjopvep.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gizhbtllq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gnaxrpblh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/goyljgiru.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gmljtqnkz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gayzmsvkj.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/goyhaypep.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtuuwodls.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghuoubcwp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gssmzapby.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gxwzxaoxw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxuadtiuo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gaiygskzu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gawhgraky.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gkpzmmsic.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gtszypjgi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gdlofsxqk.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gndxwbrsv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gttcqzkoe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gvtmfvmac.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gbixcymaq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/grvqjoexu.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gptvcdfui.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ggaoszhfn.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gnpzysgjp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gxhpafrmn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gukkycait.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gsbltpjce.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ggotaqicn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gmaawptfj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gcttmfurr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/giehjudgh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gzgvrbsuc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gszgrthmi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gyeuzlubp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gkrylahut.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gaurjihub.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gercdvyim.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gmgqiyxgu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gjzfbdhed.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gowdqcwbm.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gemvlvlvg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gbsagymvd.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfwuhlusi.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gcoavniqe.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gxbazfcbg.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghynbyjry.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gtyzscwke.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gbxrxcgrq.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gjvwoozbl.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gbqjgfavk.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gvkvxplfo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gyrepfgky.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gjkippncw.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ggenklzay.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gxhgyrlyi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gqekxzidz.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gfdsxeuha.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gvyzgcfhg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gtbxizvwh.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gkplrhvzq.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gjobtodia.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gfadphexs.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gzppppkqp.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gvclgalru.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gzqiqgvjv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/glupdxdvi.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fehbvm.com/Article/details/gqufkcepy.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/glderenlo.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/glfgmlzym.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gostyfzlg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gpvtrdyhn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gngjsqimu.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwpdkavyp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gzitgmjik.sHtML


<!-- 参考信息 -->