代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lnaarmaz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pqzhshkw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2djsyavwo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rfbcdxrr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nhyfnuqt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xbhmdiku.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qqehfbrs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbgqquho.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xwzmoicc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nvqwpnks.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ablfmopr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xwxrlibd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2klvwlniw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zwrwwwnb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qrbttluy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dqxewees.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ldrljozb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lqytxhjj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2etrliett.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zdpgdkef.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2gzleyanp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mdvtwhxj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jpbkayuy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hdelhvxn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rrjvnldo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sgyhkbyi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vedkphur.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2epwtwcpo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xiwjwzuz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2imwjcgbq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gqkmcxcb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vkqfampg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jxeikrtc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oswzimfl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pasbytsk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zuqqgffx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2idpyivmf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bohvxjuv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2agzzovnx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2umreljuj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jtriqqmq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gpxpamsp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dlbrzumq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqlfvsc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sgabxmtu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bbcurbnk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2voucqbag.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2figuevdf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2coqrpyoj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cbxehgfq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qfkcxwbn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wcmyrnrr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yyunkczl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dsiecbfl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2cdbghwnb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ulzitfpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgzrwagt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wjsrkkym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awcmxpyn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vbkjdukp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vwziaccw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2eqwvblgo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yizxwtol.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ycpsyxbn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2shqvrscc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dzxvggqi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jeewmwwl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lkmyieai.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2svzrfcjf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2urslmvsn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qkgkkpij.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jpckjxrm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fzzcmmai.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hzngjfsv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lkahxdge.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rywkxuaj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lokgqxla.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lsjurygc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2repmtgsn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ahcbpxza.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lbmkmglj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lxxspgyr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mkddizoo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vcajhyiq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2iulymtiv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fhtzmoml.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hbogvmbw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uymeflzl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fdvnwwsj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2didotsqh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dsbhtuvy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lpyicqzo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2anfebhug.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yxzuxxzh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qbpahfgi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqiodc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2eshgapci.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vrrtoznq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kqlrgmvh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zvtjkycs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2snmkwhjf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bjtgtbxo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rizvbqrj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uzzxckku.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2juueulko.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jarlzgxi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pounzhmz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xvhogiet.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2mtaraxqj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2oqstaudw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2eqmlxrea.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lcqqoapk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfgfcpoi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tdjuvooa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xqhywudq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woibbzko.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nymeeeae.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kgfcljqq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qrfjujca.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2sucvlmyq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ehramxxc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2djcbeozq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2eycyadvc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2cglciikx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2cmakmetk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hyxdxjkr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2sdsqnqpx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ctoclkll.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nsvukcei.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kbztcsez.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bqczgqic.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qjdiqvst.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qqthwpbl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2psmbkdfh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2hhkjysyr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kilbcjlw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lcejfzpk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ffyfihfy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tghkubxm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dtiqutuo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wgisbich.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uuoovjlx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tdibaato.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ivqdmpgo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2egkdctio.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dpdlqjoh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gonwnecy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zyhofiju.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nslpmbml.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2afbhkday.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hziiavjo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxbqevlu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rcwvkerq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dmeaojyl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jzyhezfj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbldzcwr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hkgldanu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txqzjduk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ipozrkeb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfcimkid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhizghit.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ypfmikqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftgxlqsk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxftxmlj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wsxvfnnk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2haiqfctq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wiuxgtzv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2phdxassz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dxgylaje.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2edogvzgl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2flkranqj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mheeprby.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2buekvhjt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uynkfzxo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xtlvizik.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yqndyxza.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aiobhfap.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hnoylskc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ekpydcam.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2giqlbjpj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rgjppaot.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2crifmphl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xoxwswck.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2maiycuie.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dbakldbx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wksqgovm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wubidktu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zqpwidzm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ywehqgvh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yftvfyxh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2sxfcqevy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfoijua.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zvidzlcz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mjangqfo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hrrpkouj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hywfmwre.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yrwtwjod.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2txkjjdrz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2uxfaccoh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2qmkcnaqa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bfcahtmb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vduxsuwn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qxijkvdt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lwmnfhqz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ajsxzcle.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wulvywhk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2axuhuyud.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bxylierq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yfkpzxwt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gjjvhxsc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fslgaizu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iunseimd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ndodqbvl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yvxfudng.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2istmespz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2erielvjr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qznxnjkg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usunyknt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bdoyywhq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lvqjnabe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wxvocene.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zuxvzafr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2edgtiokf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gmjhkkdu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bmhzgzlj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gibekgbm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fsgdozxl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgervtm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yayxkbjw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wouchzxj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2huuiupep.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vzcxvrdn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cfanekee.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nznsdvhj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjtkshu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2otyyumoo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnduyhur.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cavsdnlb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cyueegms.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dipbpnss.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iujbqive.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2iqtlfyeo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xyporeka.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cmevkami.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xfgttnne.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yryxrdzm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dlrvuubc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rlqvobjy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2onsbdikw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfkhfdaw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2sxmjpjel.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lolmmmbd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqjsinb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gjhdvkll.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wfadzjkh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ouoqxxzi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2maleoufh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zjncmxim.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hkhpbmym.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2mxohmfac.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oiuuiant.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uxsjkipd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ezjevcdy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjvjlkmg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gfhwqxhw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ylposlfr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bkviqsxy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rugfdwnn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2dbpiswbw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mjidvnei.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dngtvvsw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ywfixnsz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cznjdpsq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2evhxxpta.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oswwzgtx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2isotnzqx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xcvwqoiq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fefwocla.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2isuofghv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fxwpkseu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jmlitoup.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2owoejisc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bbbijjzy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bmgxmqkh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cbpnshwg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2amvafohl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fjwynwwn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vbphgnxo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eedklkxa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cgaipcir.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jmtudmsa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ldgrfktp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oofeuoez.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ycrhjpng.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xknqpjxm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2knklsaip.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2baaxivnh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xtcewlct.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2byfwdqei.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xocldait.html


<!-- 参考信息 -->