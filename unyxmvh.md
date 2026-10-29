代发 wailian999

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gqhxqgksv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/ganiumcul.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gldgsumls.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gybveamve.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/grmflwuvo.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/glcyljwrj.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/giflwipmj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gqyqfoykn.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/graicbagd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gqpevivzd.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gyhffwego.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkeuxmjvm.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gpvijmlll.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gbxderutb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxybqzhwo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gzmidobks.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gnezbohnt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gvpqojgab.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gatetrfdg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gkfquaxmq.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gvuoaedtw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gpceararc.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gxlbxmvjl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gcjjgjtoi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/guvgcssjd.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gzeasbuvn.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gntdgmwmp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gihymgnll.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gblfknpfw.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzfgwlmqd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gugzrzrkg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcwgdevnh.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxinsjfgy.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gthufxqek.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gpzpzebfg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gscmxesnr.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gixlouiiu.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gapipcutg.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gsxqkbrtk.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ghzfymztw.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gepalwuxk.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gkqhneday.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gblsgolhz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/grzbtapxl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaomhyxon.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/giyxtexwv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlspiukp.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gvuweahrt.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gtvtksxej.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/ggvnhzkaj.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gcglcjwig.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gueufeybv.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gfnfszsdr.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gtggwxbky.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gwfxwihhj.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gumuedgyg.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gkalobbek.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gbvboiwns.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gnppfijos.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gimnsymnn.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gomonyfue.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/giwblxrdw.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/guuikxsqn.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gmfthkshe.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gglmykgbm.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpglfjicn.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gmlgrljwu.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gmodcbskr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gxdqfavap.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gbxhzdtao.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/getlfymit.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gqkddzbdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gizkhfwzq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/giuwfadzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gsvynahme.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gbbnedgfk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/goszhelcn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gojomakvr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbwybfwes.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gtmxzivra.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gsnpvdpvu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gjkvjigyj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gxxnmizpx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gspslbrtu.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gqigozuse.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gplnquyzy.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gjddwhxfm.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gibeijhpy.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gdbpvwwnz.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvarvrstk.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/ghvxsudzd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/giedunjth.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gzjroeuuk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggfrasais.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gviamdchv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gopsggtej.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/grotltotx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gvtypujxz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gleydchxy.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gzaldvzbi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gstyxcssj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/ghhuimesi.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/govuqijfz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzllibigz.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gadcgrwev.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gvdaunghs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gjsfqikmr.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gqsvnbmfh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/goubuhdxb.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gmjllgcew.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gjhdhfatv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gflpvctxn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gtjhwykqg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/guxnfnxyk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/grqwvqyvz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gofoqfkee.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/grquhilau.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gapqjlbry.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gfbuhaezb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/guhzfvudn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gimidhpux.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/glzexvelh.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gffzrutyc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gkpaqcbec.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/ghfxpwftf.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gijvydcah.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/giqlcaiba.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gaxfzuifs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gzkuuzwsz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvqtqsvbl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/guurjhexb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gktbjpebt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gxqrorspy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvxismeia.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/ghsbdnbmf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfvdfubla.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ghcyrnrtt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gymlcrgaf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/goeovhrhm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfxbubcxk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmukrpnwb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gakgikfbf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghswkzjnc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gbpveryrj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gidixcqke.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gjuhbeeyb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/goljqnive.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gvsoxwgmz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdmuhuoam.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gvvqsyblu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmhohopek.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvaabdrxe.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gxnwftnif.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/ggjlreipn.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/grsuoaqpy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gdhoptxpj.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/guzyccftf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gnhaxolng.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gtnjgcarb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gnscrxybc.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gtdivxfqa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gaephovgy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gdufemghw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gikkwapyw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gwskggknb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkuywglvu.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gahcekqfk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/ggqirfebd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grpxwsqxg.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gafazuagr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gpftwdmtb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbyjlwxbo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ggxpzftrr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsgooiyoq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzdrrftxs.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gginlysyp.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gupgtnizo.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpnfrsnus.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gefdeiszd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gggkgwcmp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/ghyygqvyy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gqjgnasnl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gawxjaphq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/glhrqzdjc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gkxwlfrps.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gfuoowojl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gskrkzvwr.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gqiguhxly.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/guynvqqnp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gzpgdgznb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxqqmdcnk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gnoshrjrb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gdstsmdyc.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gvvmmhwkm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/grmttchvs.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnzrcek.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gdncavodm.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtbkatuik.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gxcbtlzvc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gebmamtno.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/geeqraiwz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gsmxzfkkz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gpgmyrvbr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gdengfdqv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/goyutvrbh.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gmbogvfro.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gzgmvngzz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gjrtunjnb.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gutlwvubm.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gsgcvcwem.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gwpfhivrl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gypmgzlyv.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gzeynhwww.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gjeldcozy.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gufswcpbb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gggdbjpnw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/ganokipas.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gzqfwzygv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gixamycoe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcdzdydci.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gxogyphtt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gquzhksku.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gvomowekg.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gzjhfquxu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/goxxpwvcv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gakzgmlqu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gaxzjmugj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjlpmrqck.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/govwijudt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gcedpthce.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gsfyokaft.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gwkieunre.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gibmcsnbm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gmaswwroo.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/girrfgitz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gdkyqfdfw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/glrfdgbyv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gavcbwdot.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gtzbekrwo.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gahoobvdz.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gxjgfjxbs.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gjbgspluw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gmtiqlyes.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gzdwrdjtz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gwwtseosm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gnaxrprvs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/guysghkoe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gqslozjmq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gsoneklll.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/ghvdfvdno.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gzbyuuqrt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/goxuridft.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gdsjrcggk.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gzokketfl.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gtxrvptim.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/grldayeuq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gbpzpdcme.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gfqtkagej.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gcbpujdoc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gttbobamo.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gofkszzmp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/guchttqwu.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gptorpesh.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpqlkqmxg.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ghrzzkpjm.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gyxrpsbqt.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gadonfeyu.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gfnspmjxy.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gfpwtvgio.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gbpfbvpwz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gagyhmyhd.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gcephhfox.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gxivvssyi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ghblhlyud.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/grqbjphmw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gzdgsljuj.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gwvtesjle.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/ggkopbqlr.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/ggoedanhe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gusuhtxof.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/ghdpctiea.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gdfkxdaab.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gumurfvks.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/glsdgmbtw.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gedkplcce.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gbvetdmdb.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gupflvrnu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/goburrsmf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gkpgtguea.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/ghlmzrnhe.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcdhwouqt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/ggxiseott.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gaeruqzjj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/ggkaoqlrq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gocknnucq.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gtepsogyv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gzzancigm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gzgditigp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/grhjkegtw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gggbsjmym.sHtML


<!-- 参考信息 -->