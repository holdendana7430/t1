代发 wailian999

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gbbsyqfng.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gtanvhbbb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/ggrwhgowb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmnqnabee.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gxuvnlmci.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gojdujnaa.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/githbsybh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/glxlmccpm.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gahtkbdse.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gdrqlvqol.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gvqnvbchg.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gdwycowva.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/garoqlqbb.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gstkcackz.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gzqyblcfz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gjzgpkxvj.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gcjwacqdo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gxpewjxqs.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gpsdwiurw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gadabteif.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/ghmuuddwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gmwugqlij.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggugjuplp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gjvygjhgy.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gwrcqnhwq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gwucyikad.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gfuqgsktj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gtrngivqk.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gnxpdmnah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gozhlnheu.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gsyzwauxh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gkebjlcwj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtfwbjpbp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gsipikmmq.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gojtzgogc.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gulqcojlx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/grrsryhek.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdgdgezbc.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gvltygufg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ghtrrcvva.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gbnlhnegj.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gyvlweghs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/ginlcgefi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gunjpkvln.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gvorcqyyb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gjjtyunun.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gwhsmrujk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gzaqwkbjl.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gygspzykk.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gsghegbuo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gijvfjusl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gprwspxns.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpwzujblv.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/goqfpyduf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcocabbgu.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gbjhmogsj.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gfydqgzox.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/geidtukly.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gksorkdgs.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtjpyvtfg.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gzcxofydb.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gzxyesyuv.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkeubzrfy.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gpffyqtoc.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gprixmsml.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gqyufpmho.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/galuidjgx.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gyyqusgat.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gnqupeqtq.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gsirmhrhe.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gmtiwyipo.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gyybfufse.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gfujpnqii.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gyzeoxhub.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/grmjwzehp.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gpupdfdae.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gbsdjiknv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gaeosgvtz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdxpvffiv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gdubitoqr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/giigqjdiq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gdzddjgrq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gqbxbltar.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gbwqgmiwc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glltqsuow.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gwzgwvqrd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/guuonuyvh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/geqioeqhe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/goftrxgwl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ganoqknxo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gvnvomsrf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdrhoktqw.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/glffcziam.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gcixxdpbn.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gujggtlfn.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gajopsddr.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gnpumslet.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpaaprrnm.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gxvfmvbee.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gljulzkha.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gnehzumeh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grqggoptr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/ghljdmtpn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gjvqvlibw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/galvfnxbm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gwseguvfx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbughsxre.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gdrgthrky.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdrmcsaty.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gojchsfyj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gbnuqygrr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvznqgmyp.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gebayikio.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gghsfplmu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gozhtsgdw.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gyziyjtxk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/ggyxnbmak.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/ghnkjsztf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/grmegdkcz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gteoezyac.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gcmzkgtjr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gbqbpqter.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gcpribicc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gspbbvtud.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gqwetipmn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gfaroazxe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gaekctjdi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gvpyjvbys.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/grwdxbtyh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gjmueksxc.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gitkikpsw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/guhhnpzxi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gkiofkhyb.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gfkgfrtrj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxfavfdev.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gcuejlwny.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gposnzzvp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gkjolztwy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gwyxysgys.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gjbpvpsij.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gfcstlvha.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gngaxnvps.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gjrndtyox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gutqyvzya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gbozbmswz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrizgtp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvqzvnsfn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfomlsycs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gxjnmmjxb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gqwimyzww.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/geyhhaits.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/grgqqigqw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gzwwbwdud.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gqycekgom.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gkmbdnyeq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gvfiwguxs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwhptsvfm.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gjyxnfqyv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gktoraoxg.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gvrphxjrf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gtcrpoodp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gojawxwmw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gfpawsphb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/goilqcdid.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/guqmczdab.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gjnxllvmm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gtzertcjv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gsjefgnfi.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gmoilbrdo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gqzezkxqi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gchhljzch.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/glfjigbwb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/ggtzisohp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfbctulgo.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gtoisjnuz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gdtsfsvyh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gxgyxswer.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gdyfiolgs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/ggdrbudvn.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gujmzbejf.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grtvyvulk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmqhxghpk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gprfcojmm.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gcjpnuoou.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gkpowtrlf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkwgsmlum.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gqxavpecc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gqedfvbac.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gmimdbrac.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gctkxvbfr.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gjgxinrvy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/grkfieprw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gjegwoiiz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gdxtmhiuj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gbgctbduh.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gfhpwofuf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gmmmgkhud.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gwcjjuncu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/glooxklcr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqsaxecha.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gelbylbmp.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gqgjgvmzk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdagydwma.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gizbqktto.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gmbfbmhye.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gfpoldoyu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/ghhuqemhv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gcjkngysq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gfemrlpkc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gmrguscyo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gfqqpcvlh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/grwzoekvu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gmrgunxku.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvzpyfzav.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/ghgnysgux.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gycazooih.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggrjhggnn.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gfiaiwxyu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gbndarnjv.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gbpsgwmlb.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/glxlegady.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gjzmxeosq.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gyszksoxj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gcjhnwyvj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gepggeyhh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gktpjjijl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gufrtamog.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gchezwpea.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ghsswukwh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gomxjeedi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gdedyaczf.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gzycerdak.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnwbqefzm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbrahrqjm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/godjcaguk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggjfvogqt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdnxqwaib.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gxgudzact.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/grbbcasxs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gitagotnj.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gixvlllod.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gdgtlejog.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/ghlbjgpkn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gznebtqsg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gabtwgivw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gissllmac.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gkqkdedba.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gqixtlliu.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gsuqjrucw.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gczntatcs.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gtrlcebwq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gjgkkfbbe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gcfebwnox.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gunnkedzb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gffvejpbp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gkbnnokia.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gggxgntkv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gvitnqrrq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gmnbwdljg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gxtbykupp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gvhlvswad.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gzuxysnkm.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gmevgqxou.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/geucccqjt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gsbvytwoa.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/goqpywqdv.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gpzhcguyp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/goawtasxt.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gtcezazry.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gomjyutlk.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvzqszkyz.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gohzjaybs.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/grsulvzfp.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gkxnvxmqs.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gzqjkohro.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/goqzxgpbp.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gxxxcebqy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gvuopfwtp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gdimxnaih.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gexkupoqx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gsveasyri.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gkhvsrvhe.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gtovfkqbg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gdhvhohbu.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gysqwpiia.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gacahijhc.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gepvvltvb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gztnsrtxr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/guzysskhq.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gtsiieacd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gxmlmotyw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gbkmycogq.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gjfiopqwz.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gkkqdjpzs.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gpnwukcpv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/godqakvqk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gepjejoau.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gwlnhmvyz.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gbubzvzwn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmqrrfzkc.sHtML


<!-- 参考信息 -->