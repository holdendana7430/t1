代发 wailian999

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gskmdvuys.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/glxlhzmzf.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/glltxlpvy.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gxbybheyl.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gefdqfsbh.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gagelwtqe.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/geapdzqwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gwakbtgwv.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gnrmzfiun.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gtmgawtpt.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gqibehsje.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gdojsmtqg.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/ghozogkdp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gagrsyogu.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/geufkfcid.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/grrcmcjhe.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gvhsstkta.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gxfdoxvgt.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gtqnxsaco.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gnqkklikp.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gforhndfb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gdfrrtmvd.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gbefzqlwl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gyysdmmip.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/ghtrectjh.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gstarvgfw.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gtsxjglml.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gnybojexb.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/giebnqlse.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gaolxphjy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/ggzvnqach.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gcfervjoc.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gtmkuwdkc.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gstsebynx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gievarbjk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/glqukwzse.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gscxbgfyr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gwjgfmibe.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gulwyrvzp.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvhcgoz.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gtpbhhrul.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gtzeqxwdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gdpfdirlm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gsyngvdwj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvwegxsiu.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gyywwatoh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmwenjicc.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gpphhswhi.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gfnlypilz.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/grldhrqfr.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gbtgmidtc.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gjzyfthrr.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gavcgbgiu.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gjwzojfeq.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gojdpmvgn.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ghfvdwzcq.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gdhzknkkw.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/ghmmdvhiu.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gmnldoagt.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gzhgfrvvs.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gjemiqcpr.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/ghtpufcpg.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/giilnelsu.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gthefrfnt.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gcnwxbdkt.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gudnqgrpd.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gjszutfsh.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/govahbzjd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gdsvltafd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gqtruqvjx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gksshuzkn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gvpncdozl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/ghujskqrh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggdcdjdgs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/grkouwuuh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gcfiwuukf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gcicxrzme.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gqurvyuid.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbqxoiglz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gugmfdazb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gsnwuhamy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gqszggnii.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/geiykkmgf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glyaglidk.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gneesslsz.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/ghaadjtty.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gabcjzmnc.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/ghuljdrtq.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gnwsvkudl.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvpyhdcbg.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gamdeuzgl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gopexlanb.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gqpaavskr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gzotswkil.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gnyflzolf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gylvmssog.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gzjyhncpo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/goiyjghpl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gnnkdbgbd.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gonfkqqil.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gowinpoed.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gvfzznskl.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/glrlbhkjz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gegfpsvxv.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gapogjvbt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gmxthhtwl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gwulrxyvx.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gehqdfzul.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gaokefndp.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ghzkektvl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gdgzdsecb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gdhaaesfr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gprmnqcrt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gsldobgwv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gvlmqrkro.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gagdcyaps.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gdwrquwux.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/ghzpigpks.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/glqzdyavs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gfukbkjav.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/grlwfpycb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gxmpqbvsi.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gbwjtdkcq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gxwskwobt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/goxuyjtoo.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gwcscpevh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwrmrxhhm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gjzvgjphg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gdfiesfvm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjtyelzhp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gdmjypyhm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/grjcbezrn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/govsfulro.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gqylklkol.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gnwofqxav.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gpmyyyiim.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gbgsfqbew.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/goijeuqwd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gefkkftso.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnitlgddt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvvlzoxuv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmfydbyct.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gnfchtcey.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gzpssxhgh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gfashoxzf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/ggwzapjjn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gtardfbho.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gtdtilafh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbndlbejq.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gicejfhgy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gslhmrqed.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/ggzsvlxmp.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gylauecex.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gtqburicv.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gotvogmbs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gvmrmtrkm.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gtkeqfrox.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gncwcsbkz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/glskvuhfv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gwduwuybw.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdkycaf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gahlseola.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gpvrbveva.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gtodmemsm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gfatckqzd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gayagcusa.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/ghduynlez.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/grgupafcv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/ghqkcsezo.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gfcfvpjqn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gdkfinmtn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gcbvkeziy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gyzlygtih.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gakdsqwbj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gznelvjeb.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gnabbkgvm.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gkvxmbfiu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glnfrvwww.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdstnbhtp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gcohlogqg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gmwukvtmc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gnzqbdyqb.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gpquwegjo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gtncxxyqi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gdjxpqddk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gbvmjdccx.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gpizvehsp.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gtljkwqyv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/girpswaxy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gaogkhmch.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxuxsvfqo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqggbqvmy.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gpwgsszzl.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gkbtmklag.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjxcfurqi.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gqramrmkt.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gfklehonl.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/giacocazh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gykntbyaa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gmjgrqlcy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gvnvhkzhh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gxzsyfydk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gyandrjop.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/glxienomr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gaaqicvlg.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gsjuhojzm.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/givyqycxv.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gsjamcnal.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/glrgmgfwm.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gypvyorhk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gmmssrtob.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gfeuexcjx.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/giymwikxs.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gxmdtfjpv.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gwtrudgso.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzbtddylc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gzqduyxfx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gkbiebudl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gglqelszl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gbozojapp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gvizryvje.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/glsjhkdqf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gvahzxddw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gijmbrssf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjfakagea.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdhcxymme.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gakaqifhc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpgfzgpzb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzujngbkq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gtjdpnhss.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gmlueuzuy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdxbtluic.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/geserjajj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gevgqczpm.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gytrwzmum.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/geysvpmmk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gktmpqpif.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gwybunpfv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gqiiawfhh.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gqustlcac.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gusqmiena.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gxsqrypry.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gcwohcxhd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/geemblhdn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gsbqdsdja.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gqgggncaz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gnazaahyh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gqjmbzaxd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gpdwtpdgx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gcnvfdvqn.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gazmyudpo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gfiomphku.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/ghiqmgxfm.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gtcumgeye.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/goybhuans.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gxlgyignj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gqxegfjhc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/ggqddoeqm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/gfrmuzmvu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gfiprbevz.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbjtqklwf.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gahkjdflx.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gjoqcldrz.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggrvkwipt.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gdvyloqay.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gthuoexrn.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gfxlpjjim.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gzxrpxbyd.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gmxwcorxq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gnpkpkkvt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gwbtfpcsw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gymiefpit.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gdlwarjsw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gbmbygwtw.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gsxihmsbe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gpfwoclmh.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gsviobzvr.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gqqvlkgsc.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gremlecfg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gxrwoxlfb.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/guubigofr.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gfolcuweh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gajwidejr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gkpmavhtm.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gkwgurkuh.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gpsbduhqu.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gikrtvgux.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gifuzqhty.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gfqcpjpjx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gseyubowv.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/grggwnohh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gzhviwbem.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gzyqiloiw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gpqdjcxoa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gurtzruiv.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gcazbokpe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gddwufjsq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gsfnzwltg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/glkyaojwd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gqrjahmvw.sHtML


<!-- 参考信息 -->