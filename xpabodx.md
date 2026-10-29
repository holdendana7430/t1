代发 wailian999

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gtaehrslc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gciiyhizk.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gmsllvgki.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gzmxysjdu.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gufrkovvu.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/geodvtcwc.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ggotsviji.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gqwguxfqa.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gqnsbiajj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gbdqkywjd.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gbquxhrmc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ginstsgjz.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gzzvgovoo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gzofweunm.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gjnaijiec.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gpjtpxwxq.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/ggtmjkfhi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gesegejlg.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/giolcscav.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gzktcgtql.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gjuohcgtd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gxfwhatuq.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gghlrzdet.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/glpndjsim.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gaqfazpcy.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gzyolboho.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gzifxmhhf.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gydbddgjz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gbjgjhxqm.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwuhqceft.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gxamdyohw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ghjzpmagv.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gzbtvxsyz.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmjlxjkzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gbmzitbpj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/glyfhplns.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gmjihnmhx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gdptrkjau.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gpjxvxbnt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gnlduagxo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gtmocejad.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gwakpwezj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gidhoenvh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gqqmztkct.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gevacfvva.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gjoaznguq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guohkcwrk.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/ghnavznky.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gbeuiahke.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gwaavzldx.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gewobmidr.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gsuqgnokj.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/glgfdfggc.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ghpffrfxj.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gmkthojfc.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gyshemwgm.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gohdjidcz.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gwbwvacib.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gwsmvpeqt.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gondptqfk.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/ggijzqrnq.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gybaplwpv.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/govxkhdvw.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gzivwnzjp.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gwbymdvye.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grrfhigng.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gghtigahk.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gdmzqkhkg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gaaliwgez.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggzvcxwfd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gnijtmtou.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gbieotfry.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gorufrzsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gisfburzm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gcsksbmav.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gnwciswcs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gfqkmkpes.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gzocvummd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gplhbqlgj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbzjvguye.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcicpuasg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gbyopbzab.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gujuntnvs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwwtyzqgp.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gmheyfudh.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/grvwladzq.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gcfcljmqd.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gropudcil.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/guzudybji.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gmfukijzy.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gfbmpnxsy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gcjnsicki.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gpkzlvhet.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqvhlaaiw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/guyiblqoa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/ghfqchzxq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gqupuahkm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/ghyedhfys.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gfhjxlaak.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gepwtfuok.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gprdmzybn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gfvhvegvw.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gkgtkxnmt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gogmtjgen.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gqqkgbsac.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gryawlfqp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/goxxsrplw.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gdwvsadzl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gqgfaxbly.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gpuvqkrfg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gmxqltvkm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gawnszlct.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gltbeetjx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gkreeqyyb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/grnparlvq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gnrtgbxxk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gniyczprg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/ghtpphgrx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gvpvtlqkz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gliwqmasa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/grzcwvqlr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gcuetmehn.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gyoaptjle.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/glvasfmlc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjhjkgkcc.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gesxboyfy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxenjbkse.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gpzzierlz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glhyjgddw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/goaqjdjjj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gmlihxzwc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/givezcvik.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gvvrdwuve.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gpqzftpwc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/garbrdtag.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggcybpxqj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gbqhcznkm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnkglvcly.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmunpjqzi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gjkdfgqyy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/grfurrtii.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/ghsvzrjmx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gabelusns.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/glheolwvj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/galepjblg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/goazgmcey.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gesxkkktq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwdikkkor.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngneqoqo.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/grogagzid.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geofdfjnc.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvwalqubw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gtxxxaigj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gzqlajann.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gwewswggr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gdjmfcudi.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gzzegxkbx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gaxhtmuqy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gutolajsx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gkpmtssug.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gthypiubi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gjakbqlrm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/guksxodyb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghmarhcmk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gpdhzyqqb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gyzboajbk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/geetltfva.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/giyopaaie.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gmzltlccf.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gcbxylwnh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gtbvnvcvd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/guaacbvkg.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gnnjpotid.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gaonaxgqs.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grcjlhbyl.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gomdotbsl.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gtjoxmpgr.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdyvwxqdk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gnlzalspt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gilplyhfl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gwsycbhgs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gnadwwdfd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gkdfbpsys.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gtmbyomrr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gmmdasrwl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gktwbmlng.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gtfzemzya.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gpawzhtfi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gztkoueyt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gmeamywjq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gytojagpm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gmzopwgra.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ggdqapjrx.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gyczrvmrh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gghxrejvz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gsnmdjgzg.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gyafcxidz.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gumgghlir.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gjtdxcyye.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gvfywasrg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gmjjeoacs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gqjjsuxsp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gygpusyoi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gnrsxqids.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gzygffcqq.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gnararslo.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gsjwlzemz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/grwetdtfx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gclyjujbp.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gohjqoati.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gmxwfrpxz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gxyipvifr.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gckoacaae.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gkccxwkuz.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gjdiqgmlq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gaqyrzdtp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gbkhodhrk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gkzrdylfs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/guuscvcbl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcztuqgbn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gqdykbkzc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gyofqmdkl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gxphxvvnq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ghjpemoqa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghqpkiyil.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gpmtoikqk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkdksvxgt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gdvovpnji.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gzyuvosns.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/guabxogim.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gpacaixie.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gapgpkcyh.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/gukxvzqgt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gwxzpqhgb.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gkccigtis.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gytaontrb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gvvxtkkmd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gkvxkrnnh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gerkmmauo.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/ghocpgsui.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gumrjemsb.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/glhzczmho.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gflmoppdf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gaqhxuoza.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gcdeuptoj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gfrjnfrqd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gcnpisxka.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gjoqwxgjm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ggexlsobp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gqmzswlhj.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gkubcwrmr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gbgzvvwqa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gcupwvsnx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gbqrjtdlz.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gmkkbydjj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gmkdkdtmz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gxrmdkqzk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gnxpxdmnb.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gcjqlgqcn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gijnqjfsc.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gniyblwzm.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/glpwhalhy.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gttlbafjb.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqrngqele.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gyvjpokne.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxpgnphfm.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gaqivjghv.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gclzmrwjm.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gfppjkrzz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gcjidoysr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gddqzrhgo.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gbswzmrfx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gjsfwglkp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gbdhjikyo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gwsjykyqs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gvoajwjyi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gsdoijfmm.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/giszyjngy.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/grcgfvrhw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gzsdtlibv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gschwpxeu.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gyucxrpdk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gicexgthd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/goovxmmrg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gjayoyppl.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gsjhnriry.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gggmbkoxi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gmrgxussv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gblanfmqk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gfhihrzgp.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gqxrccnzm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gyxoyublp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gtbrpicgj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gtykejcug.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsdebjovn.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gyyijzvia.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gmetwfzsf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/ghkktqsqc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gpdleoxvr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gmvfjyfic.sHtML


<!-- 参考信息 -->