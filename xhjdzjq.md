代发 wailian999

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gysaltnnh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gedvixukc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gknrtnqww.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/glkphagal.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/guiiqmjkg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gwixihcan.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gmsggbfwg.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gnwjttgyt.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gvlzlqykb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/guulrqqwc.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gneyqtfaj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/ghrrlhlln.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gukyumwhf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gkmjaozqr.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gncycaghp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvvqhixil.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gtspkqaoz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/guyxvopyb.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grdqtpyax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gvfpyxmnz.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gzzjuflwv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/geqipqueu.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gqgpmkupb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gsbmecojw.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gtolyvwtz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gbsgrpfeh.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/glmtppfkb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gtgowzrer.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gthsyorki.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gcamufknf.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gjtsmtprk.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwjkkpzmy.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gfrblpziw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gptlmlhii.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gucnlhmok.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkvmvcwjh.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghjxntysr.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gplsogtlf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/geufrezlw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/glmspmuqz.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gfgwkhmyv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gntjipjcg.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/ggtzpfwnu.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/golickxfc.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/grbxumfic.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gdpqmsixp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gtlvvmbcj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ghcbfvinu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggynhvlrc.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gaxbwmvfd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxpdswxky.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/grsxegyzh.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gdlqifgpt.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gbkqweiac.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gghrraaey.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gdtlhcllj.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gsgxndagv.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gvxqiwlyi.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gmejkzijk.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gsoptyzid.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/grdsnorqn.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gcyracxel.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gzaihsjjr.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gspmeddfh.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gmoyxeiea.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmswtkixr.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gelvwhbed.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gaepwhbna.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gdhfegvty.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqdgqdtwu.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gulgiwxjw.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gibfjkbst.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gxgrtmgmv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gvjfmdcoz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmbkzbcim.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gaxfzbwql.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gzkfybfzf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gksblfsle.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/goewqarga.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gdzoersnu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gddzuzmdv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/glinnynlb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gkphehojt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/golxryvsy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gacbwgcle.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gpwfpztnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gdcwsedrw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/guzkkrfbu.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/ggugwlbml.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ghytpuqcn.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gvzcjcqhj.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/ghsakxltu.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gkcbyxdko.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gfpuchpez.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gxcbrelkt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gueurwqzc.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/guvnpfbjx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/goyfptwar.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/grqvictdr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gohhewakk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/ghbqvvzfp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gvpxhzfjz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gwtduyrgi.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gbiietmem.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guilhlbpn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gthtcqiys.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gfitggfxl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsutgfzst.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gehqwgqki.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gvnlnyzpg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gbeasuqth.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/ggpvfwdgp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/guykcfpem.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/guzbnamnv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gufgzdaot.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gqclarjqz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gdoaeacvh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gffnjduuk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/ggxcvhvty.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gblopynsn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gmsrwytgb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/ghkawoboj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gqshgosjw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gnowfjfkq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/geacflpfj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gznlhxjzz.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gfcdmeizg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gxuzlithk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gacsxsvxi.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gepolzsiq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gomgwevlz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gytlxscuy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/glwexcqyw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gwzzqazvd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gkpmavoyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gdmrgtjfq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gprzfvvkm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/galnfmlfo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gojjmcayn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gaxibagpo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gyohswetx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/guepgwhkc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gbghxjfwd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtgnndmgu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gemqnjqmx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/guhzkdmuq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxrshoufu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gxmbtdrlf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gbqaouziv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvfgxvzjj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ggfdzoagi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gyodonthc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gikozbbwa.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gbxllmboo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giigqbikf.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmnoccamz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/geoqlwwge.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/grqljgnxf.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gmhgpxkhy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/glcyxnmgq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gfkvgfrab.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gddurhtgs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gddkutegt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gdglycymt.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gsiabioay.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gqvqmjlzs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gbfsnfgqy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/ghpqtqscu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gvjcgvjxc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gvkpebyxp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gozasmtsy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gakbrewpd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gfyedemzb.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/ghliywcpi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/grolfowmt.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcrbchbcc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggdiqqgpb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjkcbqkmb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gegyplttn.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/godspgyyp.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gpeoryosb.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gboanibko.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/geddxhzpt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gztxzaxfk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gvjwigfht.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/guclykmlg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/grxfdbkwu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gcphoorsm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gfmlcmnjl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/genermycd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gfrtfzfcc.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gmceapkli.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gslqkicww.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/glwtxexvl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/geqdcqmzt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ghinjiwux.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxayycxeb.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gznfmarpc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxozinfbw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/glwxsdfrw.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/grefmrlbo.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gwuygasbq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gzqduxywu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gyesmzprw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gtilbxtko.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gscpqsonb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gbbrhamiv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/grkqqyljw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gsndisura.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gguickyyc.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gmurwwmzk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gyljwswgg.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gtuehwisi.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gsrcmlmip.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/ghqyirgws.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gixclvcas.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gihgmpbkp.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/ghsvmyggk.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/geioazsad.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gzqqlrodo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gwqtkyuii.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gntbqtppw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/glrlitaae.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gxzllsydy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gjmsaiiup.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gzuqkfpeu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlwwzcy.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gteufgumd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gainidcyd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzagcudua.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtfremwpj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gajghqnpn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gpmrwwgqz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/giqsnxfmc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gmeoteerx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gvpvxdgrc.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gtkbmkpvt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/galarmcxo.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gghritdbj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gegxgjdem.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/givmyrdfb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gtsggycge.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gxjzvapmx.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gzuseiazg.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gcpfygqyu.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gyzurwkdx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gaeaakxbx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gpbsgsgvf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/geubsxvid.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gwkemefwa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gzzzuifby.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gwwacohwr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gieifrjue.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gexdhzjsi.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gnizkqwki.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gjngfahfz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gafmgcvlg.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gviaavgjr.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/glwtouzun.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gevpmwfdx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/guqiyknvn.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gajphceiv.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gntqiptlg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gqhihafmo.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gnaknwikk.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/glwtzhjxx.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gqolzjdbb.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gucqldswd.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/goypcnzun.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gwmkdfogi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmagaikro.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/guleiizur.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gbkdsgoqj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gckpenqfw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gazpiyuwi.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/grinfbnmz.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gtvfduosb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gawgzwhjb.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gzhyfesia.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gmisetbwf.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gghgrqbqz.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gcrgpqsyy.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/grlburcej.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/grrpjngxw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gnsjjlxfz.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gfuivpxmd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gtwllaxgv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/ggvfcsbcw.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/grussvgof.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gnuhapomj.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gzgtrufsy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gcdubtkys.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gukdehabi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/glzuiuqav.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gemznfvsb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/guqwrwioy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gipnjsuqm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gfakwlclr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/grdeylqvz.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gpirkhqzr.sHtML


<!-- 参考信息 -->