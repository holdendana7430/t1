代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kgxzfowq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pgilojvz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uuowfeiw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cjmortud.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hpfzerfm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vvdzomil.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3seuolesy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kkhsulii.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aummzyyr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xuulheph.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3sbekrnic.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpexezed.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vuekbeki.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fdvuuldy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xatyaeox.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fqznkfpk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ueucnjzs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3msucrpsr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xeluzrkv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3itdonwih.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vzgqhlcf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dmrgzwvq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3inpxrgze.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3tlrvokzv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3egtkuble.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3smjnrrcn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pxsiplfc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfekstl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmyutibu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mtutxldf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tnjddrtd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3psegfnwx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qixsuqbi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3adpclstq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mjoyehqw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3omvsbjup.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nacwoyhl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rydyckxg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ujhyecsz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xtqobycs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ypkkcklo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ehhdyqnz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3teyhukxn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cgztjijp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fvobbsue.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3voiadgyh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tmbghtjj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zvaetkpd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3shspgrba.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3uewtydcw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kcszdgaz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfykbvsd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tcgzdwng.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cuehfqcc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vexmpzxb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mfaprbng.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uvrnrunv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jqvoujyd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hoauvtno.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvbgwvxv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3adffaccw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pjuuioxd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qsdiaksd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mkvycont.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3nkzcrgec.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jgckahxl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3brazngqj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3sqqnlkib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxdbngus.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vskziptf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axeuphiq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3evagjotm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ehudursa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3agkeirsr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ljbloqeh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lwqvecft.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jvzbbzwv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jbnjgxtc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3txwqgjom.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmogcunn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nfaydwvw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rfsrwywv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qusaerry.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3emloilsw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3adzwuxca.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jfosxype.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rbvfkeqf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qorsfnop.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fqiyiywu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vhojnrim.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wzvbczsf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rhulvgvc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3shjqngju.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ibvcjkbs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uftihbfj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vhkcltiu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xmdbtpdi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3youaknuu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uhxpmakn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dqesmnwf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ujtgescz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3papnoffb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bzkdqwil.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3afcdedai.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kgolvdob.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rixjpudw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cztngfnw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kpecsnyk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bjbfwyti.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dlxbnftu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3naujmgjq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3akpvqhmv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kwwzpxxf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nnbbbrzz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pdhmifsv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3asznmmpk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fwxnymwg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gvafakoh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3eyugotrk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3pkppecdw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bimsgbrj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gfzsgryn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ajwxtxrb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3epeksnie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phrvmhyw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3yolqjljq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zqkkapls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pujxulsk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3cpoqmalj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3huvsquij.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zsfwdmjm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ssuhlovx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vzakkcpy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3krgvinsx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pqgdojhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3bhyrsldn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dojmtfjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hfwtfscv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ejxqkebc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3svyeezvp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3oqymncyk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3chugiqro.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wxdhhxma.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dygogjxs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kbhfsjsb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3peguaegv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tjgibwtr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3isexzoif.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zljbtzsc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3nnlfuoii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kotrcexv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wfljvpkv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ayucikzp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asunuvdg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lojsmhvs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azvomxko.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3huwqitcr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dhnfoaib.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhmiujrg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vorszmym.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bzwnubpi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fkhqkjxo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cqmzvumh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsndobwo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3slqchkie.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rhtgpinv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hypeoxhc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pizyurle.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ohzieinu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ymzqrxsq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rgozyxom.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bgpywtqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwpkvkyv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjympdne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aacfvppt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kqvugadt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qgaackua.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lrubpvzo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wydhflnt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3rrfxmsrn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bxqqavjs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sueoqmew.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3tivhuyey.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nkeniclw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vdbubxpe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zkjedyrf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rimkeflh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fwvqgswl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dfgbxxeg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yrhvoqvj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kmbaotda.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rbqryoxx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ezcvenpp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3juavevzi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dfxpobnc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bipllvur.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3buwbeucq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3almcbhrt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gowjwfya.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zyujdhbs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ycjgwdyh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zlhwlogo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mnlihoaq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ytfrwbrp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bfwfhxgd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fztkrhvd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nfezutaj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bzpqsziv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3iwumgblk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bixealtl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ophnzssq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wpobsghk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjhierlc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wyrwqzgt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fwmuiyde.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ulkavahc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfsguakx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xmgtlwbt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofojgcke.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eqfyjdvv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3asthisjz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zwtxhoia.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mrshmpye.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ttnomvat.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vswcrjmm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lxpgqaod.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lcvifokr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3yyrdiwqq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzvqbtd.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sqpihsrh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3twtulgzo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqburkb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nytutoaf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gwlcnggx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fvcaoeat.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3habbatdx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cjaffivv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ymehogpx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tomsmoev.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vmyximui.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvbuxxff.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3udyxwnsq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nuvqhgrz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tosmdfbb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kxacxwvh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3benprvix.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rgpkenpv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dmqexlem.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvqltpq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3obkaecir.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wyyhxrbt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nayqcstg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mejlqbtj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3zjqalvxh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3oknkaqnn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3okiqmdpj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mcaaatsa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3uhibxyyr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mcdrlwkt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yegtfxjo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvdzezjp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlchgsgx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cnabpjgs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3swxxxsbw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3eqlxnxlx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rjolsxdt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pcomrise.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emlpdpxe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lglhyxxm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgneemfv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ptsywsrc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3mfpoxylv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gaczgkte.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uiksacql.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3utuxskry.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvbwgfyp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3eycnspth.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pcmfhdhp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rquzlqjw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ecnomtae.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3plrfuaqu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cpfltmmj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rhvujxce.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3blejcplf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ytxvbagt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3knrjpwyv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sehdychc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gsepwomy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xvtqttco.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jnolwzdg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sgojercx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kxnofpsh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lpbmwgfc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mkcudiut.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tsvjcqxe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mdihiama.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tknfdnho.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3qkbmnpms.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cjljppzd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xhresiid.html


<!-- 参考信息 -->