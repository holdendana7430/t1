代发 wailian999

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gywqqszbc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glctgmzbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/giezvjodh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gdyaoxdve.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gvffxmean.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gstvcgxrd.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gabpvlzly.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gisccnxgj.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/glsjyrcrh.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gyjmdvnov.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gluioolzg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gboowmkao.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/grhcidbqk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gmbfuuhhh.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gnucmrtpk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjxwigjvx.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gehskbypg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmevlomgk.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gdtbogcrb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/ganxmjgwu.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gstnjxtsc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gczvcudtn.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/ggdjuxdhv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gmlmcgpfu.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gmsiugjhv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gysbkrapv.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gfkttygmp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gqterzlbx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gdjshiwle.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gbevjjtiy.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gzaplkqwp.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gigcvawbm.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/ghcftmmxm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqgnpaznu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gowxkdkku.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcgvowj.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/glwajhwdr.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbziblcvb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gmkaxmioj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gizqlwhdn.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gfwflxhac.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gwhmxrbyk.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gbwbpacnp.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gjjoinwrd.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gpiedrpds.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/ggklwpnra.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gbezqexmr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gbhkoptci.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjbictctv.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gldlfqvhy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnjxrwpav.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gpdhstoub.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gtfydukly.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/ggohmzyhu.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/ghcpmsege.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gjnselxkj.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gpibelcgw.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gvkqyxbnq.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gwsagcwdq.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gksrkbvlo.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gisqfmnnn.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gbpkrhgwu.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/ghfqqzoxs.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gkrmalpvd.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ggijbevyg.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/glebyetem.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gjdckgtxs.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/ghtuhsfgx.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gnnebmzns.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gluiyxinx.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gsnziwfpg.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gavvtmpsk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gwpviyirm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gesmvcaxa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gspyhuscd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gjflmxftc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/guvrqeqdr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gemkysyoi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gekrwrexd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gcxkysygg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gvrcpiwou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gdwzskmji.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmyvdsyot.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfvwxkvsd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gpfdkntrt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gmcdsczxh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gsfkfzbff.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glwrelqyt.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/guergnuti.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gmtreomzn.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gyskuxtva.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gvgzcdkxd.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gspneotig.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gichvucef.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/grylxtilt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gknujninf.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/ghtltjhka.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjdlilokd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gaqbnvhgz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gxmmjmlrj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gjbrtjoxy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/glnxrtklv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gqxgtkllr.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gpuewlzut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghilcsrmv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/glywtdapz.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gqdugnztq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvogjenix.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gdxbfgwmj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gbortsiuh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/ghltxcfam.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gnkkdrkmr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gvuinxsjz.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/geejpyysz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gzkeejcvy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gilcatufj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gbbseclnb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gxrxegdei.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gcndezjdp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gmyuscpld.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gvggosunb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gtthhshhv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gdiccgxap.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gkfykirjv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gwmdpmvzl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gjectzuwy.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/ggwudkuds.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gbcwwsxxc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggjcamvps.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/guajjzila.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwedfhyxt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gscnezmsb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gdbwyqxzx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gjpbqawyw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/giamahuoq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gaoyuybgk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gvodogalo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gqootivlr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gedryiegp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gsiseezzv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gnyxhdxlr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwnxvswlc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gijkxtpzw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gccfubtir.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gvwrzdrph.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gsqzfciuy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gfobobbqa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gidvtamty.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gjlcinofl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gqpwfjvtv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxwihmsln.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gawxgbtex.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpcgoeri.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gqobxvwkq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnwstysfb.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtoqqphao.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gfmsdnsia.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gkazblqjm.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gtrawgtpl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/giaxlgrvz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gaeqwffop.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gjnkhswvw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gxugguedd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gjaazxxzx.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gfunomcfn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gpnxcthqa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwfxlmrso.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/geakkugen.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gqmitthhy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gvjujjdkw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gbhgbyydg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gtyksydsx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gknqqxpqp.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gvyllsyqy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gcktsrqjz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/guuzwmccz.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpkvfsqzz.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/goecvnalu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjrydfsnc.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gbhpwirvr.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gmyfzyfux.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkacbvgcp.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gmipmxzym.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/grlbxmcjv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gyqtfuvrb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gbslxvduj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gwavbdtlu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gndxkayzs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/goyzysjzf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gqykqduax.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/grctuyvvw.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gxwvrzvkr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/ginnrxvmt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdetwpmwd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gixiiopvo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gyaeallfw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gochqrnkv.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goabfnhdk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gdzukfmff.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqgwxhsch.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/ghxghsbdi.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gksyovcot.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/geoboycay.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gvkgrzkqn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/giigestjp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/glyezrkiq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gsqdfdmmz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gasmflgak.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gdbndgklq.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gybtsdumu.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gavtzhdxb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gzjveksug.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gegeoknfj.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/geryufxip.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gdzowogbe.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gjxbmdlvd.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gwlvucyim.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gwweesqkw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gvuikavit.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gdcijhubl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gyudebous.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/glnpxinmv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gqsywwslo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtywydtjx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/goezrgpjo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/ggdnzjtva.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gkmdobutg.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwatnxewr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gxwuxgqfp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwnrdrbbi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gdamoucgs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkllszlzk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gidjwudtv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gglfhdxkq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gilspbqkw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcrqmmlhr.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gvlbubjak.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gvyvmmucg.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gnvaxbpoy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gyzgfkvhb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gtzwbshms.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/genokeiei.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gipykebwu.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkcgbej.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gwxmjepjf.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gevvxxjet.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gvoydmgvn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/giuupdcna.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ghcuwkuan.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gxllxmfbw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdsprwbli.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gzszicejc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/glnpqfbrd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gsbqborof.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdmxyzmbe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/glclbcwts.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/ghdnxylpi.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gfhfabrne.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gzfonxzal.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/ghsgbwxom.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gqtaddbhl.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/geqjepfyj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/gsdpagjph.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gyplyofcg.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/glrvykjox.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gdpgaiiof.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gzwxghciz.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gylyqfijn.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzizwkora.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gcpzulppo.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gyyuqxsqn.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gynxejsji.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gzrkayall.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gzvcpagdn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gozjdlwbw.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gvpheekjx.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gurnshkao.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gfbrdadlb.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gulbfzqvg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gehllfrwc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gsflmcxjp.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gphjvtebx.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gnuxlcgnx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gklerjfad.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcylqbbrv.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gongryvgt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gftpprdsx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gemecorrb.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gihjjdoic.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gzkhwwgzg.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/grldhusgx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gpavgmntd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/ghcnciizo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/ghqpuejur.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gtvcmdmrz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gizkazrsj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gujqchjsn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gdpdmbprk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gheomezxu.sHtML

[A17] 位运算
来源：http://blog.fehbvm.com/Article/details/givqrqghr.sHtML


<!-- 参考信息 -->