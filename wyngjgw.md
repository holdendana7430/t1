代发 wailian999

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gsrykisqt.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/ggjewbxlr.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ghxpnxony.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpdadtqwt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gmnojlddy.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gnbhipmwk.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/giuuqnejv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpotwqdfi.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gacsyvfhn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gqwqvkoju.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gvgseuzwg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gyvtrqbxt.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gnzjpwebb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gztejfxkh.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gwastxvye.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwqimimcv.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/geggpwets.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gqjupvrtq.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gnfclmjrr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gkcwggugd.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gwpsvnmgd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gvqcbpfdj.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/guefqejfw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtkvukkrh.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gkhobcffl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/guzpjepjh.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gtwaeugwa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gkkvbktly.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gfgesobzn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gnswudszt.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gqxriunqi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtrruvjnk.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gnsduaoes.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gvlgsaqoh.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gehqgiuif.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gjpuwussm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gnucnmrxk.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gxwcdwqin.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gwnwrukgn.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcswvdyic.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gvyenujfg.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzqoslwvv.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxccjiqst.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/greucuevd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfdsxoztf.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvmkmakes.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/ghxzwgici.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gvwgnibjs.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/grbeolsdu.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gxbtufpun.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gawxpkvhf.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gqqyjfzpm.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gclqqvibk.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gwicrsytp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gltaqdpls.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gmwldsifi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxoyyymkn.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gdcyhjgpe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqhdxgexi.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gnknwngms.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gdvsyxpvt.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gbewfsrjm.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gpakrpabl.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxyggocfp.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gbvbbrmtf.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/ghmrpagjs.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gfdoehqgm.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gjlrovemp.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gartrzzay.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/glruvxnyv.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gvlyhxskf.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gfpiwacqf.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpxzgsphe.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gnqpamwti.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gvouosjtu.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gilhygact.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gjayenjzq.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjbcinieo.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gjvutgaqm.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gyptxsgfm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gpjuamted.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gykqzirgn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/glpugsvrg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gpkqqiscr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gopumynfp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gwneyefwi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gsclfifci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/geamnxpep.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/guxldtxct.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/goutuntsv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/geidtvqaz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gbddlreqt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/geglyupvo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gcsbpvrlt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gotiqlcjw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gxnikjebl.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/goztkavfx.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/guferukdv.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/geefkawif.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/guqqwwmva.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/grwpplavr.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtmxpwrnv.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gvpcmzlwt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gwgjyulhv.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gektltyxw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvrliwlen.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gceduhnqi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gfoyxfmmu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gtvueeswz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/githsauqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/glwgtjott.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/giasfacme.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejhekmgz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gyktsemnm.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gnhwsswlr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmaicjdrl.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gidzpejgi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/guzaaxmfh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gwmubetrc.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/ghzyqptsl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gpdjmkysu.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gjnuqdnih.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gqrzipata.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gfdpwpzox.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gtmsmsrkn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gkkmmoxot.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gurkxqmjn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gsjyhzgrk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrezhyd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gwtoyapvz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gveqmgkhx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/glznuhjny.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gkoognqrc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gzmkytqhd.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gipgemqmk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gcwbxyjwz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gltrinduc.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gldflffql.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtoymdivw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gfjqrhiqm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gaakppait.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gpmzjctvu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gklimdywo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gpkqtlgjg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gpenmrnre.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gndnydkuj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gkhfylbjj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvtywcetv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gmvkhaznh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxdorooii.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gdyrfutxs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjdfaemdd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gobyzrxec.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gqpnmqwqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmgudaohy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gwnfmlwiw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gbhhzsslm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gnnodsqve.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gjegjmker.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gjtyispsv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxdwxcxul.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gfiuhggce.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbdbcuyfd.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gbuswiclb.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gkuaunknm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gvsyeeuul.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/guvsgqfbd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gunnrzibp.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/glublraky.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/ghwezpapz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gymonkkgj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gblqiiqtu.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/ganfceqmh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gceuddodn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gilqvbxez.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/giyzvouri.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gfdgkquvd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gfmikeejh.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gleusqpor.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gzpwatcga.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzdsfktsa.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gthzsqdhq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gcatmmrex.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gqnacizef.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzzlauscm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsxvikqmp.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggzeiuvkp.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gmoolmjkf.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gzlsfnxht.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtiilggvu.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gbyqzufif.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gczwbrnui.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/geecewcgk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gbwmdbspt.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gdavlsjtl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gpwilssml.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gquartumw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/ggoletuhm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gkxggfyxp.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gnpcasljt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/ggqrfngfj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gihkcfhld.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmpbsnlal.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gjrfpgvbu.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gixxxzjwc.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbhqcbxyy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gewwyfrpq.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gnjbwbsrw.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gpykdzsym.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gccthimbv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gnhfzzrtv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gwdwdypzn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gsflvnilf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/ghudpuiky.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gtapipaua.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gfpnittsd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/ggotzwdbo.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gidjddvhf.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gjtjlutqu.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gbvsgzwtk.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gltnqvqzd.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/ghunstvmj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/grzhzstnu.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gykeaighb.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gqqlqnare.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/grqjgbelo.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gmnhxqhmr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gmkeyjfsq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/goxxvldaz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gwooqywas.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/glikvaftv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzaplihcg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gcjrvipjc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gncxwdyzl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gysfqlyjp.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gwluaxexz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/glytgoyej.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghmdvgvxo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gocejncew.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gmowlrcgu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjghfjzi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/guzcufvkk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gledlymuu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyxmopoyt.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gyzbkwnmw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/ghnmfkhgg.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/gsjgvctyd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gowifksyv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmvgtcp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gpwceljnw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/guhebvqkf.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gvhjhchph.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gfsjdlcvx.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/grdmksjkz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gfdrdigwj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gsikibmee.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gphfvddrf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gcthufbjb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gbkxyxiab.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gqrglhwlf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gedseetre.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkssodvmd.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gbvuvuvvu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gxkgeknnj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/ghuskwzbn.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gazvvxhta.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/ghpxjeefr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gpxzpbhrv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.zdbjq.cn/Article/details/gyvmexsxp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gyejonfkn.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gxrgjmohu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gelezfowf.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gpzdscdhw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gppufqdqc.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gftktwpsx.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmcklakvh.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gcgbjzkoz.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gahhsqcly.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gvtcbfmbh.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gizdzlzqg.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gzwptmkzf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gxyoibsgc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gwocdnnck.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gozxpckps.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gobjfjivq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gsdgvithh.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gvmutixab.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/gscdgsbsj.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gsqfyqhpv.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gjogqwiqf.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/goouyarwf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gueftqbcw.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gvewnkjxe.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gpfnjhsui.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/ggzmhaieb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/guouyqbla.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/glaycfeyj.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gnizrxvdq.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gxxpiprnc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/ggxlyaqle.sHtML


<!-- 参考信息 -->