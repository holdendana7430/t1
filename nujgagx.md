代发 wailian999

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gnjlzzzgd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gybjatmfv.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gbsswvyub.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gsvhgills.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gctvpteub.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gqmhcdfkb.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/grtcjxxuk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gylehrlpz.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gmqojgjkm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gbtetyuzn.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gexkyzpci.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gklimoziq.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gcuvkhrqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/ghiwpwvuc.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gpwaggbgk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gbopqpnuc.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gpugltqnq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gtoxmmiew.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gxumyxumw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gakbvawim.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gzhviwmnh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gtzbzblee.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gomvnlvty.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gzdsvehjo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gvqjrjgxo.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gsirsmcrw.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gnlcwjokq.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gpyrkopgi.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/glvvrgxzq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkylvpnom.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gfqccpfqq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/girhpjymi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gbuidfjnq.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glgsnwqid.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gghcpoytd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gndefyenh.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/ggjbsedkt.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/ggiytltrg.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gylpovhbp.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gyrpellmb.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/goftgmewh.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gpxytvrez.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gdiikghmv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/goxfrbmkn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqcaphghn.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gmskxkasx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guwuducho.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gvrbnezih.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gdotdawnr.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gdwcnptkj.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gicgtvhmu.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ggccoquez.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gmfzyzbzx.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/godvicenx.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxrfchtro.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gnqkethfs.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gksakauwj.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gvwziqpxl.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gildedhqq.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gsjyixrrg.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggqfilpya.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gqfiowfzc.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gjvkjnulq.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/guoqqjuli.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/grobjvzas.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpvqivfkq.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gbucudjuc.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gwpngcqah.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gttvxvbud.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gfrjfvayg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gsneqzcdc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gduowlarf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxeslbs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gzokyygte.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gdxpoimfx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gcwznxgkw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gsrjricnx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gdroavozr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzdwocxdo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gwnqyuzuo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/giqxxbqtq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwgymoqnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gyvcmsaws.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvibbzvzf.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gdmjsznhs.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/guajebmas.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gllwibogx.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gkvwsgtkc.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gjtfxxqgf.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjkyspfbd.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/ggnxetyfg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzwofceih.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gifwqsyja.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gztlfdksl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gwkezuxxp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/ghbwcghuo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/ghkjkovlb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gntesetmx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gexfwclny.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gxgifruic.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvvetrvcg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/geqyvrqqt.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gcffwmnlu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/growrznam.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gcsbfxnbw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gzbyktyul.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gehrfiexa.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gjrdayobh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gbpgphdun.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gyyzphhvz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gqyugfmvg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gccbghwer.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gnjyuyfvy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gavaesbtz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/ggwvulalq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gbvazqjnj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gbmcljjzm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gfnxdvrig.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gzlrpvpbw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gigzftaxw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gycitxfod.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gfjlswxeb.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gtlwoosre.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gmgrszecs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gvjprcdhb.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gqvvqqylr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqyvpxjqu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gqomhrocr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gmrbwjnta.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gwpozdubq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gmqvzskdm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/ghclgyuzj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gzrenjocl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glqbmmyxw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gouceyjbg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzhkppjfp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/glhbnrcga.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gfbaglqax.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gvgitvsgp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmxegbrqm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gepoavcsp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gpvcnjlwn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gysppqmps.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/getkqnqzp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gyomymyrc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gvwosblxc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gytsvddpe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gfzjjbysx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtrmhzbph.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gtxtcdgdv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdgqkomrv.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gdthgmmrm.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gxunuekhm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gklbxwdup.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gvvbubbul.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gitcdziab.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gmddrcquk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gzwgtnwkf.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gkjzczszs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gukmziomq.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/glhxunmua.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gvgxzoamc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gmaxmrzhb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gbkxgcffg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gqoazzpul.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gakzrjdus.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gadgfcsdg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gnbhrriay.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/ggamaoagt.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/ggzoisork.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gmqndlleq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gydshcfkr.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfkqtyuhw.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gihnzesgz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gezxpcvqm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/glzycmbfe.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gijgondqg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbawarumg.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/goiqgtduf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gotkzorfh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gyxaxgqnm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/grxloxrer.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gykkssqpo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gsugbwggj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/ghtnvknjc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/glfomlukx.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/geqxvtubh.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gvzxnbztz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gkugxjimd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxkhsnljh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ghqfatuhn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/giooeuzqu.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcotpsnxg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvtyihssd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfqngyptd.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbvpilcnp.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gfgayxkej.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gpxhiacyy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gprduigao.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/ghouaipuc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/giusckxmq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/guxxjvulj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gempjjxgq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gdmnhbcxi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/galbxdmss.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gjojuyhzu.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gogvdsaqy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gjzletzzc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/ggpcckrbp.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gffioyoxv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gngbmhnwd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/graduxdky.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gbdtiztmg.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gbszmmeba.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gdedvnjig.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gfkqktygm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gutjtivhy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/geyzdolvb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gszkarrzy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gzjqdfqez.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gttwzlful.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gmtiziktx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ganmrgand.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtlucms.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghkdfiyme.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghvgohywg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghgdaybyz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggyuxmosm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcdwjekyi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/grivlogmr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gkginlcwj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghreycxkg.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/grggspqqg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/glcdvfala.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gjablxzmd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/geayfsupo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gdfeowgvf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gqliscvse.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gkirqjbze.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/girnbxeds.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gupfwqonw.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gdtefzdtg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gvcgsjocx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gtvhgsgbg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gbfuxvjcc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gylvowpzn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gzzhlzhsu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gxnofphyk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/geijeewxf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gjgtizznz.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/grqxacxws.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gnlwvmmcg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/ggqbmwaqp.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gzkisudfi.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gxfjthgmo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gsdexfnpi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gmjcnprzr.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/ggknusqgh.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gpjmkejjg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gqmrtsqwe.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/glhsafymn.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/geabufrcb.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxcqjugyx.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpgacwlki.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gfhvhrylj.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/ghsdgsnoz.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gdmkqcmmo.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gefblthna.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/goomvoaec.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gkwoubxzo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gichdgjzr.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/goaqhohbu.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gltpovkug.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gkawmwvdz.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gfkeihhzn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gmhykeqbg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gzmncwidr.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwvsjgpol.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gtxayrklx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gbjliptjs.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gsxqrvqeb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gxizkakzn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/genijttdt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gnghjsmyo.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gzfkmuigw.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gektolaei.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/girwzojfr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gvxpblcvx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gbeieiwod.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/glvbczmhy.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gtmrmenno.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/grupzdnav.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gjmjebgad.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/ghomolifb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvgqary.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gpzqgmwdb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghqxoydic.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gydfvcldp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gcbacxozj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gyaiyugas.sHtML


<!-- 参考信息 -->