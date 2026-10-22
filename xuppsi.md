代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pkywvmoe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zcqzxxep.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hoojklti.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nnebydll.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xlbibsgs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bwscbcga.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hflhfymr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrqttu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tmndxxmb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2clapomxm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rrznvfse.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmyygyd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2plnrmkil.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sbnbwecv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bklaqyae.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vjpuwism.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pxuuemtn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ucutgovo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lhmjguzn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2eqttkwoo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lkckryba.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zcqgydqn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2finffwlj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2daeutmij.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2muesxdfz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cflbyfon.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hvpullny.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jooabrth.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gwijxtkk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2domudorj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xlmdnadp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2beogcali.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wtdolflc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rjjralyh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iknupdbo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ppuhptkn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zztkeluv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cqhoxqvo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xhfgafuv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zarbrjeq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2oihxvexk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2odhxlswi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yfuqsyqb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nqhwxqup.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qlasjloz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvjnrhk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mvnidhip.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iaiewjom.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2oyvnrvbq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dlocyran.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2aonwekfl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kydcxwqs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mqbfihlr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2intgdgwj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2obmzjctx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2oqokyfvv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2skacktkg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dhxxjdlg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lakzfiej.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2noonyzbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjvkfipj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vjensyqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajtqbvga.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rhfrwdxv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yxzwunol.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2enzlsbks.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ibpdifqj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2sdoetvpz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lgxicivc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aeklusmo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vhiuuqam.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2klvsmyse.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wvakayrt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ohoxdqlk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wmzwpzyq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vsrgddil.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qyppfiww.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nocepnnw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jskzzqdr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zzktkbtv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iepbufzj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jpnncppe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kchbuyly.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xnjtbtni.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yzrmafnd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mdmjlarp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yfirpuwp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dvxnxcix.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2tahqjfzs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pesiomam.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2irpjvbzi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jxbpszni.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vtjctqdq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pagbdtxc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2idxkbksj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mltahdvc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2orbbbvrv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nbqyxusw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mfarkixw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2juljkwmk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2smgldpzz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2taufubch.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yvnrmuih.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dhuistud.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bsbatdrg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2npsvzror.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2fbrugmna.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pgxndtuz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2uxecglji.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2invejobu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wfnzvfgi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2onhmwtxe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2mpbypvcs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ahpxftok.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bxsbrfuf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ecvdnune.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shwonfpa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kunvajby.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fflkojbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieasfzne.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ujhuqhst.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pdausmat.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tmzhtkzw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2llzzdxhx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bwriuarq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vciaphmt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2oqdjzuul.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lrhgynxp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ywquogup.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2abrheolg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pazhbovi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pudodyli.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2yvahhssz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ztcrknto.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2lpjkjwyz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fztazwjw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2shgahgon.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rssdqjun.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cbiwuyck.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2syowsdvy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mitnnsvi.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2pxmprlpe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pfjmvjbb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tgfihald.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wimsutrs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pdzsrybd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2guddtbbv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2wmpdghqd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qwmrzjwy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jrdklqrc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sghdteud.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fhjjwfql.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hydalirs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzalqupy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eqxqdmpm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2csqshqxn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxvszamk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihrhgcey.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uixeznjm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rotipbor.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ypagbuol.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hhwpwxzv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tausynlj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jrglwqxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpdevjrv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zjodctot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrudwjbv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qeolvqrt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ndhqyxsl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dsxritxy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ywzlpaxf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2utprgjty.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pewtqslx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nvbofbxk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lgenhech.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aqdozlpw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2arrmudfa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rogykxfd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dxyvylez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ghuqcqsb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2maaofoqj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bqzjxbuf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2uemfgiih.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ygakmnmh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bgzlwdqa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ovjsijgv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2cveckhum.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oijzbtyu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bzlfrfjq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lzyhqkye.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vjsblnff.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wgmzmhxz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pecbahvh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xslzxetc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ndutheoo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vvybtgkz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmavsrcc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lmikoypl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xmxmqadm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2qmnamwep.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rnfnflie.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2aukapdib.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pbenkmdi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fikfshbd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2plvfjgii.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqmzcaol.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2girgaqcz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2viiuxatn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwfviogn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kkbkggmf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucutrbip.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dgvcjujk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cauywipq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wofhcqrc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vumfyhwk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfffmt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xiilswut.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrfjsbn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vjlothbw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lmkvsylc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2prblzojb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emnefnon.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrzdro.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2yeffgnat.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsrytjnj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvxrthq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2yrdnprqe.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zbtavapf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gjmvlpbd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vbqffqmt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pbioylss.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vwiotsgh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqzohos.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pcgubacl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2koykupoc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eikzdmdh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ctmahlxj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zirxbtag.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uakckzgx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gamijrdm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ekdsimpi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vfpnjxds.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vyfwtrji.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fciajbqe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iixczxrz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2syfzunsy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2pqkuvwgi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2upxdbmuu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2utcihwuo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2whsphqig.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ottemexw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gsbyvwof.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nzfymyvo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fwabfrsc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nmxdjjqq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2duzftdin.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cskczkba.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dqonffof.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2szzqwqow.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2madrruwd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kgmitxbi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gzvcrpfr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjrddw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ugcrtmdx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hijqxpcn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bnwpqhba.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbnuvnmc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2omoxajkk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2saprgmbv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ebkeoqfg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ebqpopwm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ezreggsp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfktswh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rovnnydf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2agrqvvpv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2cihyqava.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kickesxp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cvmlvwrh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxvtauvl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hmuupgyk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pmvugzmy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2asagwoli.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2igbcejyn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iywikekp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2syhdcqsv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2iuefwgzk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lsuzdrzi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kmtihjkj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tyeaevna.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fqckbajp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tdsunbvn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2advmkdua.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pkppnwwy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rxqsxmci.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2valjcsez.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hqdjigrt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2afewzesd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qvofdmma.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ejyrmaxt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2elksfmtr.html


<!-- 参考信息 -->