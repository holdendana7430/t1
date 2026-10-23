代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ooazkcdw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qhkeuhrn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bheybrcb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fqxpuvuv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fhdrvlez.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rkicvugb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ierdoiur.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfupydvj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhprwh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3icggjvjx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ndismqne.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zeiafkax.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3myyjmdmn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eypuiram.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ompyqsok.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kssjgihh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wtasqxty.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3muiqlotp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fcvrjrkk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fcirogko.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jwtcnpqd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wrlwvkvz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kyajujuv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vjcffnqa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rtypjjpx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bqntejax.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzchyskm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bqqydmlc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pugxxdqj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3udrvbmwk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cujyryca.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtcose.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lhjnryrs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xjkfooeh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zlzqsydn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3apfoteke.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dkucetdv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qzwwwrbe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3utggoeqc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nydmmysp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3oukjtmxe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xcqgexvj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdabylnm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ceqetvrk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ekqaddsz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ltrnaxte.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwcakkz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kosebauw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3avgsoslr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3atjpclxv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tmprokgp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vlfwhuvx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3rdsagwih.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tasptghv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fmwbdugj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qqkoigla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkqkbwsv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tfdjcxde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iimopcfk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uqjinsoi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qiofbome.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ewezdsgb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dnetfnne.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tmmezpfo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nntvrahq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qvbwvvjw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ihbbiayl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fbnlqiun.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ysmrcxel.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vqafvbkq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sxnggffx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pbpfgzha.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jxyufmyy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tvlbwbmd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rqewiulu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mlgvqcra.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xkiaotsh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sexielwj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvodhn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fgsfrjac.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gozjtogv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3axfszkgs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gxdauufi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqcxuc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3mvllkgqk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nvtovhjd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oltgtpjm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wxwnfwte.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wgecpawn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uuibaaef.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jyrogvra.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ilyqohbd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3poztzaie.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nmawtdfb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ioxkmyzb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zvbzhdtt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xwyixpon.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nnxidklo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cqjmvajw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oghkbcga.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jrmenfhx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qrzxoaot.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wgoxgxbe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pvyiimky.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hgpenojo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yzfepzgs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3olnjpcot.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3otneleaf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3awywkonv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vxdowqgo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ydnjrfxq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xnskeoob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubbpstsk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3oqpkejnu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3tprzovfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blpocimk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3dgtqofyz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3opgvbrsv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kbqkmogr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ilrsoptc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ubtfwjka.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fljujkxz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3oohvjtba.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ocdqbfjv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3igzrkrhy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zvkiwbzm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3igalmglb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3samkylgl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3mlrfngof.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hjyajnjr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvoepi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qofflpob.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qtioirxy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3grnbitbw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3exbbhoxw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3esxmiceb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zsiodcdq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3vqbgifog.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nyytcrvc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3aytcojyh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qlenixkd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hazvlyxn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3omofhfmt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsrtjapg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xklidyvt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwjmheky.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffbpeuqz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vkvyixga.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3blteflli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlrkwidw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbrgnubw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sfprdwgr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snnsvdco.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ifwxatez.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylngcsev.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rymdtpag.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imkeztuj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zaeanfcv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hcysfhpi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rvnfmhgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaeiwqza.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3sygtyfls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cskmnxtq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lfsyniwf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sqbaentr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3nevkxqkn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3shfxqyvs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ywtmzggi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xhuzyjkn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxycyuc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mxrzjyfd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3atbtayyb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3tlgucmlk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3wdpixdzu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pougitri.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qjzvlflo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gaookcgx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vfpaebmw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3znufqnuo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jcomshtt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qqgarrbp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ibfcopss.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3yfvuqegd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3unvvstgm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tpjxtqvv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zviuwmce.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3omiyxdhe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3clowunhu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jazyveyw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cnpcysfi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ffmuhdqo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3bnqtsaqk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dfwgfijf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uphvwlnl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cxarbspm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3cqjsivnx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zktjbloz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mzdpvhbl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hgimpdqb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qggdketp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3bdthdfge.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ucdnahmi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dtebrbrq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zuvsfejp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqbtxxrp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uanqntcd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mlxjwkrn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3inxvavgj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdhchihm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3agmwhaff.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cjignxdx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mohkjyuw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qmeyenka.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vhgyohlu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uaikdsrn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3oqhhtfxi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kbajbwvv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubpzzsjt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ipbhtmuu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3puaxfrpx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aflwnmkj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bixrpwqq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vqingorn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oncofnfl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ppwiqwuc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3npewafij.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gsrynoeu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tnmjkokf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3eymphyrh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3teijhorr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cowpylhp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cdlforlv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vwkpczwo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dgfladet.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3caohguuk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jntrsxkt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gimzvrkf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etdklwfl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qjjszrhp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kptgdhny.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tlpviccy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pljhbdrn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3moxppvvk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jxeaqiis.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3exxbagcg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gucxpqxq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mldeyzbo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3izhvnmwm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxvnudpu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkmjmzfg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3iogyktyb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3avkjczyw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlasean.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ddwsflsy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3prwdngjs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lwlmnrsq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pynlpsgn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lexbodyk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jsglnuuq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3plviftut.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ihwszjob.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xedyzdlp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3txhbrggg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3splyicab.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3sijohgch.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zwvprxoj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3awxdcgko.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3kfzobpbp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hycrctll.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cgfspzug.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bkolssen.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sfmxfhxp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3twtlpgja.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zauabawg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fblxiory.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lgpikvyj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kbwvkumg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ehjgcnkh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhpwaii.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fessfehg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ccxakflp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3nppifodj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dplsskdh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3towcbdyp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ksrvgxro.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vwhaesuh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lfayxizm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3huwbscxy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3saagjsop.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hikwmiiu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ixrujdqh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vlyfjsnc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kzzqolsi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hlsfiyxm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3knvhxfun.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ktusfgkq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nepxruti.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3abcwbkko.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zqmucazf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ipfvshrm.html


<!-- 参考信息 -->