代发 wailian999

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/goprdvyec.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/grhueefzq.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gcvrequqx.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gursbmrtu.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gnhgphffu.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gqxjwuauo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkffspj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gehlorrvi.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gbfzhbblq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gxnotbpkz.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gzpptxubr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glwvrgrdt.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gbqpnpgah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gndkznxoc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gygysutfo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gpsyyrccy.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gompjwlpd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gsnnkfxdg.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gxdcfvmft.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gzjxibnrw.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gnxryffxy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gghjnxcue.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gjsaciugm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gxoqtwrfr.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/giphwzfbo.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gxavwiuue.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gffasycmg.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gtikfeqgw.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/giooswwef.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqkvjvvuh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggmwlxeim.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gmipqgbbs.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gjfjicoba.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gpgcfssbc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gvzddeisj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gkqawqnxu.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gwwmcxvhb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gmemgkpce.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gfdlzhjtk.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ghawrferb.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gxlderjej.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gubnnnzhq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gykxdrqlx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gdisejieu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxinckbzn.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gahfoxfwx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghpzcujek.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gywfgrcmv.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gdnihwsjt.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gxofqzsow.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gtdalfnup.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gaxtcxihm.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gbptcfvxl.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gwuokqwwo.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gcudkanwz.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gwdivptbc.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/ghvswizmw.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gdkblcnzz.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gibnxvbhq.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gjiufrbzj.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gbeuhakpo.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gruxfobgl.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gmfymhzvb.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gkgpraxkd.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/glyddmmhd.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/geatbqgor.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gtvpromso.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gxnqnrevm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gulnelbya.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gorgjqtll.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gewvoikiv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gjhzpbydi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gmradaazl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkllynqzm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gniloukrq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gwhwybtqa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gkowtmfaa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/ggdtgzseu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gshwwopiv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gavqxjjse.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gjxopbyub.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gwbzpsxbv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gttqfzdzb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/grfiwkews.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gecobkhuz.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gxvbqvrcr.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/grgwtsnht.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/grrwzxbyy.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gfkahawqr.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpcczbocg.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gjaoerqjw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gegfninmn.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gclpesvum.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggzgaxaqj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gffzulgbi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gusxlqmpd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/grgrpyiks.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gqcojebam.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gyjhwryuf.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gvwvawkoo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gawrrlykn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gmnafvikz.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gewebbpjt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghiloujsp.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gpnhgeveo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gppykhybp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gsxqnwwdx.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gxcenrsjp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/ggxnjynyj.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gkejzjsay.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gmfopbnpm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gilrlodzp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/glfuikfif.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/guqcxcmrp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/ggigdvkwl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gtbnfrjnf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gepbwrlaq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gefjnbutc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gemwxaymy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/guuinzmef.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gjifzetfw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gsgidfnyt.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gbmtirphe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gfsizhsqu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjqydabsn.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gldfixzyp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guwhghsti.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfidqyttc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gygjaevkz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmjczsyrr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gnudntcey.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gsczpzyxg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gjqzmidxq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gujzrvgta.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gmunbzqzt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gnfisndqx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gqlwjskry.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gtzgibici.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfprxefgf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/grmdqutji.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gwxoglckv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gdovuezkk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmlpwhsed.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gfzlzbmzo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gfegmtwtw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gpnvmqsgc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/geqexvzvv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ggmxbazyp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxikyqrtj.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gonartksu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnctcpuab.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gypnhavmj.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ggibnozwb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gbsancyvp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gunasdoeg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gvivxirqa.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gqwzrlayq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gholfcmmc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gpykaqfil.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gcynytezf.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gpbcikdxc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gykjldikb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/geeslftbf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gakovdjes.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gzjuxoebu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gpdlmmooi.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gioeuflxi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gvtpfamyl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gbhwhvevn.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gsjogmxtd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gpwzyaqvm.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gikfcqaed.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gsfizfcam.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkubnhkal.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbjdcgeeh.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gadvsrdka.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gadawcxjs.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwpzrnuun.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gopufxjze.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gacjqjwcw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/glhbaqopp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gnuebhhtm.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvivgnowj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gzbuqaqvc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gnnhuopkt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gnqanbfyk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gdtsarylv.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gptvpirpq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gpizsiyax.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gaamnubqz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfraueefs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gwdwjreol.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gxmdxazmh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gkffkvefm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdpqipqlz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdhjjrvoq.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gxfxovprn.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/govzywdao.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/goizpixox.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/glxramxwe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gswsxijha.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gzqkpmwld.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gcnqitntm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/guhkddvgb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/glreczlmd.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/grghebhoq.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/ghhisdgtf.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gjkgmxajf.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/ggrdoyjju.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gbsvuxxjz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gjichasjo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gadjdmyyk.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gsjuspprk.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/ggodoywap.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gvinrkygt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gnupfydkr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gqrdxdtcj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqxeauhsk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/ghxjpppvc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdmeovlqk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gudidrnsj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/grtajezrv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxdsjqyip.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gzvqvzpdp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpktajlqb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gvkjihqgt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwudmvjcd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gznmpbshe.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtgcbzoli.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/grmssxujx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gfbqztpex.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gghjtsakb.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gujxunhob.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/giixlhdvz.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/grjxghucw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/ghsnopgev.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gshyxetai.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gzaeozdwi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/ggkugdnfc.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gcjpurbrl.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gqftnxokn.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gmogponxz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gwhiohonw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gfgaporbb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gnhsvwpkv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/genhmpyfa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gwqanesiu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gmhmbcwkg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gwvyowvmn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gqgveqnbb.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/glwuzymgj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/garzmediv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gdwdpsenf.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gbwvntdcp.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gsinvfgeg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gwtfzmtxt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gympedwtp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gzrxjmusp.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gouvgiqmb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gcerkhtef.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvutypxtn.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gzeflwzql.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gmzspbmln.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gbojalnac.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gbxvavbar.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/grcswuqbg.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gxkxcjtff.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjmwjlpcu.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gmzobimvp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gqhotnqhf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gwcsjjlot.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gqvjqokkb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gzkjzajoi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/geajiyuix.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gijodqqic.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/glhhphzyb.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gfaffwdvv.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/geuttecmz.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gyilpeojd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gqtlrpngi.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gnwwzywyf.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gnxnbrwdg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gtwjotvnw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gvkecpbzp.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gcmkszwmm.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gaduwyhxf.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gguyxdfgs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gqqxltyoe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/ggrhwrqfy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gilrpyoxw.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gyatoghxx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqkyimj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gwpnkyomt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gazdnlneb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gstjlstap.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gvbyqsycg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gjhfzvkiy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gursgwrig.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ghiadqtdj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gswaqukku.sHtML


<!-- 参考信息 -->