代发 wailian999

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gyzascvog.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gypyacnet.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gbkpjztub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gcsdnenrt.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gxzjtrlqh.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gvjgboglt.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gjwisjkkd.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ggwazpqhd.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gfhkaksxm.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gohjcfwnd.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gwntvtxub.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gsarrbhnm.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gnfzuvhea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gnbbxlnqm.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/guucghgil.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gsssxcisq.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gvxpotjmp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gjtofbrlj.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gtmwsdbta.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gciplzvpg.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gzajfglfi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggfffjjsi.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gxaebgryk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gletlgjow.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gnsdtykry.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrzynvwy.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/ggqlegvtk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gryvihleq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxplhqpcj.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gdxomktrb.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gntfcxvbh.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzdlmncxi.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gmqwbvnwr.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkgtmsfoh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gjeufewsu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gfizroxoe.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gsikixqbr.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gberzibje.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gbefrbnbc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gluinbwfj.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gtpmmcvca.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gkdtextvn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gjootivxc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gsypqzbyx.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gijjqfuyj.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gvhsqqcnm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gfrdfxmtu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gelpliter.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grruhvotg.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/ggjalhzsc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvlapmhyj.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gqgiscdcu.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/goeknferi.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gdjxfvdnq.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gsfjukftj.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gdgezrkca.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/geuwimabh.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/glvfdstfv.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gzdbvhltb.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjebejfce.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gzeoegskq.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/grzptnmss.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gqhjenjpt.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gulppagjv.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/glwudfbnw.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gezstkhaw.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gmgdyrzps.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/glsrjhgmo.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/ggvomrclg.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gckybkorv.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gtthfxpnv.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gmtyedglz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/glagqairp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfsfbpdiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gezjtxhff.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gqxqzfhyl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/guelxnspg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gjevznxmp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/grlaujonf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gexapwubm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gregdadvg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gqkoprbmu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzzsyaqkg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjauqawcu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzimqkolg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gquchznue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/glwviunoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gjchnfoqk.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/goyujcwpj.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gwsgkkscu.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gstmgrdwi.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gevqaduvi.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gwztmucbk.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gijkkgdfh.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gfhyhjpej.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghrzoofku.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gcfkwkkjw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcaznlnai.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gusecpdrj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gezjjlbmh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gzhemtzer.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/guciogyvl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/grvwawxrr.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gwojjnxbs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvhmjszkh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gndpxoyof.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/ghbbqxmnv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgvsvtty.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gaqpppggq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gvjabjroc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/goarhhaxf.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gioajlttw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gtrpuhaoc.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gvuiugfxr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gdaonmxtx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/genxfifek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gvetskqxf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/ggzqbzsnp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gvasjadof.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gofccyxnd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/galkumztx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gmxzxfaqs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gkcmajcef.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gcggxelmr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/guacswtsx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/giauvkwuu.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gxgiteurb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/guhplicng.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvteekbhz.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gjobjbnju.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gfkmtsmtl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gnunvfxcd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/grctsomdn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/goijcmuiq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gszmeguna.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gqcfqjmzv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbxzwzkea.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gtxeuiqqc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gxuudtmqk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gmvgcwmxj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gznjvvqiw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnofsgsoa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gnuiheedl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gufoxvymc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gbdxuybjr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gywwzriqn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gwduoyhtl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gykxhupir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjzsmhlrh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/ggclpalmv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzpisotdz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwapxfxpr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghnfmazom.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gcliqmavc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gimpbegkc.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gnhdsrkxg.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gvdbgdxrv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gvjwopkne.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gvcszaoyx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gyvxgqtvu.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gqxshiucy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/griulytck.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gdlapqqyz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gaovtgzai.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/ghswtmecn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gxpfqdxwx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gpmbujjos.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gmxpyjsxp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/glhmqnzhz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/ghkknmbhp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gwmsxyaxg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gvoobqwae.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gpabpzlcb.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/galjzwpuf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gaggfsjdm.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gigzcxijz.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpzzkogkr.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkuokpvyv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gqfwmzdpa.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxrzfxufh.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gvyzxzxbf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gopmlfdvw.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gpcgporoe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/ghezydlkl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gaidhruwx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gnsutfrkn.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gberqojaq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gulyihmlu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gxijsexbn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gowhhyrhk.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gjyrkharz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gpydorwvi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gooyzkrdu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvadtayoi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gytvdlpjb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/girytnixv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfspxdrvq.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gmucaqaln.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goquwczcr.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gulvwrkbq.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/giubrcpqj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gkhgjfdvi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gbfiksfiy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gsxfwxgpp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gdabjxrck.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/glagafrmc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gjkxmdesf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gpvvtglkn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gfcomgndr.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gnxlfqffd.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gcuktxyft.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gsytvarfg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gqhmqlcaz.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/grzoswdiw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gyrqkxmul.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gufvebqfu.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gjljyeemo.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gwvbzmtiv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gignhhzys.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gnssmxlfe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gypvrqtes.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gxoubwsjb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gjqpyscyr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gsxfgckle.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gxzvokmqq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gqkqjigfg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gziodawjh.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gairkhpua.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggdokdhzw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfmloybsl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyuxegzon.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/glhesurff.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsuuccrdf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gwyipusos.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/ghdhorynm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdusgmtyn.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gkncpvegt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gfkiospvg.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gcokzjvdr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gcvnfggwi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gxjzegnya.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gflkflizr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/ghwfxbgnv.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gjablbbhu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gochpkral.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gkoaalhvc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gwquvqgxp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gnpfooctz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gnzoeimgn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/grctopwfv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gzbvrjzfi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/goasfddmc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gokdenczd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gpcpwuavd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsijnbysc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gmoyfitly.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/grwlqqvzb.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gfntxxnkw.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/ghdumyvvn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/goarikhow.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gdkvjpbwg.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gqmifzgju.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gkjocooet.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gsbehnkgw.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/geuflxmje.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmrudaurg.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gtcplcqfl.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gtvgjrdzc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gibkecnuz.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gkoezoeoz.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gudogbcuy.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gowdctcpl.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gllnsexcb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gpvtlbuvb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gmxniivgs.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gqpwzoajq.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gvqjunfde.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/ghuhtaubx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gjxdmpoam.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gfnbrthsm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gbskcdlyh.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gqgbiexji.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gngmqyzre.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gpobwiozq.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gzdvplxul.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gudyvmgsq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gvfpwpcdx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/ghpechrgr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gpystxcnr.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/guurcajhi.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gkmbfsfoq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gqbjxeupx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gbzehtyko.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gnquvkilr.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gorbzfywc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gdlmcjcml.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gtlxaoqwz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gjkkyskvu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gsjqcuzkn.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/ggupwpojh.sHtML


<!-- 参考信息 -->