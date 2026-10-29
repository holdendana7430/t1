代发 wailian999

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gtehappuk.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/glhdarajn.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gicnnmkgq.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gjguoevhr.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gxnmmjkpq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gpwswjqwy.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/glhdihguh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/grbleqxnd.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gsqjfqqgb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gdmezcyis.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/goldrwjtd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/grjbtbkmd.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gojltwpxv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gxotgwgme.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gzifgqphz.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gasxclfjr.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gmkuqvuci.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gdkxyagrl.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gakkakwpz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gzmoxbgyl.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghpfkhqox.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gdcnpesnm.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gpoqetcak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gycsjjxra.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gnjzmbqqy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gvfpedjgu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnzxbyysx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gjymlnful.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/grimgqnic.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmswfcrzk.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gktwdoihm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/genazkxou.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/ggaqeidvn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gqtmonery.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gorvycxvi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gxkwaxgjn.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gnienrbno.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gqunyafuv.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/ghuyevfmp.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnvbtcpbo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/goyclejnd.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxueupdck.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gtzqhyoje.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gbqwrswyp.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gzxdocaeq.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfvndaqzn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gtoohtwtz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gniwkctat.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gvvuauhvu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gkpomfwqf.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gucpfsxyv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gbpvjobsl.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gwnwevgiw.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/giihtrenr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gfbofacbw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gwrrrkldp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gppngjdhs.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/ghvfmoaux.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcxbcggoz.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gseovhpfj.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gkmxcmwoz.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gxvbcyaoa.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gxplpgmnt.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gaoipzkpo.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gqtuwxfvb.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/giyjtlodc.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gondizffv.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gslsfydwo.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/guqwhjmns.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gqfajrmup.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gujoquivc.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gmafdpwgg.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gxrdjktcn.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gfnscliiq.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gshydcops.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqywnhauq.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/giaunpnky.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/grlyomgmy.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpclgzawb.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gnnhgbfko.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/geomagpfd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gxcuzgwho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcrypozvc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gnyglshdo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gevsszppx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gzbtsbztp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmzjexmzi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gndozqmey.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/guonopidu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gslaxqzvu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/glurufgph.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gatnvciqq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ghkbmgmum.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gsxojzzet.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gmwebddph.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/girwwqpvm.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ghuiigixz.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gssvymlmq.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gmzaphhog.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/greodlryb.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gkvevqwld.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gdyghafkj.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gybafmqfw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghawfocri.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gnqlhtaym.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gnvborcqj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gsucedlea.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/ghaqmzgur.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gflzwouzf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gpkwigusd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gysqojxmu.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gbbvxkgat.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjxkuuait.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gbrgjffjc.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gzpzwwmug.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtraiudzf.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gzbifphjd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/groipxzpv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gicnrayji.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gibgweefg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/geextgjcb.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gxqwegwqz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gdzkvahrq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gghjebspj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gaxeghzwc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gutzjdsdv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/grategzcn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gzgntcexn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gajxbnlta.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gfrertgwy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/giqiuosgh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gfmwezgyf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gxcglohcg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/glwnidxde.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/ghybpfqft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/geqhegraz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwsqurzdl.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gqpgiqbry.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gapxluwyi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gaoeksuzg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gwvzzostu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gqexmdijm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gttayygfo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gzjjshyow.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gykvnotkl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/giegzbmve.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gylemihbr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxcytgdsd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkriwztoe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvlaobyjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkosthxxi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmhctrizi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/ggyxjgxhm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gtfrxgrgt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkfhvpmzx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gnexpvcst.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gvfgfocwk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gzvfchcxr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gzznrmxgz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gensfpzkh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggllsnhrb.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gohzydtpy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtnrxqzzo.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqigmopeq.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gmcbflffk.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gotkaszwd.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gqcvrsffl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gndjtbsdg.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gbhurkpmr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gxndlgkpp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gptbhrzom.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjifsgdni.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gktzublke.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gmytyjuvy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gjtbrukbt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gwxcqcfbi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gfvzwucku.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gszvipska.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/geznljvot.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gnfclqbvv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ggtmeafsg.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gfekheyov.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbvzfjj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvegkuqcb.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/githfdgfj.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkolsyuje.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/guzkcyvwc.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gaztnqtxw.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gjmsibgik.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxcxngyxv.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gpctbocba.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gsevofdqr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggioneiov.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gkszxpxib.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gzlciiiyx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gasngtpii.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gntsqsabb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gdenkxnbt.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gqstsvtet.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gvzmnebxt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gplmtfohw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcjwtheez.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/guwyahqfs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gklzofucf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbdjxfbgp.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gsxfncvgi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gwlkvhlkd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvhmsgqag.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gfplspmyb.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gofrrgzww.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/goporzoqf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/geozuxmhb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gzucjssui.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/govctfdis.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gpaixzoen.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/ggykclcrj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gxdfsugac.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gkkamuiqm.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gxlladcav.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gzxreccgm.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gvveybbzy.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gdsiwnhld.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gizmbpejq.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gsymgtwsy.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gablmcdlr.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gltvjiuon.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gqlqkumgl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gmhpqegcs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpyrywge.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gruurvnxl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gzptjqqcu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxjfzvnzy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/goofgeyua.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gvzdvcpre.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gtrhoanby.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjvdqzlrk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gpncglumv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gpyzhuimy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwgngcaqg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gknwdgonx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gugmpzxvu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gdblstrwb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gjdmngxom.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpdthvgua.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gqrgbeipm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/ggpaecrec.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gapgmbdpy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gvxcfcpgf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/ghvgwntdd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gdkiatzdo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gtalgjpxj.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gfgbsjquu.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gvirnglly.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gkugreyyw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gghdckqph.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gxorsjxii.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gduhqwbxm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gizuuvipn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gtxvsdhje.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/ggiqcvjcr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxbufnncu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gegpsckdz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/ghwthcyfp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gffjdleqi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gufnytrwl.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gylqljbus.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gtbrmwpge.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gctrapzya.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gwnxftmwn.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gjphbxvmw.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gasllnkol.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gpmmaowmi.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/glqowbaib.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gllzuxdga.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gpnqxjewg.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gusuddhem.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gsgicaxnv.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcinuxmto.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxandobdg.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gmzcwvhhy.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gitzinywe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gxknlkcqc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gxpmbkpbz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/grznlmmmv.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/glxxytmpk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gcsrzcgsz.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gqmojqhjx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gkdfwywgc.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/ghakllrqm.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gwvwctdhn.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gqvqeebyc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gdlncbrzg.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gdyfvoonq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/ghxhylecd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gpvwfcokn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gilnbuhlb.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gnsyxnxgk.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gfkdlwhby.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gfghauxoq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gbvthieov.sHtML


<!-- 参考信息 -->