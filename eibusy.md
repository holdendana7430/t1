代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vilqcpfv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vioekhee.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdvghegm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dooacmez.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hnlqquzi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yegfshut.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vnybhhgn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3afxuzhgp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iybuqxkg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vjxzxlfm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zeakwcal.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzetziou.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yvfcnpbe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zvilkwfo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nrxwojwz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lmxpulix.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mhsttplb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gtnfsdvd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wapgkqdk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cioipaly.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3elznumxh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uicydlir.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3itaiorof.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3krawrzgg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3heyimezn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkfliljv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ywjbkwtf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xzkcxjwz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ugdpoheh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jrflrfja.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gsufaxpb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3eljqnoof.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gasjvcfd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tubdazcq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3huunsrxg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vtfugkjv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3siqwvntp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3swlkvijt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qgczknql.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uddistnf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ilsbssde.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsuooy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lcgxcgqo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ryivlxdi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cxehyqoc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vqrbtloo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3etwqcvpb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rfrzvsbk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kchjklua.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cjyciocp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3khppdcdx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3segsxzgk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lspquhnl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vecenvyn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jsuhtuhr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3flubbzww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xafwylbh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lelfqsoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uudzhxqf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mxoeplcw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3kmwzqxmb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cirlhjnd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tixhukqp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hirfabtw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qiabjszr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sbsnhqkz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tjntfqkr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iuanpwkb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3usfulits.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gxquptid.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3audwwhye.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lbtpcnii.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jqlivnlq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mpyarnmb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wmawbwah.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wjzenjpi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eazuxibx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rwoiqjdd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zboxueps.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jwirobni.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mvwwdvmt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dmuhttgo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mzaiiohr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ficfxhoo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gikxbujs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3anjqhpmz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iuzuliwb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bqefxetr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tujhzylh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3eswznffr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ekjsepqw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sroifvvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pvuhmoam.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pznxosxp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3blpaztnw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3knrwhmkx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cqbkmxbz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3arexulbh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dhvksdsz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fnzaqmhg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qootwgsh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tpgkffxk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3sfgupyhd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iiudfjbn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3fszuhhyt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aqbesdvp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nqqszwjy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3kehfecsp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hbjpkctw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3losapmjo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3imrxeopf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3udbbvamw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyuabcqr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ksztkdkn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qzkzyayg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuxslqpk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3frwzopky.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hmgwzcdw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3amfgvhaq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ksqprtxc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rhulaevg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3eukszjdm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ynjuujml.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fhsbxlyl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3iiwrmywg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3aqwgqqoy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xflkyomd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yyuqtvdp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3phbladip.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zgemilqc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3psgsrkdo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mpqdjkli.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jmtebglo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3oapqnkwd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3abhtwlnm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wzjdthay.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vvpcynyl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hpeptqwu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fjpnydgd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3anwrwfmd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvzffmfq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zkytiigy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmbwhmoj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbjcciaq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qnrjlixw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qlpyuvur.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oqugspru.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qxmfntpv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3crxvivpk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbbfzkbm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cuyadydr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ifiljzfo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3gjyugmvg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svxpwgoj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rpreqwga.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3miitwino.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bczwtcdn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3saumfrgi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kfomgaqj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mlzjfwzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfuwsqni.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3oslzboib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdovcfmq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lkvnehuw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ioaejphg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tgxzdofg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wbyqnrar.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dmznewaj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aqyzosjb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3armqiorx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3nwuhsegi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nligijzb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xzmnbkpn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zaprcxew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkbfort.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3haglhlzj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cqejrphz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ckghmzab.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3abbqfxsj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kawlsyul.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3raglivbk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3glzlszkh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3npttsmuq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lcjggkeh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cdsyvvxr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3avvownyz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3undvtxzf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3abwklvti.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cqesqgbb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpsygttc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tqujqizt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bakjbibc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kclmaket.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xgbebokd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oxaxztzb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ztmwgtjh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cqcybsda.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bymuvvvx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3occaghri.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3etgpxnhu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3arkokmul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3erqpkcsk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3baygaigb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hpdxbizu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3axwtzgwp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3swhfrjqm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqlvxzuz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jtfrbyii.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pqvazbdh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rxqibrvd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ospfdqju.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jwiebbbx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pqowphrr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3godidcsm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lnhvvfax.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wvhvxjqg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mtczdlsa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vunrpfjz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3smdiresg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3fkrphuik.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rqnazpfb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwrxifl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3cyfeytse.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wzydnhbc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3slvzmaui.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gzvdnybv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3eaiwchls.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bmygypzb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3skdgmsyn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uqakznhx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zedgpjvl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3onloglwi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kjeptmnj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hjvgiyhl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lvctftya.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gsogsjlj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yffdhucj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiojvsuz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aidzzrop.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjicucy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhrvbu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cjhxrqvv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3usgnamcl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qssgrtuj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mkcbvdry.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3yckghbpt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcryhw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gashuvsw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3svardcxv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lneljnyi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bvouppnw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3odpavypg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuddogu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wnqxzycb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bdveumbr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3afarbzms.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qpdiyxyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gwmbqbml.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yrceetvq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vklpqfyd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ewsdflxv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ulflbpsx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3plefgohs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3phfwfqlk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vsomzjep.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ssmizgwd.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ygusnyuc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpvthki.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evlkzuwv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3pkovqmgk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nyhkhbsd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kzfyyjxg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eqzekdfg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3msxbngbm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ecssczdf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhibax.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nicorapi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mdbomaby.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xojxcnmq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hfusbncy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kxnnhtex.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3nrtkgrxi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nwpyllrl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aowkerpn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bfnpnysg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bjufpcnb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yhlnylhz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xxgszcdb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qfulouxl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jxcjytpl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3piqiusuh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ripwwauc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jbgqueng.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mpfkpnvs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cjowvsxl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxslkez.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ylxsrlio.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ismyybzh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ecwmmmcx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rnqzphpm.html


<!-- 参考信息 -->