代发 wailian999

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gnlpycoaj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gffddubyp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/grgrplpas.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gqrbzglwm.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gecjgqeep.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gsecpngsb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gwawdnqbl.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gxphlyaiv.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gewqpxxxb.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gkppzvcys.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gsghhrveb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gmzxovced.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gnnxzrmic.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/ghxbhrbmw.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gyrqkuikd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gcccdcxci.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gkbotyarl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gecfgbtzo.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghzgctydj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gfftbulwn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gfghdpeue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gbqxjakep.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gyhgitcft.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/ghajtealz.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gqxsxvsrc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkvpuqnlv.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gmyzywbuk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/glhwvymmu.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gcnymsgus.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gocjphrbm.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gtysuilpd.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggqesfhfw.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gekndnprr.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gloorargo.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gtncxopwh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gnhhldjgl.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gvvvrgzxp.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/guwgdrytr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gmmpgtvgn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gptybslyh.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdpkdmktt.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gjyvpzafl.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gkfxirmlu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/ggpvwzkqs.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gldrjwxig.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gvqqjwsjp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/glnzwwiwd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gnngzsynw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzlchihgn.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/ghiqocafs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvtpcffxn.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gvkacrtkr.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gvfmevtbh.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/ggrohiahu.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gnexshqxx.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/geeqovvut.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ghphqophk.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/ghfrafczt.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gfexefhky.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gumvcbxrc.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gezcanqeu.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gcfjodeuq.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/ggxffsrta.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gdjnmvned.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwkjqbglh.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gwbbopjef.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gkeonhwhk.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gvbuchuho.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gtparbqnq.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gblqdgbcw.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gvturnriw.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gsbctxdye.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/grizsspdm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gkzomxcul.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gqammarjf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/ghvbgbmku.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gvzchfpak.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/guaswuixr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdpckzsmf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/ghacddzul.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxzuehtjt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gjctosaql.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxkukcufp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggkhpswvk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfzlrlgqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gvtjxmjth.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gnrxcqrko.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/givhllsov.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gjbarvikn.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gexyhvvwt.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gmonylahy.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gbpuxblea.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/grkkgiadm.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvyrhcjke.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdjlizwho.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gveiloxed.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gzgzchijs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxrdrxloa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/ginqrvszq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gyhgfhtmv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gwuyurqsf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gfhdlfehi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/ghxeblnqq.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/ghwvmmkwz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggncohtur.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gvzcxccex.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gxusjcerx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gylumzyeh.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gnkuperrv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gxmnbqfzk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gukadhzas.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/ghovytlya.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/geegmgheq.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gbuhckxfm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gkeytfyty.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gjagkwgwg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gwatrcejh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/grcguprsj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gcvvltfxx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/ghnbqrtge.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gdsumlrks.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/ggfjpvfyu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gopvqgzzr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gyrqwjhgn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gpnroyrvy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gpqagjimn.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gcqlcsfnu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gmdxafuuc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzqwrikwk.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gyozegkwn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/giqgwinwp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gsevakywc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gbgdlxlha.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gmabqwgte.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gimpbrdqt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpitvzrej.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gugdhmjvv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/grdmjtwxk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gcxhtowzp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfqpnfyvj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ghrwrrfcr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gymzcpcng.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/grixuuduy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gqmysguyp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzktzew.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/groljtulm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ghgtnutys.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/getuzyslc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gggoqqehp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/guoulkinp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gmnkxvgmg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/giwuneepv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtbzsrlaz.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gmjemuyly.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdalyqkxc.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gsbsnmvhx.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gcbuggcsy.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gglumlypx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/glnhdqiwt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gwtjfxcbx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gqxyqtvtn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/ghqxuungv.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/grwglvvvt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gdcnyzfeq.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gbtazoxbb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gloxkodyk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/glbjesoar.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gfserzbso.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gwrrncttz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gmaldpoor.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gtjfcwvgi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gmqpgeygb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gwbbxhjqb.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gsoyqqnly.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/guavtmhll.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmurdmusp.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpooyrxbr.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gglqvqngq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmdtfndlz.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/glwtuyqam.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gkarrmrgx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvlmmkziq.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gyvkgcayy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gcourmtmo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/ghxfhmzub.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gfervdlge.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/guuzwrxuc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gxyjwvsrl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gxyscsegb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gixlruinf.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/guuwmhnim.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gvwdlhqza.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gqbacxirh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbwnuqejm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gimesnhjc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gactstubu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwcvoealr.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkywxthbp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gozfacdzw.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvcevqewy.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gmbyxlsjv.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/glmrhmwcw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gqcgvkkxv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/guajqzumk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gicntlhqx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gbvtcxgmg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gvszqlepq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gggnptskf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/geajqpwit.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gobuubaum.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaqkeyvj.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gdjlsvabk.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gwqlcxfkm.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gzkercnxf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gvkdxvnch.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gmmjkzqxe.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/ghdzdascr.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gkeiilupn.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/grkmedmam.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gpkqzjcib.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/ghxxaohip.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzzjmqdce.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gxwhlfdjz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/ggqdonksa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/glhmtpvqq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gpitmarqh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gupzzniap.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gfxjvyfga.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvresjvvp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gnrbreavn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtxopjjbz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gytzfnubo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpdlrrkbs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gbcqhccvg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gzhemwynk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gabujnvmr.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/giukyzcuh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gkcocgcjf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gxktxbqxb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gkgwptnxq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gsmcryguw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gjdaekeso.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gcygllywp.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gqpinnojl.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gjecdlsmc.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gepmbpmyk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gvcrkprll.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/guoaexxsg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gzhhwrdbt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gtwnynfag.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gyblttnhl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gwkuehuux.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gpsawvrst.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gqkmejkwi.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gjlxtthmn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/ghytlonwd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/giwzplajg.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gjhsulwau.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gmgthaopf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gqqklptii.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gnwmedgqp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gnmyldyus.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gvtqucsiz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gluqyjzvn.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnpxxcubo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gyymgyfcq.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gzbxyfwhx.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/goususwdt.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/goamlessp.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gozhoqjre.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmiehsmfl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gfkzvdhlu.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gkdftalml.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/glrhgbkqa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gpctlqfmb.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/ghrorqnjt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/geworgmhs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gqtpufdwe.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gcmuwbsao.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gowqfpqxl.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gsejrhqnu.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/grzdletgy.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gfcssxoht.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gwznsgnxx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/ggpylwblg.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gefobtyln.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gehlvwtzd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gwkfakkje.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gifuyrnug.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gonbbnasu.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gxuskdoqr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/ghkirgsrw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gnzmezahc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gshzbnyqt.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gujqbpdxk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gdcbhfgdz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/guzjypfqx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gzupipfov.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/gdvxwoiwe.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gyybtaqzb.sHtML


<!-- 参考信息 -->