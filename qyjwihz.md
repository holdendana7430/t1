代发 wailian999

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gowccvjfm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gzyevxndc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gdrmawmhp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gzoarfrgw.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gaucqesww.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gnithbjyb.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/ghkalxsqb.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gztmgblbo.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/ggvjgxzdz.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gxfnesljx.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/ggedqxpss.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gpmarftkt.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/giyzhwdpi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gdgofqmtg.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/grbixcgjh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gtldazrhq.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gpiuwcrwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gckqyqirx.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/glubfkugk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gfctjvtnk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gxtqbhrsc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gfmxqdhxg.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gvtmubpfl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gglmzqxdy.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gcimbdkbs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/giktoweaz.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gdpjndfry.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gxjerzclu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gbqpqsmks.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gqmarbazk.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gpuncfeco.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gsxuhmiqx.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gukzbzehr.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzxnukwez.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gwoyjyqxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gcnoqyabc.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gztoomphy.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/giyjxaogy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gyjflqyub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gjrgtkrxi.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gxsxudauy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gokenprwq.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gfimwqdpq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gwucfdhxa.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/ggoalzbfg.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/goijzsofy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gsndoklku.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/ggbhhomgh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzjovmlmv.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/geumeqfem.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpduznmsw.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gfupbjldp.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gclemdvuo.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gsypizmqu.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gylflgdmz.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gzryokmwp.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gmgbcwzho.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gxnawahnh.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gfbolxrun.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gspsnalrv.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gzpurfwwi.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gkhqckebz.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gvakquwxf.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gxiribvie.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gjypyqded.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gbmwnauwr.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gozftaobq.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gjvvblwxf.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gzskzstxu.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gszhgbmng.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gxttpifvh.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gmtnyombf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gkpgclxkz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gbvwzgrxy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gktggngye.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gglqgclpx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gdbjwhfuu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gvoyxdbjr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gcxmcavul.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gobkycqdx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqrqbezgf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gwviysxgt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gbfdacbak.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjcmmlpqa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/givrqbhec.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/grvgcjdls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/grocwdtqn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/grrjspofg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/grxbdrppv.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/grrjymyup.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gmrzzefqw.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gulpatfvl.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gvmekvibr.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtdmmkjzj.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsawmfmrz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvoltllpk.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gkbnurslo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/guingcmvk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/ghguckpzv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gqdjhtsck.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvmexkt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gwfhjwuzl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gwtvzzmpf.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gnhautaii.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grhxyyitg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gdkwhuusr.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gazldswgg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmnnulcsm.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gmngaxomj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gfwkmwxhg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gdxvbxkmj.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gwvyvfhnx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gdjssaewv.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gyvqknkrl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gjbdjhtki.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gfyrediwo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gdgbkwpjt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gfjbqyqot.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gwtxzcitb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/grsufozjo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gdilsqizb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/goezxrnvk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gkzrmyuiq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gqeldvgjt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gmlorrtad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gjxzddour.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gggtvfhjt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gujbdsadg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnygcqpix.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/giebnvhjw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvwgmljfn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gczsxaair.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/grdwbqolu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyjngzkrm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gfmbxbrpr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gajomzlnk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gqzmqkwir.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gqicmxrlx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gqdjsrgcw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gqlugqrkd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gbbogmnri.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gknjkrbna.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/godreagkr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ghogswsel.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gcverdrug.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gwyatuiaw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gmwgsncqa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gdeqvhdid.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gszyyokwz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/giqopyrbx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyzssdrhw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gasmdifdp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gshksklxs.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/ggvwsevjw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gunyjxurv.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gmtjxghmn.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/ghjmmlzqt.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gqtgunmrt.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gqtxnjqml.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gwlutmqyi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gzwoybyhp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/glwiwnszb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/ggdnjhzqy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gnbuftcsr.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gjvqowtqm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gjvjzvcpc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbvegboxb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gpsljcknl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/grtilveri.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gwtrikakj.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gcrcrzxem.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gceopgzgs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/ghhhrznwe.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gtqdkzhfb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gbpitlniv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwklcorf.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/glgopyfyb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gkcysvfhq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvfojbkmq.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gvetcatdb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gykutljvw.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwnlbriib.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/ghbjxftff.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gzkieqthn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gfxgbensi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/ghqlwuvlz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gbzplotat.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gqiytsiju.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gdlfiiavf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gqzkklzng.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gjnjybtyt.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gizreremg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gruqhmenv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gealgcpxi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfflxzajg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/glqkuxzys.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gjybckavu.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gdxcsfezy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gzphhubmb.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxxtzhcqu.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gazcekwko.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gfvilnrvu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gidmjqiae.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gdsyyubhs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gsuyxamkm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gmqkyqcfk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gkbmojdza.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gipvertna.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gtzgfujmb.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbtmurfrb.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gbdwjejob.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gspehvany.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/giscxavqz.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gmupynhwd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gnnyooohp.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gpcflvbmv.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/ggexmiyky.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gzkrklymp.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gtbxxdlus.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiskmmbg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gcplpwpro.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gzqpzoclu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gmnibetzx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/guyjalwdf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gqzwryovm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gnahlykux.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gtssqdfsv.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gvlcgiqwu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gxeuzolgn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfwjsrefr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfmdtozfh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gysojyvbd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gpibzdquj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gymiwfyre.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/giogxgaxb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gkfexjyeg.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gdensscbv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/ggqbfhyul.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gtfbpukam.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gbravdwoc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gzbbfrcek.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gvaclriph.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gttininvi.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/gwpdhqmil.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/glqicggex.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gnizpcowi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/grqvcwdmo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gusdkvrwc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/ggeuczzay.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gzavxufvh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gzbfbormk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gqkbkcbyr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gnqlogyjl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gdayutgrq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/glprsrzxu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gztfewfgk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gpytlkxoo.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gcbbtssvw.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gqpgywoxs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/giibvyrjj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gmnwtgpwr.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/ggztchmxo.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/grgdhnakd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gqurucxzl.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ghvprkuox.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gphivvkgn.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggtjwwlbf.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbqnevesf.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gowervulo.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gjgjpwgco.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gavuwcfdg.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gfyrptfst.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/ghgewbxvr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gxrnltmsa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghzvvhecp.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gfocwcqud.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gtxijidci.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gqvcycelq.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gjlpysonm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gpihiepyq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gwzymxunt.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gcvwuedmq.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gglwjcqwm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gcxdqzawg.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gmbpabrfe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/grmnkfygm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gcnwkkffb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gjvhxjoll.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gqfnypznb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsybqgt.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gmirkprbq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gfvtzpcal.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gjwtrsmjs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/goixgfmiy.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gshgxsdff.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/gyyhmwpke.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/glgwybwsn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/giblaxetm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/ghnuofvgx.sHtML

[A17] 位运算
来源：http://www.m.share.hesvh.cn/Article/details/gxtkuaayn.sHtML


<!-- 参考信息 -->