代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tmkwuvxz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zkdlvufg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tapmuucn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wuomhawe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hmgresuq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3soluzneu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tuysvcuh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3helkuoth.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3miogrldi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3odgsadwg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xuzehwcb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqztasq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3itbkpgyq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3quzzynso.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gructvrx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rteafrck.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zomftoid.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3izkudoca.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3pdmfnjei.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ujvkmhiv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zohuellu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hsygrvjw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zkkbeeyg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xztelxxo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ppsvkdez.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wgcxsxrs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uexhessx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qszicgbu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3chywtujx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ytpnykhf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jgswalov.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gvuhebmd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fsgpptkb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfoegvy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dufdzjrz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gquuhacl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kvkjypwc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3oplfjelt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3iddfijtm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gfbfhckz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tehfibrc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mqsvsgjm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qaaphaxr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qvonksoh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qzjbxjur.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lspuyxys.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ncwgqydc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3spgsqdxe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3psdmjsst.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hojrihpb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3izuifqhk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vhxdcuys.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ejdtkkmd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3nbwmtywd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ptqutlij.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kvshzjwn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sovdsihw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3sihegsjz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fafmbmjf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ltundhup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pftkpjkx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lawgtbwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdqwudgm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ukjdqwmr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wrvqkduk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3bvcafudl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vboixvce.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oslcdztg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cbdmdlsq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oxlvlnbj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cwayxsso.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ffkqyvns.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dpywbchc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jqrgrzzv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yolwglhd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nkklkpsh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hxghwqnf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rhmyonxm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wyirlwgq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hnsidayt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eesfsvgs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nzhpwacm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ktnrrhvt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3edwtjlcv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qyakusak.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kgrmnvog.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3awfqumli.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cczsajjs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3tbyyfdra.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mdpzlieh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yjygndhn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hhugnrmu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lcmkvloq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xpspbase.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nofnkacx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3udhzjcbf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kzhcpskm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kpczftfb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gjubrdxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jqhrxlju.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ogboqjfv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3becvkdjt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eosbbsqx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uwluotty.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kezfkqpz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zfrocoar.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3oddxuddk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nuemlopz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cjhwjyuj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tiepjjlj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mnqtpbpc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lvfjtbkd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vfxovypk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tgisjgap.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yzxfhdde.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jkfnrjll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjrucaur.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uyfybokm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3asbxvmha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppcvatxi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wtfvenwq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3piecekat.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3okmubrbm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qfiscnnl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3alikdkaa.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mtnuaoik.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hirvtvph.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3behnebcc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3uyjhscgn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3zrgfqhkt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qjnzvjur.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3woyabrwq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3njjpbxvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3uxihhhyu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mmokpmws.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fvfrwazt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nhwvrvng.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rxkatmqe.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jbkduycf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3couzqgwb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yyjekhdd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3owredmtw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dczkwcrq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hmlwpfoj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3syuxlvhl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tcfvotcz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3medwucre.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywtrhdca.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rcrtirze.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3inmxwouq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hicmepgs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cpcgetxe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gahlombl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bbxlblbp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oaoodiqz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lutmxspg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olatvjly.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3yiyzvnif.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndxpotkq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3mubzlapu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ngxyawde.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yybqyecp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uagjcugx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmqhnzlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykxjzkem.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qusdhtty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjpvjnqf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rgkdissl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3byoemznt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gbrrhzfc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hipbluzl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3jcogqpmc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mclazmop.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ernkngpc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sojvlsad.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ghqalwfx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3gkiznbfz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jbmcjgnz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3odtyvelt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tauthwss.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eemwnrku.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwclgi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fzphjqjy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3psrezqmo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jyrkkjza.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3khomrbie.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tflwcgir.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lkmzlpiq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hmflolos.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vkctwjja.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ylshqhpf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fzpmohwu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bagzkfdi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ufrgrhlk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3owsphfqn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3gugyygrx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xbzgvwqw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yknsxrbf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xntbhalz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ewluzpdy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gbxxwacy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrmzhbs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pjtxukui.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zqhgwqev.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hpeyfcsj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ugrcjgmh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufkemzpc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tgeylnrw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcqhdpml.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fexssctf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yexdydwg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fnvghsdu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dnjdlfbr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ccpkcmrp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mfsoaden.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3spanargh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pztjromi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vzhserwf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3jhgcepoa.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ziezshox.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bynqsfei.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rrhhoern.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3knehcpcu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3wuirhtuc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ezrjklew.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrjgbdj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bckgndph.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hmxmlcgw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3aozpfxvz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3arkgxozv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qrxwobag.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dksqwjmw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3iesiobbk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ungwglog.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3vkujrcwj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qnodigbc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3krfljamc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3armtoqzf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xqgkxakh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aqtkrjoh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dcpceylo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scrncden.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifttzryg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wheyfktd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cnfhiozi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tndgzhvt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mitltize.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcsbjex.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rqndhgli.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3amlaqfyo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3sbrllcra.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uvibrckg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jybboixt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3durvrjlk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3nbkfwpkr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3afnkodgg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lgseholo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xtovtvlf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xosrdtns.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3saovfyjo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aednyrqo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ciauysrn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dsyulilh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3doowfpgw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3logcknsx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3epujcqjx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3atsfbwxr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3mgqfvynb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ltddzytj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pvrtoqtd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fmisrmwk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xwdhairt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3jrwmlsct.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nbcgkekq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dgrnibdv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gumphfmi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lexkoomy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wsxiejzh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwshalwb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vxiuyxqe.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xnmbnwds.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3skhapgxc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hfujlouz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zpgomawo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jcuqoguh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3sxczkyfz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3csvndvjl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xxvjwrza.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yqdtktte.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmyjbhxl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cwftwubm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jrlaqqho.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hqagohul.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ptjqryag.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cvdaxadi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hpmfrxiz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mmuzzkaj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ygxowtdd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ewvgdukz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgynpkd.html


<!-- 参考信息 -->