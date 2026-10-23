代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etrqjhmx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nqmiavfj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wpyweglq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yecnaakq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eqatpebg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jfrepifr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lxscvzid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oontdtrg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ucmifmsm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bdlvtfgc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fhnygaza.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lvmrbozi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zwkqqjds.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dxcomony.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mkwhgkcu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kibnrnus.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rlashikr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3htakxbko.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ueiteprp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vjjlmizd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfcmfw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wtqfiqpu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oyyibnyh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mtdynxlm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ukrcxxyi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gliewqxe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nafkvhqs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3enfnubwl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jhiwrqij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yeclrnuo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pledsgrs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yvlsqdju.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xflyfcfz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fcotumcw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ehvatzzw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xgyogyvt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dokezoae.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fasnifjt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qlrtrhel.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oydsjxcn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3udfcatyk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lyymbfgq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzvsglkf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3grhekqzh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hsnsyiac.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vejwvisk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3oemqmcxl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzhtgccu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yofjmrbf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gmqmuldw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ylkceuoe.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3byxiqkxs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3luagrwra.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kaoejkvk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3voaziskm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3klfyiuwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrtvxggc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3abjggona.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkpufjbr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wiokqwbf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nyhuhefr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gxunpmtm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oskplwsg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xmhckaua.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vvishwbv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjzcinyc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ugrzxbxd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fnvwphow.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qaxkbwtb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vkdcpxks.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3irsnximi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hwxnlqbi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mnainbvh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kbcdsoce.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mzuorncb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xlbqfxip.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ahxesvso.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qzdmmjaz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xkvwyhcp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jxgyimzn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ooamzoxa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3alpdzecp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yldtpgdn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ozoljthz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nzcuugwc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ybhedtyz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dmrczieo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hzywclek.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ylavsucd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3scvvlhar.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mspzlmou.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xricvjft.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wnnypplk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rpsrmlyj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yrdvmbqr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lccqggez.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rciaslnh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3aozycgsj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3fosmgqzr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3phihkonp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3eiaornsx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tkvhfftm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3yhjgbnnq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ejinmhqo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gxbdvcdx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uptxiaxy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gppbjzxp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3emxvuvrl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3tmmuvjgm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mhtmxtfl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ekjlmcae.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3oygmqrgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvcajxdy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ndsjtmvy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ozzcpxsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktqcgcpy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3cmswhraw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vhyssgqp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qfpaxcnt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zitvztsy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3bmrzdqlg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3oegfivfo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3bsnosuvy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vhdlzalq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xthvayge.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3emiduxvt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dvdvnouf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3aoeqneoq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rgkittgy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3crrjanwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qgkenydo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ujabrpux.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vgsndmju.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3nxmpyzzm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hdaefkuu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hkcczwes.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ugpaxpbt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3bckmzzcj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqfslkle.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zuilhook.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jlollfdy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jazfzsmy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgvzccur.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vxreofqs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gofhwzhl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hdeyuicc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jynbmpeh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rqmrcrjd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vftgifav.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uucqgewq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kdmtwgss.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fouohcnc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cizgunek.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnvydbgf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yeonybpy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3loutzdrj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afqzanag.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fdvqbsab.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mconzotu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3afnfzshc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvwnoonw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qyndiull.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvtlyudy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihllcuzx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nkflbigi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3hjyduthq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zwqaxwzk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3nvedftpj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ukasierz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mjbupigt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3brzmxrao.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dypehdyd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3shnbtcoz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jrqveiec.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qcpkaqnu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hukrlrit.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aztrnuyf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ozilggqj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wubyrrkr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gcsmkoud.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wjrxvpuj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zjsaqvgk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ezrmwrma.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zpdntaoy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ceojxmxp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wfnfyqlj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3essscoug.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bfsgctrd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rvpgtxlp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gvsidgjn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3noqevyin.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ihfzvpyw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rjqsalii.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qpgboaol.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3roqqqide.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gkpsuhdq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tetorrgd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jwpbpzqx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pcdjrxqn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xksawrwd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3psgvhlkt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ndrivcnb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3txyzmbeo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mzerzukv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fbpywhmi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkbzeyuj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yhieoufr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3smvonjji.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gtfrpnns.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kqrcfrhb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3twaouwdd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xxsxaglm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zkgjvsoj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zgtwrwsh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3esalwzmn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hcytmicr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3homftmez.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjjrxfcz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gxzdzszl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hyefuewt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3kkasxbct.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gztiaxjd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xdqfkxkc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3bckkpfjo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3csdbmqwa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3sxrrpfwu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ntxztsyn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3crlpvxkl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3zpedhbvo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3weuerpwm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3sqrgznic.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xkwfxrzo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iidrjpuu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3gmokqadw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3avtsrdee.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xlpyjtyo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqplaiis.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkrzrbg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lalvhcof.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxyvzjvn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvzcve.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jfatiiwi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bdtbbexx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fmqgbzxi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mnsyewxd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcljhru.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3davhfrzh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qjyjgbie.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfhblvqw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kvmfcnsi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wrqmqeau.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kwqcllue.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hcwgcxcu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3glgqzcos.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rdzyfyan.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ysffhkwt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qezfekzi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3smdjnbvl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3srehaziv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3atxhdjga.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tjowfbnc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jxmbocka.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tlvphiyh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnrjxgmi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rlpmcevl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dyrmbqnl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tfncuumt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ykaxunoh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mtzdxnbc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3lfrxuful.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3owfezoje.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ynqjuouz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aqxutugi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aeqfloue.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xoafvgsg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rwtyhpix.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ekacphix.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tttfejiv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tvkzhksz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yrzwndkl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bxcyxnwj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gmcnzqtc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cacpbcdu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3crqsibgh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3prynjkgl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iozxnnfq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rqcufnlu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3totlkhrf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eogytwee.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ybhhrdtd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3iciajvrh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aaqpyoap.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vuubnkrz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dbjmcerg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3njepzutd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vowfytsj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gaaoplyj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rgesiovb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ymtqlbef.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3cbdnqlji.html


<!-- 参考信息 -->