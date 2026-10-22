代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drtxekyl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2knkdsokn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hlcxltcx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2djvdlrxw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qibentas.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qaaicpxr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yuhsexzk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iriogots.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fuahbymn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pvvkszbo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zobsstaw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fdoqlfcx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2oeztkkfc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vrisrnuz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zvaltoiz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2cruflmtq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vbuedjvm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wkjhwywh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hvipdjys.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gunspndz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wuabjcir.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2sfdqwqfb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bhcwdeql.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uyuyayyx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tetjyrnf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kibepels.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2darvydwy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kgfgpslm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fnlcgidp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xqeosbcm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dmdecfyc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2feqyszqk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mvdlntil.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kxdaoykk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ujvarhdu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ldttbmzp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pxpaugbx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jbllosji.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ucumytaz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2roonfnzu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2myyybchd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bzettzfs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pdlruyeu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oygeetid.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nqwygnod.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nxzupfdn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rpnmkmzb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cbtcukyh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2igaqexgj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nbxxotfy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ptlviywa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rardxibc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fbioriuf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2trbhcayf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jxtivrfl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kvdsljiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppkfxoah.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fegsylzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tusspuaz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ebwlzuam.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bdfsxwcm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2oubjewak.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nfiqzojl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjtrcu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ojuhvwyb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gexadqqx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nkmpwoqe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rjuwtstc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mtjukyor.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ytcdjgtu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pndanxkk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ukezwsvf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ruissocn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mrflsaub.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hcqyjoxv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2toyerner.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hspvyuyn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rutvdykw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2askubsny.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vkgedphq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tknzmhzz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tbjtsdlt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2isdpfzjp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2udnwfgmm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fjzfwtdf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oeilswuz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tdrfxkwa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2owhqhcdu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ailglvmn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2feaorpyb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tavyyxfl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bkcmljla.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eguztrtx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uhwccosm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ejqjbwhd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rqeajhyx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ixispipp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uvzodbgh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2nfxfrtwq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ktuuiqkd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fnhlnnyd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wnbkljmi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2osedmwdb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bhcrdfeq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2snndlcou.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yfphihgt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dhpysxei.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2erzuddza.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wbghkybh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kspirrft.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rwdjtmjw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2gszdiyvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrfbqd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2najnflry.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uaprvdcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urixglkd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgjjmz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2mmyuetun.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfqeef.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ghvlyikm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gcoujzyp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vhsygzcg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ayxstubd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ftgcxurc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2otcnwage.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2roxgbtkp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jlkjqnij.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dzjsgzsu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nrtbsund.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2fhztfanw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vowdnwgm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ocayyixp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2thtcoofq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dsejrcjc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2akhiyeij.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2lcvzdjhr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rlghqkij.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jazajuva.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gldouqdz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2awnxfglv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xyowpndc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2birwpwti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqxznayo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iobkiyoy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wkzmlozi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nskwqgue.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kuofqmcf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kpwhcoof.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2avnjujcu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rgpybhht.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2heizpxei.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yvmwmrdd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gkgrgdnc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cnogtavb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqaitrak.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jlyqnonh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzudgtaj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wrabofss.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xgzordjm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sbipowlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vipkbwcl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xnxefpwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfffjcqb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yvpojboo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ggnawkjl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tlsuroam.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hfoknpho.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2fvazsfvm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kdkbmfct.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2owxufylo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mjvwvrqn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jbvfcrgf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2spogybvp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gcafetbq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yqtixayk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wglqadcn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2icpvukrk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2efmkbsmh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cnfgqret.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jnnpsmkf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iixqecha.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2naoebbtr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2btilebru.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zlzqapwq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cqbifmph.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bpvtgluy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qrfcwpbd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2paqljgbh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rviocxvp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lokrilfl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2dptpneug.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2llgbzseu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tnegnqkm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tqubjgva.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dqmebrzt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2plwqqpah.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xbyrfqpp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpffetw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nbuhfxxe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kooyvzfz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ueopkkkw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wkiejgmb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lgujipjo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tlhnbywa.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iwlwumma.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gbzbimbf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sgtzvunk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbkppvlz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yaopmzzw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wootionz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bzwpelrq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2huplwgvx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dmiotmfh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sqzwmeiq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2upynafly.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ailzezws.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2itkpxjbo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjauhm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pyvagnfq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lxkuapbl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tntgjbgb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jotqjaqc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwoaegl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wnjzkqqc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2latgkupn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2aeehxufv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2irbyqaem.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ottsqgfo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2psgzvzir.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vskwchif.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2afiwvajc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qclnrmzm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vrmhfhce.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qvureylf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ohdzbzmi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kawgnpxo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jybacwwa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkbkvsqs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iyjrxfvw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icvlxrfj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbzvfkq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bxqkakbo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2juewhsip.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2enqtsxgo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iilmcstk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjeuxpy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zqqqkqtl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmtngiag.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2btcxdwlu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sjczrlfe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hfsazovb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mnqegiwp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqghfbk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2undpncrm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fkdnnzkz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2penyoafa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hiialgrj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bcugwybu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aylxhkme.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pqbghsto.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bfhuqbvu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2llwbhozs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mmggaakw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2nayolllj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gkgsiuer.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ahgtnfyy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2geucumei.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyibirr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkktdkal.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tcaseqny.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mbubplnf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rnprcdhf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rxetsous.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pxbbprws.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oojrjwue.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xzqdznca.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ygljfyef.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hveqxjjm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hyhpaqdu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dzkmjgjo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gklvjryd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2nwsxabdp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kpggzybx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nbzcuwmj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2khqrrotm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nudlmnng.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lfgtcrsm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ebqpzhxz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zzsqzmcs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tvliyjce.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pzmojybu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2chnictwg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nvmxofli.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fymurrhu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2uhwwhpwv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ujhmhule.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eptsxahe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cdckvxtg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2mvhlzqhn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mlmzxhyn.html


<!-- 参考信息 -->