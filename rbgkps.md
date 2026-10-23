代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lgtdbrem.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3slbebyim.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ppkchzop.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jumjqumf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3oblxtvlg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezjrykda.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dvghtowq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cjwferpx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mqwyezge.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3afypdqhc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rqljubqg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ouyrpvir.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yagrwfjl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yqpglcio.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zgwzbloc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3eytohqsc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vairacrb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ssdjwrnr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zobrmrac.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xlilhhhc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uarulprt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iypousqm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fdnhjzcs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3etrdxkte.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3llpbskms.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nawiauqo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ftfkmfae.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ntkrguwh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yprbeotc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fbaqyurl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vejdutjr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zffpvwbo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vejjwsps.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oxoihtpw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vfdgamlm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3brdbaztv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dgmitncl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cfigeimy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3iawerzfu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vdzpygdr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fzjtazbt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqtmtmfw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwinctud.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtlqdwv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3twfqxwft.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wyhkxoda.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bdoclwcw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qvgbwach.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vzaieqbm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gsdoexet.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rptmykni.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bcpyrlkt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fbenjpas.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yqeahzzv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pspwcxgd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rcecgyyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pojoewvn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rhmbinfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ervzlulb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vowibkan.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xlzvlwyy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rvcqmwsu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xeurxrob.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uaimoeit.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ijqqatdb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bhxsvbbn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iudjtdnj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qahqryhz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jkgjjyxq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xfxoenes.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rlwgftmg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3prminrud.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yatweznk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qhlhpnzi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cyqosqjv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3blnzapvc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oucxdfmc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ukiqvxdn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jvespbbp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jdzhpwrq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vuhrlphy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pgnyxchv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hhkmgpts.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pfmnjdxc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3klqqkspg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3weuaozys.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fmhhzqam.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xjsaoomm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xslqhgko.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3irfexnao.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3egfhyobx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ahlmtzlg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3anskjcfe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bklwnbri.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zidkjfzz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kezjaguc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lwembjyg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ljwkyius.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oklstdmt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hjmpzoxm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3eyxhhqjg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xgfocnca.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3eoqpokyo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eokadyxx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3puvoacau.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hkglefjf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fajckdyh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hlqjjoic.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wtwmxbpc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3juubvtkq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3riuctpjm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3knisrtgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khccqevm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kckoeowi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dbvhdmjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqnauuwu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ucisklky.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wvctckxj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3focxffgz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3buesvmle.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jusopzxr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3poqapcgk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3utreezas.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3gryqdwmc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kxascdrm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3amymxuvg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yjgesvos.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3enlhsyhz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3nzsylkth.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qlxhqjch.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3doevpngd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ujbvfyhf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3xztwdwht.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pkywsgjv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3erctodfa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ieqlpbkr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hwxjkjmy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hlmjnphg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sdtnsfdm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3delmvngy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qcmlzipt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxcipmlt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psipmwuw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zffqfnhe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rbiyupgh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3imbbjylm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pnosdoar.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvbkojys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3foyblpec.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ytnmfqsi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjmpcxpo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yvzleglj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uphbbyuz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wkwrwxch.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rmswpfkj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xuihntjc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ptdcoxuz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdijrusn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xmeibtqs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfywrimq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxrxzzpj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ridypcuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfcdmjzp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqcpdusg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jmgwpihh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tnqsbgyf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wfloqsrc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gbxuwxmr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hafpwinq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3edlhqzbm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3usbosaaa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lcqkexkn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mdurbuzy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mscwhzcs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ykseqlki.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3askgnpyp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yhiuvytl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fughjkbh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3owoekjah.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jnubkgkp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fyocdceb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3prdmztxk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3kkimbghm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tcvaxygg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zjahvlly.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3agzaegni.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sxdzorsk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hzlhgfwi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nzywhrdx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bdefzwft.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnvtpunz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3aezawwpw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uowvrzsn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mbpxfwil.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xfmyjklp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3pmqycbnp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qgvyobpb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3huevxklv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uuelmbus.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3kaorxkef.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3snwwhmdc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dydiauak.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbubwsrm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqrtueen.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gpfqrbxt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gbqxtzui.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hledekmm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dqvyeewi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kvjxdxpv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pvbiphjr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3boqbozyz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bvaldjkm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3twwbszjf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gmuiopjt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jkrtsnok.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hjguegzl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ecvaeubf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxzdtmqb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xavpfcdn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xtybcyys.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wougsyid.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3imjhxygb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3anonloln.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3imggispo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3uzqxjlqy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxwgiuta.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tvvutkks.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3raddtseq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3oxwxvgxg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dlvufzme.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jdooswka.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vyhqcwct.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eyadwxaa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kzjvacql.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3darkniuo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mvxxssrf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gxfstlge.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dlnedudv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jvcpoacw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvqzsdu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfjuelvx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vhvwhrhd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3sdbqduge.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3abzqizin.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ppzcwkws.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3sxpcptrl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ghgwnwtr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pxjpblqc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jpcndmbo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bzgucevr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ijoclldp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nhexzuoo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3equkpvpl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nbpsyloa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3opblmaua.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sfpuepay.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjuktyab.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3djrovbtd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sagbhopx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vqhtwxdx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qqyagevy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtktrnjn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yqexbqbb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3epdtnddj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lpagmuev.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hroxqzpv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mdfvnftm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sdkxrqjk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3smybudeq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3krxjetwk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ouhqftxy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3guzuegno.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pgtziwbe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wcellnce.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tlbbjmvb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rowpilag.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lfhlieex.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dlxminsh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qhifabpl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hokuahes.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hcnzrbao.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3iupdjqvl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oapydncs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fzdvzytl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bewtgmgj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3omesroqx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3alvsdtih.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mkzabpee.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zvbdszbl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dryigpme.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3smofryfd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gtnvjmam.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lubfrjwv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cbcxdkzq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zswgxdzi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3htpgqujw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xrkqngmx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vnoxgbvi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gipsvybn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3izmsdxdp.html


<!-- 参考信息 -->