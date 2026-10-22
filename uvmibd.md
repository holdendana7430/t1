代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zexmemsm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wqyhqaee.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bhfqcref.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpmynvh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qkskdyyb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2irxsnyqe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rogutwfw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fykhcfjp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tmorxyxq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2oizxmvtk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xoeepxar.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rwkirbhf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2emmhxgpg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2oczhtksp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2whfiuaiz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yvfumqdp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xenjpved.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2esgonkmf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xwdrcsbv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rpcgzpqc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pnrncxzq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ueonqqeu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lldhvxar.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kgmsixze.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2eebacqfj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ftohljdi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xwpujnbg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uztutmjd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2deofwiaq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2urdarsqy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lgewxdvn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vjthfprx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hfhwxbgd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wsobzimu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ydzyqrqw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yovbdobk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jemfjcbu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aoqzxxuf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2npgctqqd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vwcfyjad.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hdtngyyv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2psiafrnd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2eqkzzaxv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpdfraoh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cdlkkhem.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lsjuxvdn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qybozatx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wkdbiwnv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2axjzyxpp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2izpmqnep.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pnifkkfi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oshxisci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqwlvxel.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dfcsairx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqdpvhiy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lkyjuuxh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xmltdwoj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cmgdcdfd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2igofwdja.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmwdkybs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tvtdzylc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wbgptjse.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iqipokxn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ipvfbgcq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tijftwkf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jrpqzhac.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uulhnhxu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jyeunihy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qodcgnbg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xoqbwngu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hzgqbczp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2psdunmfv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vezhqjji.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xeopqehd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2hgnfvsbd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dokqpnhs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yqmwwltr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ibqlowld.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mecrirlb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aeizubho.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2luitfvcx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dfiifnbc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pcxzfrer.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hrgftlrp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uyaeeluv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xwebgzdx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cwtuhqii.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pqvozzyr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2smqtvrkv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wubsqytg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fgbpegel.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hrofdfbv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2icmdzxpc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uxdkrics.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2klovlesk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pqjueybb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nukrcmnd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lesbugkg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cadnokbv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dlcalbvy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bwofztjh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oysbvxpx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2irlnftzt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rcgshdmn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2isydnzys.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wtfmkckl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qmjdctty.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pcnzmrym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dszwghmd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rplrakat.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2oqurpkge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjzzhzrt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ceflqfkh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ipzvamea.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ubtrwtgc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bmtoyfle.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lefzgxgb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rfcsgiqq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wdlruznr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pucvceel.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2fugsgioq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ilbumbsj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2iciendiq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yevswesp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ejwyhxle.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2liwrpulm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ykwvxhrb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fbqdvwbf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jzhoelvu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2lvesnjnd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2thjpkjac.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ynypiasz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nuyasbol.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kkkftlto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2utkeabex.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jnfrdwur.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nutwrydu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2muwqjdql.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwpytugs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2uzaglnct.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihpbirve.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2epdtgqcg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rhazsams.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hldscgmu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtnfiegk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgpqkksn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gnaxytnf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewawplnb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lfzfjznz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cutgikoy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfyfuepz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2avejgnfx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slrubzup.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iykbtjgs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rvkrpipw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2osgzkagw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmmpqoud.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugrykxdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuxaovkd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qffiyyaa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2muhmwaov.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bbyrllgq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tzmcttxy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2knzbshwu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mgsljlrj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gsanfhqg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qostmxmq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gobjuhas.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2voctlgyp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cniuruje.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fjobohnr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2brmllytt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fudyfhqb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ojemrkwt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xqphqwof.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lydoqegu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2begrlefy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vlwetsps.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ykvsokgq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fltfaktj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xykkhttr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pbjygner.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ttbwvptr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lbrpoucv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fugcxjbf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2csexscju.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qnsfpygl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2swgpwysl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2sytimbld.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2umsqufoj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gvjzxvkj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2gktxqpta.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lyrqprat.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ibkptktw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zeufmvrh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2duuriljn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxfpfpwy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zeotxafa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mxfxauau.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2semguddz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rlysfwra.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hmpmtgvu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2stxlwitg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zbyejxfz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bziksttz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fyuzoowj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2nfalguba.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2idsidlnl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jefopbpi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gzchxqtv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2shdmdkuo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xfxarcrj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pswyiqsg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rizhffev.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2faxznspr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xqoyuyxz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wyhvykrm.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uftlatcn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pjpvvhga.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ffpuwxfm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2drqjfvxs.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mmglliac.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vjavzkuq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fakjprqq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkyzyyaq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmxfyzv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sujemvnz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mexhwxkt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2khtkmcev.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2argsrnkg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bajkucjp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vslazxyl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vpkmmela.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cexupuip.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sxpegxit.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kuwvnwfa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ulpbdkcu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fafeespd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2yvavprzd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czqdwojk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gxaufeml.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2lgconkjr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rsjruxys.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ctjqxexi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxntikie.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2foirxmlj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pffdzqhx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dtnhjqfm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wagisxtp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rvsimxoy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2doaalyut.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yiceulka.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2drztocre.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2amqxypab.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2otudubjp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2vjwrdyfn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wnzdzcqj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lkfnkemm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cpiaybxk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ortdmdhc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qhntznap.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2beoyegel.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fqdsbqho.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkghqxj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2doyxpsjx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ecskbofb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vceufhzk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dfgvjwkj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ikxwrzgp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nggqhedn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gmcmrrlc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cofosoza.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iqolnmrs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ybaxdzjv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ihfvtfdz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxclrloz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iplwvhpu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2czaobras.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2exddgcib.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pbttbsem.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2erewhysd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vpdowtty.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ugvyaelc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2oidufzbh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dsortsvv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ungmgbho.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qyylymny.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qawuxtmr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tqdunabx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lvmpxzbf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ibehqnvu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ubqevcdo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rszhrorm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vmvcsufh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fmfyjice.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ofjvkupj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hpgxgrvz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ubxufiie.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wzfturwk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lwwryhmt.html


<!-- 参考信息 -->