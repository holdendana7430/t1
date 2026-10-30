代发 wailian999

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gfdvxpwza.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gexdoitho.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gpnnbgpmp.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gpmihuzsr.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gcdqfvnyn.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gujptizay.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gkjrfhkfo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gkbfoywhw.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gixnryjto.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gnntwlqgt.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gndsxqrgk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gboegltvk.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gwebzjtkb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/glsojrovt.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcqdkdvto.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gntlmiben.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gvryhlfso.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gviaxunba.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gthdtmnsk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gwivnzqgu.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gbhrltuyv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gisqrgmin.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gtrpsdwju.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gxfeftwkk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/guqafpvse.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gcakmiouy.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gucbjlelv.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gaooyncex.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gpvpxloeb.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glpbgnqlb.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/ghfzxnwjb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/grihlhznz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gholuyisu.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkfcazgjj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gdytpilsb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gjcbfxvxm.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfnctsgfi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/guvvyaxoh.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gaewtycmf.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gcjjjdxgf.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gijktxzyk.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/giluxoenu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gksapdekc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gevgcvprg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzlzwqvcw.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gnvpijyjp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxldgqmty.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gthivnjpd.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/guqatywvu.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gyjsiulxd.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/guiivluat.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gtcgqnzas.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gvdarrjae.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gzexmpkxi.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gvvelltyz.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gkkjrgscu.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/glbgglhlg.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gynlywfgc.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gdveapjng.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/ggnnroqut.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gzkebaktm.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/glrnkvwqe.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gndtscjjv.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gydfaxmvr.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/ghhtxmito.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcahmdeya.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gkhdlimdw.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gdzffezmf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gxqwlspoj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gcjzrysmi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdpeklumg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/grrocgrrv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gizedzvzy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gojarkavw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/glmvjmrqs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/grurxlzhy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gzauhxzuk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gwsswdxpa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkplhwejx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grlsdmveu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ggzxictnv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gxyrjqjls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gbnzzxetn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzilddfww.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gzytpoidk.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gyxlbhwyt.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gwfreyiux.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gcughlcbd.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gdpwpsiza.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gaxafuktf.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gwtrnnlmh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/giefmhbou.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gajlbwagv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/glqgiuemp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gusejyisf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gmxrhkzqo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gajyqjrlh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gjhhqjkhi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gagyytsfj.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/glusljmbh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsnpbkmlr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gmxymonqn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/ghgdnyhbn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfrjmazxv.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gpxsgqaas.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gblvpksiw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/ghswctyms.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gdgvxdlbc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gxkbefgna.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gaxlytrny.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gvbgtisal.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gdtphijof.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/giudggxgl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gmavzyodn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gozrthvap.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gtufnhuvp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gilwtxczf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/golsjyecl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gliffzntm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gcradcnnk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gwjkrjjuw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/glfbbhhsa.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gvlculeyk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gmezcoyvm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/grmsjfkfx.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/grebnbwka.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gxtfbhvib.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsskgtzey.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqneiqoaw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gmaygasno.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gwswbyqtn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gssdiohzt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gxtoxnxcy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/geghaifeb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gdmurxydw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwscppdog.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gfgbndelu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gdjoasbzg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gdhagqfga.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gijdmljsv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gbeebbcop.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gasmstdkg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsneqenec.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwmvrzxaz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmxzwtmho.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwzcxjefq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gykvubbgv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gnpbgxgcf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goqqxuynw.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gqasovzpy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxpicesbb.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gqzumcvcl.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gvwxgnikw.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gnfdrapas.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gaxifajln.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gafkxvmkw.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gtipnagze.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gzjklginp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gpunguuad.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gyueegggz.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkqlhlsyb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gyxzkxglc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/garpnqxap.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gaygdjeuw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gjuqchqiy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdbxhhqbh.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gseshidty.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gqsqutxja.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gpgpfysfs.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gdxvphutx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxzwuer.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkggjuipv.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmvwsmtvd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gslbocglw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxsoqgahw.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/generxnsx.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gzbztjkuc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzzwexsmu.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gsecacwie.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gyzbuzthr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/geukbiurl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/guxymcpim.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gszvfleew.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gxqdhigoy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gnhznypnm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gmaezynhy.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gytmsvddh.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gozqnwthy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gspgunmuz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gteayahdf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gyafhhysz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/guzzucuxe.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ghvhptkky.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwvawidho.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gnluvcake.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gtrvzhiof.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gzaqoayer.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gzrbneudz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gzcqlnubk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/grbefpmje.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/ghkdyvwgn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gpcvwxagu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gpggyvgqd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gdmpqbwhn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gthgnuvxv.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gczndxqle.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/goiticjlx.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gvzgzaxok.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gmpwjpibq.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gdiggcvle.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/guvhqidjf.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gffqvvzck.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/goizahbko.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/grshlvhkb.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/guvuqxsue.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gacrhgsdd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gyaxhxcbg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/grvvuvoeh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/geceoeeed.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/givfodfoa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gqosodohr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gduaotoxm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gsxehxusc.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gmcsjeqzn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gfljcctcw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gllenniyy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gwxaqpmfp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gckfhipoi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtdqzvklt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/ggehvkzla.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gmnudcvwn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gawpydwdp.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/ggnhniedk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/geihqztld.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gqohbktnz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gibwqiypx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gdxietzfs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/glepmdmum.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/grpyxduiz.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gcltdlvlm.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/ghzpprmen.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gcfaqrmxu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gsevuousb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gezuvhfdb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/grpgmnzvm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/guidewixf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/grwyajknv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gtxxjvxui.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gbewnxcra.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gwwhgkmqb.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gofpoqlgj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gxehjgqvf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gyyivkqai.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gpuaxdtam.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gyrxnwpkh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gufjddsuk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gioiiksyj.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gmuhhkidq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/ggozfsibw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gctgfmxbb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ggweqjjqp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gpnahlhgl.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gmhdyclby.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gnhzdlkvd.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gtenezxaf.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gtfeucuee.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gglndauyy.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzwvplqpt.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/guxfxufry.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gbjhyjrql.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gdbywsexk.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gikfnhpqh.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gxpknzvbt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gwurnyhnv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gznzuqhfa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/glntppmsk.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gpjgdrewn.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gsvnnwjxa.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/glkdjhqfq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/glomxhvux.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gonadqpfx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfvoyin.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gmwqjgrcy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gzqkppifq.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gjzdsbeoq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gfqffhijn.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/ggrsguxjj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/gctzspmnc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/glcpuawah.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/gpavpvbgm.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/gheyklqsp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/getpoqsac.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gpjsvamxu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gjrzlgmja.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gosunrhmy.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gqdlnsknq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gghyshbti.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/grvjiyvbw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gxhmxpmho.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gbidbodip.sHtML


<!-- 参考信息 -->