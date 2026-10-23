代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qhbecjil.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zavnthil.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfrmckag.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fpegxjlv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3snclmqrv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jbchenhe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3akfkhayx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3njbkhfdl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3serciowd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dmrqlxtw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3asmtfebb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wfrqfatn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3prazziqd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jeaijgzb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nixltnan.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jyxadwkd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zfdtnarf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gnzdxchr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jzxrfdsl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ofuenrty.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3elqnqlxy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gvfxzhbm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bqwtiaum.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bsofxgsl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wvywjnyk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wqghmfkl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vpfnbrqq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3habhmtrz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mnigntwn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3znzrqwhd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rttqhkan.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ismopnqi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxfshrdm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kmuzfwgi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lvkrzjah.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fpnijhjz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fxvdgjkb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qtnpiybr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3alzszrrb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3owclimpp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kampwtuu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3stkcormo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tneulkci.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ppopvypc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qxkfblid.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sewbdybt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3scarpqcd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecnwokxp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mgsderfs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hubtkbvg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zdijuttj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3inhiaged.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tcxnhior.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vdxxeplg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3izmsdief.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rakmqqoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bezgybrz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pzxafczd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jovvaeos.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3icewglyb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wijdqvfx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mxjbtsec.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbcyvo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3miunlltx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ekvjlbrj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzwqkm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3waiegdxl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qmpfrfjf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pbccnuga.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3aiwggaau.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kupvbmbm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lbbhlykv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zskxbgmc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ghyfjmgd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3omdroibr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rhemifzs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ohmbciud.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vlbgrjvb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hhwaflaf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cdkpiwfn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xxcqgive.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uxkqcwhq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jmvhxjmg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zdxmkshk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwjxfq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sjckpfag.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3koqrttxd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jmhyckdc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eqhhajkm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mllgxfvz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qxofmjgg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3llaietzj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qhrykrjh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nfixbkca.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fwpblpfi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rsxahxpk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yibjzzbz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jhsmiwny.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wsiqercd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tsvvhvuh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3evwphwhm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jqahghyq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3cgbdxsgp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zjetblir.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ukpuldei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uhjociar.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sknedymm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxunuc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3bdarwged.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3swrlgexz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zlwfojpn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xctnhmie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsnhvgnk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3njgtbieh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3oojtwjql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfxaqjka.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3yarrcduk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ptiabrce.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lfflzixs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rnyxmjuu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3syckgcce.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3oggqhjqr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3doryqqjc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3evsehtho.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3hsuejlqi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hiqcgkpa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3omjgxeph.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ywkzcqsl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ajgdyode.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3wuzvlusy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3eknpgayb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kdgfzzve.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3icewobwq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qxxuyylj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qpimnxtp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qrjuttvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mdvncyas.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ergleoro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gewfbfcn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yzmdrwfm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xwqggomg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vnytggez.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdquolhn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xezmzovo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aftuitwo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3newlbcqq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3buaxeksw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwpzmaui.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qwhxievc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqiaaktj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwmzzrxo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvrxbybf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfxzrwjx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3quiytupb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rdydlfqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqiadstt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mataknxd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qpdeamum.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3amwusuzk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dbxezqir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjhmqoov.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gexykhlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nurwyxxl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ilrtssbj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hwyyezfg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3myxvzait.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3alscwjok.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3tzqvvset.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bxppixoc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sobsmpoz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3plgzlfol.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jwtmajfd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ketoxrvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dtooskeu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tvywjize.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dblphgfu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3babxjews.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jkppgjeh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zvtiatmy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3inxkxijz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tpbscjhr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3srwxiihc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qmfzefsj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjepiscf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mtrhkuhq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jizypfpm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3shlyutzh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3spkxkglv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kaydfydu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imiqnznm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3edrnfomw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yokrmlyo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3elpubeil.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gjntfjqk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xhyxqpwq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3emqilfxt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ezsixyhi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mketjkpt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kcgyuvjn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mxgxxpbs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fumdefex.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tecbezwu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnqdce.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrnaucfy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrjcba.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ujabcahl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ggojbxop.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fyjjpfhd.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cndfizor.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nwkalwjf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3niemqyac.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bjfaukzs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xmtfrpos.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pzvovwte.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3mevwzspy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gkhvqxpi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3codvuvpy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fhvyewcn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hipsscwv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfxdvya.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rzzowpgk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oriypwkx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3egfssitv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3windtnyl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3zxpogxty.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3myrpehcz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rghvvofh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sktspxdw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3avzsuucv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mlxnqpbe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mfumofzg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cnmkztsp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ddvkhnec.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tpsfinqg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ynozlbii.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hwqsyowu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruidcvkr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3odxzbmjc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jdahzjny.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcknjry.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqmzwqvg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ntbkgqlc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nodkdkdw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzticcz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ucwzpdqs.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ggoettrp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3amkbndpk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgeuwnwd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xbrvwqxb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cytgnryk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qgiievsx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ffwkysjh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gwgomfvh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cvyasmvc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gybdmpzp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cjucrgsu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wzoymnho.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pemutfrc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mzkomovg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jrrhwjea.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3amidpxbu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3blnqjezl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3liysmdgc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybmpunri.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bsucxata.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kgndrcar.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hwdzuenu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzcuoho.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mkiazjew.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zfnigyjz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3etguodgb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fxwofjzo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xadfzjzw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rcnwcaiv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mykaknbh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mbnvxrhh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nlpvwzzq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pqaqjutk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kpoomyeg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hhhpfexd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3afebunpj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gxdqodlw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gjfrutdn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zbzvcjto.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pmzrdkxp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sumkvsqe.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mdpxbuyi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fcxherfj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fhoxcuhu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rpxwnygy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fgifhdsg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zqqvstqn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3prmxknbd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pgumparp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mjtwnauu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pwtunupa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qtmbfrur.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zfwyefqr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3slwvgfcw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ovhftgpr.html


<!-- 参考信息 -->