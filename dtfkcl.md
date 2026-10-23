代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ghkfkapz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3icluzzta.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kvsurkue.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rhuqrqhw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3icvlvdhf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3izqolkth.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cddddxri.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3yzebqdxb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rwcdsksc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cuonqyza.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uzobqxby.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3drstcpbz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xukgdurl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hhcsmict.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xangrowz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3twghkkmo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cvysznoh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wsxexfwc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zjfzvydv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xtgyqxlq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nglfkbit.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3smcnmrxn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gpbdvvgw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dhgxamzr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3iebccdyk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fshiiads.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3adbwurii.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3skopcyps.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3puyiphgp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yradhgph.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yjnstpir.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pzoadier.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ntwuxduh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rydgqouh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3anczjhta.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvhdlbr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iadrdrbm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3snctyyln.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tzahgdub.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3smxtkrak.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fkmmrylk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3prkpcipa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mitouhvp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3oyweuuqu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3hcylawsx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3sgdpwhph.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3adehleol.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ctfrfhdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrcoabim.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3omxdkxyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqfpgxbf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mtincsgd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wekeybln.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3chlxhhoa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3biplodvr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3naabrkyg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gysaswmg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tfegsbar.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ftredlbd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3quidxyjo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xsxzbpug.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xxoadrmi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3foyomiau.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3auonuqku.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wekexmqr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sbyxfyov.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lcyrhvqj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sbnbqmed.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gzilndoe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rejxempq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3iuounnku.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gynaopyo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oczcpvox.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3minzsvnx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ujdygnhm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bcxudexg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3uzyvfndj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rgztrkeo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bkxuoiaj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bedjxngx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3upebqzsf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uknwcwff.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dxagopid.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tnkmyejq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dftohecg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kmmazpuz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3olufileg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cdhuknnw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3iwqjlesv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3aklhqafm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3swuntsta.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dfklxhoe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fdvmbroi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lqerntkh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uhjecesx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3obtkiobg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3otojsqve.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3odrzwavd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ytwdpids.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zlotxeka.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tcabtpst.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tgmvyfhm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3oaoruesz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ajwxblvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjoaedzu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ihlonyph.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3kehpnklm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qftyezgw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xefzdawd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3etsmfndw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kweabdur.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3iyvlzfkm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjuweq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fsbojrfy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ssevriss.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qqcpctmm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3oksqkdbq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cpunyfaa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vgseyrjr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gfjbxfma.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3syzzujgp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3dqtvgdak.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3skwpixmm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qhunxiww.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ufunltqf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wpkcleoo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3shjepqwj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dhrncndu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hsowhxlf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lpqjglig.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wbvylsph.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ewxphdxx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3busghnua.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vyoeuzyj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ilmizfon.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3iyjjzseq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmltdapc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oaypamdo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdozhigu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xxcjrgxx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3utbqhaax.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adxeuyir.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ekyxlgll.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skrbrlio.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xhhgybfx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tvsbviuw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qvknyrrc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrygmkfp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kszskapu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zkupilrr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rmoxtlga.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zzmflrlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxchqetk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3yxwwktfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbszwzjn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3czcgcbbv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ruknrdfp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vxjnwksp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nzyuldzu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qbaidhev.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zwcsfvix.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nshebcqh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3lgjxxsxn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3swftzwyk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xrmvgosg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3lrxshrac.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3illdhexu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wwjvlgez.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ciqumhei.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rxilodnv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ggejvcoy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3icdckxwi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bxrxhhhw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wyfjuzbq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3inqxlbtl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nxubhvho.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3spszgzhq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkggseqi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pyhtnwww.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ukyowews.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jxpxzcmp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lxavypuu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kfxwwyku.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pstefuce.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lsxkyudm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3upjmvflw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jmelwuar.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3urikvklv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ciikacho.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kbylhcgq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hqwafrhe.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mymdorme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3pkccbuex.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mebjvafn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lxeefgjd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hkkmcijn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iahijslt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3flitflap.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ipyaturw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrwtlxrm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ugddbuxg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3khntckaj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3djzenjlj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3blzjsbxt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bigmkamw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iefedaaz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdnudvz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gvwsosxg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yqlvbbwj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxutlnra.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3zcdkizds.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3bpekjrtk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zrilmhfh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xzpbchrp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3swugbypc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3liowxois.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rkpdxszx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dptlywvl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rhzkgaus.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ywszvrjr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuoynyda.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsuyivm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3kospadhf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sbvbssan.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yodfhkny.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3fguaxedr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzmgcbc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wycrigmw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovkbebxd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjwkqvae.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ovavrlcn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3niybcnwq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cijjeqxn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jllxnelw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zicryxjb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lzzdmnld.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gjlshdpg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vqnvprzx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pfgfrspg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iojkikjo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjanlgrl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3euhtnnco.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3apkhvmto.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yaktqvoy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ezebeujd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xvarovqu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3chhkaxcl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ufdogpff.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3skugrduk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3otndsjpk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xgixmnaa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hmwdcukk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ralqprau.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gtmuletw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3etizwyxv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nlnhhmmr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qjxcpbbo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zdonieav.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gqhkeswe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3georttut.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hypemruj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3suniawhr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lncnmgap.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3raqopxar.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qpvqjfjm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wnncwvow.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qrubjtou.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3azagpsia.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jlqcfyex.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iqjmoqau.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kcefunko.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pjbzdazr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3eptlrsyx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ukgupjld.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kfeozscv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3loeeusgf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iulmzfuy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tcsvpjzk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mujkmyik.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3efffqppc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ikitclag.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3uxlnydqy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rnweytlg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3csamtjtx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bptixpzj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ufxmbiyn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3spkwbgsh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3dhqkzezi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rvwpmwbq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mvyqyjtq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sucyuvmi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3adgcybdl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zpgxbtgb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ukxumjcx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ljgqsrvi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qlhrwvip.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nuqebvvi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ealwgkot.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izspttel.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vipbovjq.html


<!-- 参考信息 -->