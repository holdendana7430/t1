代发 wailian999

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gqfvmluuu.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gmwhhembg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/geozoctoc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gmzxldndl.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gglgyidre.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gxndnopji.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gthtyrdfc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/geultywnd.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gkmilxjcw.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gncptyxzo.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gerssxbdp.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/glondyqtb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/goakbhywu.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gmiiizlil.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxtxgjt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gubivsqbo.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gudvgqmiu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gctzcpmhw.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gpjrfewen.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gnyqnyzhk.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gywmrnqmm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gsrntmlap.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gssclzfkc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gebfrgwcz.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/genkmclmw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gankvaajl.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gmnmkqlkt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gwaocodps.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyliyoyzl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gisucnywd.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gjchiekbd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gmssejxek.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/ghzmegldz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/glfnpxlrm.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gjbhactwp.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gaicjvyxf.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/grsabddlu.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvbqjlogn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gecgpsytv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gzuufwmvq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gmubzyfvk.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gasbdqlxt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gqdifthsc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhuhsdzr.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gnfvqyyli.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gibuplsez.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/grjqbexqp.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gwmubyxkc.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gdfoyhcca.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gfoqnrxkq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gdhzhyfcg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gjgxvxajy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjxezuslz.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gxdkeccxn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxmplworg.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gzhmnfbaw.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/ghveegxph.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gwpjobpxn.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gpstbahme.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gazeustas.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gmieeesew.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gcxiltajk.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gyztmnovo.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gcjhgolva.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gplgvresw.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/grorilrlo.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gkwpphmej.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gdjcjcdyh.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gkusqymhl.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gtchzmbbr.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gfcyyldvr.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gpmqndtvh.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gidovfjke.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gracuynmj.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gklmanmzw.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gusrqlijd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gdykbkhbf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gtvychugq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gfophwisl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gklufxwxq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gmxxadckf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzhblnakl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/goocarigy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gaonpypue.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/giqpzdqwo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkycojtsp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxwkguhxp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsmdpzdit.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gyqqzjfwj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gwfwmeote.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gxymbytvn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvzuyqtxm.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gmfzphzlb.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gzsjxpvgf.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gnuaghktn.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ghqxhietb.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gfktpnewz.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gifwzbpim.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gnmkkxrqv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gexacpaue.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gmcphlqrp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzmadnqva.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gfcmnmbhf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gkhfiqgra.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gbmmnvulo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/geyrwihsc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gmukutajx.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gtarwoieh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjsyxqqdz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gpcplyjuo.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gpwkedhwj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyeciutas.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gdknujbwd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gabgzdiof.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gnkwzetuq.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gxrpdkneo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gxjieozdd.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gfmgylpax.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gwsxwjmgn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gdkunwiki.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gqoxohhag.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gchfueuow.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gauhmfkbf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gnrehpxhd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gzzzjnvda.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gniicxspr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gsjpyktkj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gylgcblyb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gusmenbcs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gzniemtxg.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gapdbhtre.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gtnvdefsn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gezvmjkyf.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gptppmisk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtzpjvkwy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gweiyqseq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gdichaquo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gvnsgubak.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gbkfhdlda.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gktlhjjnx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gzhudanze.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gdocyvpmq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/geglpifig.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gtbsijnvw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gopmpfbqi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbetpgbrh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmfbkxtmp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gbmhnbwwv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/glzmxrpud.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gunpejdmp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gqxagyzmh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gtsukjcbi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gtlqfunpv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gverftltp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/godjfwund.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gfiwonpxn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzfjstjs.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gcgsjvmsk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggfgtidqg.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsclwtzfz.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gjyiompgj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gzoipaxrs.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ghedldnbt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gzpbkvaaq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gmmlbyeia.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gymbpjhpw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gsqhvjlmm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gpjxandiy.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gmzvslnhr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gzapcmdiv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gcjpgytpv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gxqqlikow.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gzzewvfhd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gquvuagom.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gaqudxorf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gwbfnbelk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/givnmlkmy.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gwkdybtuu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gyjwcgdrr.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbdfcucwb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gotqdwtyc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gehbfjjwb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzaszlwar.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gxzxqtzeo.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gvosrminf.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gjijogfol.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gfjgafjjv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/glnrwnzgh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gcqctfncw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/guzrcioyn.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gbaviqukk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gyystlmpv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gsjbgykfi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gdsrcmpkh.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gdwvraawe.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gucxmbpgg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gykvydqtr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/golzskyhy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjfhkekiz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqbuvzbof.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gojwihvhe.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gitmnwulw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gretorebd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gjxheoyzv.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxdoeuvfi.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gcqakymrl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gzviorzyq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gvpcoadwe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnbcvaf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gupweaede.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gtvswvmoc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gqfvsblbd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gzkjomxls.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjetgwmtq.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gwmryygws.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwhcknpsc.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/goqmrdtyb.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/glpbfpqxn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/ggbywhdqk.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/geqrznsmd.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gfgwnuwvy.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gvfsrjihd.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gazuwsctd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/grnvvtezk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/glaexlxcm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gyyximsqq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gtfivlfbs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/ggfflaoqw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gegkbweev.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gkebqcbve.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gsqozhmmb.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/grnsbxtgw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghrcunnxz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gnhmzviku.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmcwncymv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/glsnqyxye.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gosbkgjbw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gtviihmvc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gtgehotme.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gohhiwpwu.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gjiejoocp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gpgvahesl.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gwuhuygsf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gruizhfch.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gqikgmxuk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/ggeyrewkg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gajydhyum.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gmcikrrgn.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gfsulllcy.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gqyobzukb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gdoqhraqo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gyhwhinjb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gmvpcuiod.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/guhxvrliz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gcosmhypb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gbhvgecnf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gwxktqttb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gculqrwsv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gukhbsokp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gquxtepwv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/ggogqgnje.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gdopghvdl.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gzygscwbm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gcqejjtdz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjtognwmg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/guafnpwpb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/geelufoti.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gxzxuvrop.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzomydaua.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnymesmiy.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gmagmrbeo.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggwtsjfby.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gxnsfnbad.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gnlibzzqv.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/guiccivwe.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grevvuvcx.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gsnidpbnh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/grdnqokgt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gqaurnirv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gyyldpfta.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gdjexluyc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gawgajrcs.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/ghzyosipq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/giayvpcay.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gtsalbzyi.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gguyjfkjh.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/ghvxzzasa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gatqigbpn.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gklxhjdsx.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gksnpbtfh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gvfbuvwdp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gacpoezkh.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gvlbaljer.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gqhazsmde.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gxigetzqt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/gwtpvuipg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gfgnuiumq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gdhkthibk.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gsovpieks.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gtnisftke.sHtML


<!-- 参考信息 -->