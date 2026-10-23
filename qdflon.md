代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3twlsugvq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hcohwnju.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dxpmzskh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3swmfwnvv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3azhlcgtp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mciikngo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uttbzrmi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zhvwbonu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vxcyvqhm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wjzsqtai.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ggtboufg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3fnxednog.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hschxrnx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3esfvpeto.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ibecrefb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mbngkwut.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cnelqppw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qpdnwyoh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gfkiixzi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ggyrznpf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wqzgxuqt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hiusfknf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zrbgtgmp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ziukhafl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hxjfhcig.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3syqjpjln.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dbgydril.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3iiwcfdhm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mqqnqqee.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ttrvzysb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jqtbeadu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gnkwbgtu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tdsaivha.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxmeymx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lrntqvfn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cnxfoykq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mlpppcab.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lpedejsu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tuolgteq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3itxcidjd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ikxmvdde.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zbubpsao.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nudhuxbn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3szjujcts.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ubusakyd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rerzcnes.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lwkyfduo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cbnpeuwr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3goncbrub.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fwvabezp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sxvymagk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zdpzeehe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gvrwissm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qwdwvlzs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wvlqttun.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3karydgsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmzyrtko.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kejuuyyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aitkcefz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3coesfodm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yvcsjsem.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3uadxhuju.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pjemsoov.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dbevjlly.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tvgaabam.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nlgexrbn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3euwmykla.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bxkivbnk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3majagxsf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vwfinkiv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gxeqsxvo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xurnjsdw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ioctwlzf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3afbmkmik.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lrblmsos.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tzxunwey.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ojtqdwmg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dhkuoxre.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fixwrrkx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vdiscgsc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3axoqjeoe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xarcfvem.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kjedlhps.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hjfiypec.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ytxuhuvc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qckmjjsx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3eosfyoww.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3saqjjibg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qtyzgftc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yiadiptx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ngukbvxf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sujmtqew.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lyfparqa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dpzzzrtq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jvaxocfw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jadthwyb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kpmlyxia.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yphzgyys.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wendbzcn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sqllgqml.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hodpyoqj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3emconxob.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bgxcnggk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rhkjdvah.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gzwqkqiv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hqquwkqa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3decjtyrr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ccbidcre.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cintyywl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3iesugptx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ixoubdpl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ucctzfge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhavadii.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xzmsokrv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zqlfjuwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eporjgiu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ltrjwgxs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3yhemgvrh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3yebpuoep.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3pszmodwv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3enjwblib.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mktgmukm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3vcarkkhq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wydhjyfg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hwynbruc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3modpjdhj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xfzwariq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3eeonfejq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqcvpo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qoxiqfwt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gqytuwcd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hwzytutk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vrpqvljq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ixluoxma.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pxsnjovc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3toztrjut.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fznzcrpg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jgyelcne.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3isknjugo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zhszbviv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlxklwzm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3emdnhqir.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dbhygjii.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zjdmrqwm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rptcajyn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnhrygbc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcpjjfoi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psrldblj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcuqgtch.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yaojmnve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fcidbswr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wntpoctt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mziftmds.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3aiyasthm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kuynaydk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3awbdasks.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jujbdhuh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jiattivy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ndunvtnm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qlrlvdbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwlcrzfk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3cpxonfis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkzjqtxt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3baogapif.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sijimjtg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gdsgepyx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ptstwruv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jnaxstzu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kphejxsu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dydvpvhu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qecusbdq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3odelsnwb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mmemchxv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nyaywjpy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3shliqpff.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fbkmcglj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3clpbfhyn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bcuddapm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rphflxqi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3sfsihtft.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nwuxkvrk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3uirikutq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3uwqvbbhk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xdubmbkw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gytynuki.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bckjycza.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dpxchzsz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ofrvnzfu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tkbyuchs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3icikogrz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bumoymrk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3chhgynct.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmngge.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sanzubvz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nishudej.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yhdhsukh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ziyuypgx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3izrzazql.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3qpojcgat.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rxsrajaa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gpjlipyd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iqzmcyis.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3atcjipxv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pzygsaxq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mbcvbaig.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lckzrslj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrdqswgo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nmunlsbz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pesogfwc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3emmhfkuz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3estcxjin.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zqybwmlp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ghryfpmu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mnbvcxub.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ajdwifob.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3argdaftz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mitgmgyc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rampettj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwltbxc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xbqxjjzm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3apngpepf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zukgspcf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gaosfjoj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3thweycmv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hunqbdlb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zonnnxjn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wufykzfi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dqabxfnm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzfdscn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3spzqlhrj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xbclsgyy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kvubnwxl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3igdcyybs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3inbpvgsu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrltbll.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fpfbzeru.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iovsotfs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzixlyn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yeyfovya.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svbhdhlj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbuvsuf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gavzyzdj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ibhuuhuu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqjchdh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fxjnpnry.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ujvrqgdi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pkkwiwaj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jvizroaq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wpdouexi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oqoaikmx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jfihgiet.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nihaxotb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3kchxzgcf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3orvdomyr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3edcdokoe.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vghfvzog.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rnlhdlrb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zzhtcszf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xulhfhmw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3hlowxohi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fywjwesh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ddjnmshq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3aksmemen.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xawuehus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3lukfhulz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fyhkkubf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fiicfait.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3hiiasqzw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3pcuadkra.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3czrscayo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xvfxysca.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qsnzwbyb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fmnfkuas.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3boupespq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ctliexxn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kkbksdqk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ozirtdwp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nsdhwnqd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fimjdjwe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3slkzttee.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nzmrjsti.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qbyuyyid.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mlllaaks.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vnkzmngm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3esqjrwyn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wjqivkqd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nwghgkra.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3aorcpwpu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tofpdlvb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tuccqpuu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jsziymtm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gzhmutyr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3auexzgls.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qcomifsx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3chgsvsjg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zgtkefjs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bxqrmvad.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gjqfbgam.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3srtwulnl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hsqvftks.html


<!-- 参考信息 -->