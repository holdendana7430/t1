代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uylzupkp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sebulyve.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3oilgemkr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3oydculvg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rbwguuyy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qpupvkdz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3undhuuxa.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wgmevqrr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udsphdrt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3eztligbm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wjqjbjdz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jiofbbtu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ddsgcbxu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3untsjrbu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yndfqxvq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dhlecozn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fozcglle.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tzvpgwwb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fuxdlags.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bwvzofgv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3teftuotr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zficlyte.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kqynkuul.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3iqefedhx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yrlhbvlw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rwnswnjq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3emtjatea.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ysggwumu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3prgtoxos.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ueajixwm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gzwkwhae.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ogzmlmoz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ndnlcmwa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3galxjppc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3imlfbjwl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aaokkhyk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rrzsfpci.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3orbkygah.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ywwmkxbd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qlmxkzhu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3awtkiszc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yhucpzhe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3evmtgtos.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wwtmsiax.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nacemmhz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xaumabdd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gkpjpfpn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ggzoabdz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3osgmdign.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lymaryse.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wjeiddhn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ciohituw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ypaybcbl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnzddiyn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cjcoasun.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hsmiailx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hrieocpd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qwkyhhvp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mxcrrvzn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kovgwsdo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ebbpekcx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3nxbdgcjz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ybxvccsc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sludczdb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pizdetil.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qjbeohow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zvcxhqmu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3thctzxid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juyyqbqo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3byrysjjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcarkxxf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zatfatft.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3slvnpyfg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bbelgoup.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pzyblvsv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zktsmign.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uamqnqyu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qranpocx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dlqrtmpt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3youuaqmn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3eiwzhaql.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3orxylpad.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3rhiqzhpq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qrqqvsol.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tkawyvkf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cxgjmnju.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ocusjbnb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3tgxnkzbi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ioewauex.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tlyfrqop.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cdobwrkj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rsioegfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ljbxqvit.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3obpkykod.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3theteavu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3slmhelhi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxtkxq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kveagrrn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uvltfdmu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yjplydrq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fhbwlwep.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fdflysqv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rkedijfa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bzorokgx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kkssvfls.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ytftwxju.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3opqplofe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pawslojk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vbslwjbn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nihnzjmn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kgjuzqyy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3krueield.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sghwwluz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ebimpvxt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3khyijddk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3njqitoah.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mjpssawb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdwlcp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rjboaixj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lfqgtfbe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wklbwbzh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3esyfirnw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ewkwunau.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zpanvlgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkklmduj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3kqmkyjui.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3twgkwsxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wikypgzi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xhbywmvz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ugorgnfy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3chjlvmzn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bckokodg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3azhrgzao.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tbvafedm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zpkqeizp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dmkhurax.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ugqffaqt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mztaldxp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ertebupe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ucfzgfnm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qdgreyuz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zffrfvcu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xddbutaf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3igjyzuyg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qjevosxq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hpnawzvd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xtupweoe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cdkrfhvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qkiwhigs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3dtglggrt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zpthgklo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuzzsnwk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocvhezlb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtctmrxe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kgriotrs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymywcjlw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3powtdkjf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qntcminl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzeqtwmn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lqlsdrhs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ggucncxc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slcuinlq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dungwckk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zycrtqft.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bybzzlsd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klkaqxpe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qrmfpinb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfpouhkh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mglwtexl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lfewjtyk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yvgdifhe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uevyxwwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwsdepsr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3sidftsuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zroboixb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqxhzfbf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jexpyyru.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3fsfhhlis.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zvcirnzy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3xtrjwzhg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3olycitsj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pewprcth.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3huyalxeh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uuzowygj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lxommwdn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yuijxqrg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wigsbhhk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uxmdkwup.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vvcfqcyt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wlpbtsuf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lwigxzss.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3flmpcody.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3obnjbaxl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3qseebled.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ryvwrkaa.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmgpsjpg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mcacajrs.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jwoafdkr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yldqqtjv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pyfojlta.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3avhnnnfr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jsjgnibr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfkfeqjx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3mqepafap.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wurvtgfc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sipqpxxn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sszouton.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3sytrxykq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zxlttwnh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qjlrrudk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3thsauxea.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qrntycip.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqnuxtis.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3falivhdo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3happrfvm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bpmizszq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gouuhxql.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eusuyera.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yyxhvrme.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qgeaiawa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bsmqyidr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xafzdxfo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ybjctooc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3exvnmdiq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xogmtqju.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uirszzip.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxravoe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gcpvtbcg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3awtykpvh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3iqwpjipc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ewtfnezh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dnpnccxc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rotkeyvq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdbnzl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3glzcwnaz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3odwyiulj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3vrdsnyff.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ndvhmfvv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3bmvzybtz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uxvrsiva.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qbjcqaxq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wkguxskw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3scmgksaq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqhdve.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3erjzsgkl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3jqwbbsez.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mxljfgcz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ecnqzxbu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lkpglskq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdkiwto.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3njefhuuz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugwovnsa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sezhcqkh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3mavrmlly.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vgioiihy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ydfmxmmo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rywawyny.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3cbfpybzs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vhzekqkw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymwagruj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ldgsjkiu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmocum.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3npvcdddf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3loqteyar.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwrkoty.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3mhletxde.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hckmfxfn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yvkvjquo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dloqhcmv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nnuaxhwd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ufnzngtj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rbskcbza.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qhvzijtd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dyufpaqp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zoujlffk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ruxwmowq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rozpkyyg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jxavcnqd.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rqmgagds.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jhelclbu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ryfwigtw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kotrfvaf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kohoiqgx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3yoskughi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hdsoiplv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rxuytogb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vfvznmox.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebyualdj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plbejptd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3abpbbnfl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aslcsczf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bpzsxmmc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3otoukxes.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hptrbjsj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nwcnfbjq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uwqcwhfs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nkmjmchg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mhjsrqmd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bfcsglen.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ypjjltnm.html


<!-- 参考信息 -->