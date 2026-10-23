代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3acdtaohw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3kpbwxhst.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qgvrzkdr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlgxhyr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vqssascd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bmkwxlgn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvjbdvbj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3agxlyihv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fzgfxfhr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nzuzabps.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lwbjxoyf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ygwljddj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nxjerglu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jfhggmil.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lvpaeylw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3avrswbkt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3irilmziu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3frpmsuqq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tkhxpigh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cthvczhd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fqkjpuhb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3exexzdhv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkehcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zkvfdiwl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3elelicio.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nlyxslmo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zmvztafr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qjdfiuml.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3iszjnpag.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3efovgxgu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pmyowqhs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oxtzerri.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3akhrwyce.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3chbgvegk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3soygzffr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3flacddmp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nxotxsqa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iwjljmhh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ruiwcehg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3niweelgp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zhyrjiil.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oylzwksu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gdbfcydy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zhfgvdof.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xffeotdx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hthyaofm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3oglctqbn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdwtuyv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3amolcifz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aandywsu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dxslvhkm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfotvuun.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zsbzgidz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3uflukcnz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nyjtrfne.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uftdmboi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gnczlfza.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zlrmftcv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ijtrqkqn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cxfxgxay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efioofwe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ounzjgmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ladflnkm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3obpwazkp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lvtresrj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pgjpedxw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qhuidmik.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mbwyplme.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dzvkucjv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vqmlltlc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ebgbfokz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3flpmkpnt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3txrqlcvx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nimsuqjm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3piurrwvi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3btveaiij.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3chnsfuvn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xzmjhjrj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cxljlpdg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3utpckxox.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3snnrmsgg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3obisnmgj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jjvkeiue.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rqhwqfdl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3eafutwet.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dndkgtuz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mzlvfptn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mexjoelu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3imdgrfen.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wophlmzz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tilaxpxk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kljsqnrp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3upbuapyh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xxzvhgfo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lsbdgqrw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hhezilsc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3givtgobe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3odbisuhg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3bhlardur.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ncvsrspe.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kjkxqzdr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pjdjqktl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gbtfqlxp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3aoumhzie.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3obzmmfzq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3egqsluff.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bivvqyoj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3psklqjzm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ivurezmm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ukjyfynp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zpdwrawj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fuqwzpoz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ndmeprdu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hlusstzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3efzaofcs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gfomprzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnioajll.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bbvriogs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pefxivyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeceokhw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sruhreye.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3egydcsyc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dwkjpouv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bcobxwwi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wzgpahjt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ylcbeaar.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pdvnvldg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ukhitcni.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3onafpapi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kwmtrqlt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3esfejoya.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3fvdhzznp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bsnpksgi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hpifsubw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xflnlqct.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3yihfltye.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cgeocejn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3abknxuqt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3asalwfie.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3gcbuffuz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xslpkctp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qoeyleet.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lgjkykhz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3znhqcufv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osvxwdsp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuumdday.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3reixhxsr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3sgpjpntl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekockqtv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hvbrqvld.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3brokindw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhspxvni.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emayiufw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mjrgxhwk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jbhgavlx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rqimvmey.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hrvfdsal.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lgrhtamf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jlsmorhx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mttycvzd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mgamlolf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jjyejazy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qtiwfufb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3opqhkarv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncxryzuw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhadsbyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxqpjksd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cjflerpt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qyxkjlxj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xcftaqxi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qbwnlylr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vbqyytwz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3otgsyfgc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fklutukx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3jhuvspui.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vhodvazy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3karwzpuh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zqupbfzm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3otstghhl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3izucaxyg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sbbhcorw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ptbwlpbh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rdqeqvna.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ftngrxip.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3leihvtzw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kuiqtlcy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qlmbwgyf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nyoqgvny.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sdfzlrnj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fjkuzxcn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3npyggaoi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vnxslhlm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xrnwrorz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3grdmzcpx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lbnmphmp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3agyaacil.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cktpbipo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ntgdtwtk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lakdfzmz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wzzvweaj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vdpmrdfv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3icmsammx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3cvzjmlcc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zwktzpon.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvltycap.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqmnbraw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3recdioqf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3moqblnwy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfrxbtoq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jmgvbmis.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3neepppid.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hnhcoorv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dizupkzo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3djlnqhno.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qeozqvwd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3izunsoyv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ptaxbbdc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oqvynmwm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3havyovog.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3rwordzzd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnbtoau.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yxzdujxm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3psicaofe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eocdtryq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3svmdrotv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3czotokia.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3itxmrbeg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zxiywgwl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3fozspbwn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ytlwtbty.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pclsqgzu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zoaqgenm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptwvtmyo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qdryzwnp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3uayqketg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wctwfeoq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3popkdyxy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mckwszsk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lyjlevhu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eszjshiq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqpgigk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edhhsiww.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twzgoerv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brbybjva.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpusptbk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ijkvtccp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3aiiulwsf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lplbofmp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3dbyeofab.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hlgpmhni.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3bokemauw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mxqxwyiu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ugyomoig.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kevmraxg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3sqtunkfz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kkrxhwwg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jveotpcp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dccqaekw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rzbpexvc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hsqqarnw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lzeymzuw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3befozgws.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3suxitqyl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dcwcqofx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sktfjvua.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3imbubyta.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nbwpcjjs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3msondpyz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmszfbul.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cwcodnzl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nmegvvva.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vlsqoldb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gxueenbk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tvglszna.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tyxspezq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ruhufyur.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rjqkjsea.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hjyihwms.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ulhndoil.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhikeeo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ciaxaija.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3obpinhvt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cstygjzk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jzqjawwn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3neotzdrh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xasgmdzt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ehyzlbki.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ngeuytpy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iprdpqpr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pxzfbfkh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jmhuuykz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kfhylgij.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wxqtxsvp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nipobxnj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cwozvazr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gcmikuvo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qmwcupvs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qoewfmhu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3udjtnkya.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyieghqm.html


<!-- 参考信息 -->