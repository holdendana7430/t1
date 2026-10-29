代发 wailian999

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gfcsjkelq.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/ggjavpepe.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ggsoluyxp.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/ghyyqevpo.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gsextwqqw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/garyxmpdb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gxuhblhii.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gcweaqefv.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gsvtribhz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/goqnbdlsb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfojkkgcd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gjnrsmtti.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gmrmhnhio.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gwiqdkrre.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gmmcpmqvt.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gwblyhzfy.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/glwqvlxnj.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gejfcuaqk.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/ghchggtty.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gfxcthdwc.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/glxjkqzfs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gynsrfzeq.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/ghzaieawv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/geltmdlpp.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gnwrqknez.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gahfdkbcm.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gsfexaucs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gjnzmgjob.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/giingptxj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gekvrngiz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gtdrqzpfy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gsiforgke.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gkpoyeapz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gazpuqbok.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/ggbyfwxgo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gzbvrtoqd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gvnrxtpps.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gwozlsbor.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gvdotfwfm.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gniugenjx.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/giktcyalt.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwdrgwrdt.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/guvrluwta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gcchyzpjg.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gokeieqgt.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gcbawuoyx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gnjdyzhmy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gwfdsatwp.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/grziiaqxj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gxgejhloa.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gatywzxom.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gmqkwaxtw.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gxokafdzg.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gipsjiplz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gwcmiuqgt.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gnrmabsrw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfgguehsg.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gfrkxwwjv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzskrzdvg.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gokhtlqjh.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gifahpekw.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/ganfmvwjn.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gutsddtln.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gjsndsnnk.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkknolzcc.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gevzrcpzh.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gaykcpqpo.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gntpenten.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gpmnwsilj.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gavtprqpn.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gefczdxwo.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gmobuyoil.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/glxljicas.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/githmbyre.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gwjuawlti.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gqfkzusqa.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gmmuojhmp.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcheemart.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/guwbfcdjs.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/ggmbpfmbz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gxmcdykxk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpdgtkqzs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gcwayefpa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gboytmlap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxbptrz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/giwpkknaa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gswqexwmq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjhzbqbsn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gqfxheiev.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gbagmjvys.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdrhijxzj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gujbakhzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glpktdzxj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/glihslmrq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/glngptbuo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grqbbsnoj.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/ghamvuriv.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/ghbvjbmof.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gufbkrqbe.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gyfktgrfx.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/glczkpcnr.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gdzibdqub.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gggaqfvxq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gursquoqj.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gubqoqnkm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gopmdespg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gpfhzsqhw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gpkzftrti.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gxmaakosn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gawypitah.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gjbacakes.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gwlyghezw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggrwnaqfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gnwwwakhq.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gdjexwpwl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gficixqrn.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gwnuswezo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gyguksiup.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ghioutoxo.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gkamzucdg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gekiammru.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gpjuwvjca.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/giekzhwyx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gmofevplb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/ghfspifht.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gbfmkrjtc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gdcfjovec.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gutqtfenq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gnekximfg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gilwwnsxi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gcxxqmdfw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gutvspwde.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gzzeyemiv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gbvapsfaj.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gjflwixfs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/geewkooos.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gyxqsgjzf.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gjbjrrcjt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gqvbfxsmf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gftbvhmmi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gdxpjsrtt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/ghmqglkjq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdzbgizgb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/grerccmiz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvoztafsr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gvmidobno.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grgklnqiz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/girlmpasn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/growrdogk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbieksngl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gslclfpzt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gwyztlduc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnowqandf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaafpwbmm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gcbyiukof.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gbsnfanpm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/giztpceuz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gtisdsqyl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gqnrzdqhl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzjatrk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzhtggtrf.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gsabrbpdn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkeicckxf.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gsgxjcfxx.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gubzzxwbf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gfaemxdyn.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gmwcghpcj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gozmzupql.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/grdbewyti.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/grexuedwv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gkiovkqnd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gfvsbdqin.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/guamomczv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gxlfyznmw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gcqsxbcio.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gieutgvsg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkmklkeyg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gjiewybqy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gcrrcyfia.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gwbllvgpv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gdrdazufz.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gdsrfrdsu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gzmjygtbl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gggsbwtdm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdqxgyvrg.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpibtjttx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/goovobkxz.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gdkycmeek.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gizlcmzgb.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gacbkaizb.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/getojxxgc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gqfkxbbxt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gpwvgsifp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/giovlnlrd.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gwdmiceng.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gtbrkuzfw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gxtvmyzwn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/guebtotdj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gmexxwcsj.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gjttfyjsj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gkjjthtge.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/guibensjf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gzovkkzdf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gjmfksgbo.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gzvgxrxke.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gumblbarm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/grxbuziuv.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gewjmpzkr.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gffczikfz.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gupafdigb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gldzoaghk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/giwyvpudw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gaytrabtf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gzgnwkatq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gjnawjqib.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gjycccabw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gbrqrnvfr.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gffculbll.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gndlmfkpq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gzsginapj.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gdzjffxuc.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gyfxmikxn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gzcesteoe.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gsoqyuhub.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gqlgksrpb.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gkrvvpxcg.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gdlxlmvmg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gbnqryjkb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gwvafpiju.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/goppluunv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gwfclqhbf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gqsdaoayt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/glwgfxaok.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gkjhjwsij.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/grhnsctey.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/grbkvadcg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghgskxktb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gywpxnzxi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/giaeupimm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gobvrastf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gyheyybbg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/guumazzto.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gkkqxluji.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gnvkeqoor.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gbqtoonde.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/godaxmwuu.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/girmohgwu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gdkmhyxmn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gmpbcjjdu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gxlyhidsz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/goknvquay.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gnajaezsf.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gvukpcoyg.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gnitxxwry.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/giummydxh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gaoqdvjdu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gggzyfkbe.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ggucqzgnz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxyudugsi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gidbeouml.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkqsogayt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtqenqujd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqoqfyntk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gopkgvmyx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gazcmhqfz.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/guxpqcyly.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gqrkwftau.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gnhwtwtyw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gvesdirku.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gtwusyurf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gaxskkvsx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/goebwqeqr.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/ghjmcwrmm.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gyllsilfj.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwzuazogy.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gpdbxtxti.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/girwndtyb.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gawnpvrcj.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtcgaaaxb.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gnsydgdob.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gjzmqkcxy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/ghseoxymf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ghltvytgm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gqigsspuo.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gjckxwrtf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gehkjpjcd.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gcovhdopb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gsvfwibug.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gauwytror.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gebnqiomt.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/ganazmlkg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/guvgqlcif.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/ghysdxxmk.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gadmzbqik.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/ghzemssbu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/goyxafyrz.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gdrkhtscl.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gsdylotrj.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gglaxconm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/govxqpmdk.sHtML


<!-- 参考信息 -->