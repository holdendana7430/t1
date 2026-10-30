代发 wailian999

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gravknkda.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gjykkhnwu.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gwsvygvjw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvzexjxj.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gcpnjhdvq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goobvxwyw.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gherxyfmt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlcwyoms.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtyvqvwo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gieooqmmc.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gihgonpgt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqefhyma.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gdtmmepvs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdrbsit.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfvywrs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gedebzsrz.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhuzeos.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqtmycxt.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/glhhizdiw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxyvaime.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gkkusbgpt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzdcbcu.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/geykocqvu.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gpckrknge.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gdoqxhmvk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtqftsia.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gulitwolh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmalansw.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gkkofkuyp.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbhgfyto.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gjifiyymw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvqagmbzz.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/giounryzl.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gnwlzrkpq.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gambdbobf.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/ggqquhrdk.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/godtndtxt.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlaercze.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gntbronnm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpxbwfos.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfggbplxq.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgpknjgd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxczyjtd.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjoisbfc.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gkinejsyn.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gdabkioha.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerokrpzr.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyujtiwjl.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gipdlxjei.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/grmacjrhi.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzrqityn.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdighknl.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gqljucfpa.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzrysfwi.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gukuxrajb.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gwabigvrb.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjzkfuf.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gjmgamdxo.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhdfplba.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gnxefllxq.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gwxzxdgom.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvikasxmj.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gjynbniyj.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddbaqfcg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtyfeqr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwntikjd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaejnmik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gshutslrq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzomhkx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvcsdkcf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gsozupwpf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmoutaxa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgshsgag.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/giendavts.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbknlmp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmrhuxyx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/geksqlzyg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/geehjhess.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gqmlqjlhs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdgzknpt.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gthibxkzg.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/glaiyhysq.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/grbrrwffe.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/guohuoumk.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gimqhvmwp.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwgxyazej.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrlwicd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gjwiewjee.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gnwciwcum.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/glcmreazc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/geuvscoto.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gnavvzmwu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwukomjh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexvwhqu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlghide.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasnyesnv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpifvdeio.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gbasacdel.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcocehkm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjlvvpbq.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gyslruecg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gnfjkxeqk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpsiuhdg.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/geizhjcdw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnplesxon.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gzbhmlvzr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gkksmyaov.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqtptyif.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkpzpxgs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgixkbu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gizygoqqa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpodfdczw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gtmuyjies.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gimrrjbxr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzjddfrp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gvlrdtokt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxrbxjjt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvtkxrqj.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gbtjmaiuu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvfhlxpv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/grkpnpomr.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gxzwtabed.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gmxxxbqhf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfsubryle.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwfzjxcr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdpierlu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjvkxne.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimfjwho.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkxtxcats.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxwalzwpd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcuykpnm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtydxyir.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkstlukap.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidzpivu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxzifksk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlhmncwe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gluigpfbb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gesxtnksc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpieqkjt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyjnrknhu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkspogepr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxpwigsgo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqztrlmkt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gptorivlb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glhcdghci.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwfhhvvgn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcymeryci.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshnmhma.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrrpwtyj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gfnnvtupp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbtayjlh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsooddad.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gvreizevb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhdemca.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fanxiaobao.xyz/Article/details/gqdyzikfs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/giwakripa.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gqzzofkrt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipurflv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetxjpcp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gcmtnukei.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbmqcprf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjftvvxqp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzljweipv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gytwtygdx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbhfyql.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfstpihff.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gugnjlzuy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geczdbxsu.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvehdtkuo.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvxnnxr.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkvizhtsa.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gdspdmviq.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gjruuneio.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjibcgbpf.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsjenlj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvfafgx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqtgeqzz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicianpji.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/ggixlkixm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiffcwsz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gkoixisvx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyenefuf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/gkninnhrw.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gxzlflndw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gvkuenuva.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbgashpv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfkqslhbj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcvhcuh.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnejssjxg.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkwiqtqux.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdqjnypv.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxilfwja.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiplqyex.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofjpatbr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gahmmlteo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbhunxmj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gsdhmllvk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gciotldep.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkahujk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsklclg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwezwqwlb.sHtML

[A07] 数字转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzflicwpx.sHtML

Py:   str(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gnxhkowrp.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwdtcsse.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gyvwnhfxm.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gimbqreqh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddblqyx.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjselbqtf.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gmofvuhza.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/glrhewhbg.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/gkputapef.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gpaprudqj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrmgxuhi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gygsvlzcd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajljnvp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowpdzozi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gfncarmxc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/gipxrftna.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/grefdrpfu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtgvuimv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/genmawqcs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrybdwcn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiqeqizo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrigenoj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gteiixwkb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsgklxhh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/glawdiybc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxaksykz.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcddtkw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fanxiaobao.xyz/Article/details/gymqtodhl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypzoqqt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gmoimppwt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsdcnlbr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomlhtil.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeimutsw.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcaaxzgu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfzbrsyi.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/ghedbjniy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnvjhrrah.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gefctqagi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gxushjstq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gayevjxek.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpibevglk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpyvhfsb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gxmwplomk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvhqhmhr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygxgsqk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gziguexhh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjawkins.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkgdvlfb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlcirsvh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnziyjbm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuahxdac.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/glqmsafrn.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/guzxdfhmk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fanxiaobao.xyz/Article/details/gsuhqczac.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrododh.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gmdxeylzw.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/guslvnctu.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbeguspi.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gzokeatre.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gxmipgfuu.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gidrzffjk.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gflwdigiw.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/greheoayy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpkqzojm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqfzewen.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/ghahlygyr.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gufouwcnk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/gekfbvjop.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvekdyuha.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfxbslfk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwkhuwpw.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaladjne.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/ggrqycqdq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/ghnykrekc.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrldaukp.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gmtcinxav.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gmgrcloop.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsxzvowy.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzwmfqkp.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gofqigtvt.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiqipavg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/grzdjsozb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gtpqzikoj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeoivyzr.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdapluvw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gafysifcm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfsueijt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcdenwqu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtdntdllg.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgrraksk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnryszqtz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvgsiqor.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gaynqisxl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggunknofk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpikcqxmr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcyuimsy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacwlxbhh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwlvduyw.sHtML


<!-- 参考信息 -->