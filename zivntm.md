代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uvbghkba.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gipbgxcy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3eweoutcy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kifernsw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqgwwd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vhwyfozj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wewrmnmg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvxgpwix.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sijogaxx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mmjwfjzq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3siifmgvn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bwtgmbaf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rxoxfodb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dqwurszt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3supljhzt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyioxutx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wpgnypgu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uqyjwgki.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wmyfhtnm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ncwxbnpv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jplsqfld.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mlhagskm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kzueruqu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hntrtugi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ctqtvmzr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jnrefjov.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jrmrwurt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3eatjpoaf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sxmnqong.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3doolfshg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3noorsyer.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gewyoswy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tathlaqo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kpihyltb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3diiwupms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zfdbwgjq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3quhgnkry.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqjkrav.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ssjjdytl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xpdmaxvx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nualbdrq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wrtscxtl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3irmjesgc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3igynjxfe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hbrtqkkq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qpslhalz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3oavbhqzn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3snyhjwxk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qivaqrcc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvxusemz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3acudtfyz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fukynfbe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nyzqyooe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qfoxylqe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qvboozdv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rjnpytqi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bpvouihb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3blitbssw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3acczuyix.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3uzltufii.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bcppilce.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xatejahf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xxqqsyxm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nrtnwhlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlgnbvuf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3axyoqcrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qocubksu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ktgpmpcr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rnacohmk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3icdbgrqf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fkdyruzb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hioejtqk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mfcomkrd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qwcmoojs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cnlpivpr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bpvtdgah.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3riaymzvr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pghbaytf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hezjwhwg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tfjnfzha.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vcaywreb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ampneadk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3heledooj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yiayldnf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qbutobrd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zkqzkncy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3prvvabmg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cyoqlxqf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3espgvsas.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qmuhlemw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kdighxsl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ficeghqc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3slwvrqxm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jhnfhtiz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ixhdkhlk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wfzigslx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uaxzjjwo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zrudkklc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kxkaxven.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ykszdemi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ulgrgbsc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3laeepdej.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lwhvzegs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fsmqwoxa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zjfvmobx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3gryyfrvx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zfbnyngx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gecqfgmk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qzmfaozr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xkbblpyt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lvrwgkta.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jmbtnncb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mwpjanub.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lcgboyry.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3tjfsbowu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xkkyzxfv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ttopygaf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kzkbdqkr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3tegiqisg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cewiqrzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgnpcwlf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3oxohampa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ozydshmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcwrlmtx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kmurthur.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3arihjbpx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3msplnzsv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qnnitjkk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3oqkarckf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vjnquffr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tymirqgb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ppeybwes.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gbnvlhhl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3tpkxegpm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fualvuuc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nhtsolwx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jhtzeupo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3odhgxvla.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ymnnymru.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3twbiyuok.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3mutselaa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qnyakotn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pqdetygf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ltwrurqj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgkftoqj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3zjiksezx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lgbrxfhu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywtfgasr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzqyvwao.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3brfyuybc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lupmkmks.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kabymdwp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pdszcwdg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uydllcao.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zoxrlqnx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xkbiaesw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tiumqbdn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ozchseeg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwunahzm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jnaxytlx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3prwsbqna.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lhgjphhx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udbnxyvg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ujvnjjxs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kubkhcrv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwafxymf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zgvikpyy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ultrqwrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rockvpug.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwozupsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjhevgmk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exjcybbr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mccmfhzu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3amwnqsyj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mflwiczc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvbtphf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rymggalt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kcwzqbdd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bemznfsd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ddcqintv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gmaxluug.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hnrzgvjm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dhhtytnd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mblotkyd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hxlgdlrv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tcyqxnvc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3csmgdvbg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3brgeeejy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ykwpihbw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vthismqi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ufaywaxl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjfuspzq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hrejgcxj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uldhuvqd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gtmvycfc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gibbxbmz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3isradmji.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nopgxfam.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwknlbog.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3yvjkanga.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mafwdusy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qlqhrslb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zowcgytq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vvntdpit.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3bbdcadew.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ljutibgl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3iqcqzfqz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3imaakndz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tsvbrqip.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rprptjql.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uhybcdvv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vjolpntk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3csbctfyp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hyqwbuln.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gjyyrvgj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3auipkqqp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3idmxonyo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zmrumpmw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rxbdyene.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3izndujwv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pgfcchun.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hmcvxvre.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ujycwmpm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qgpwejcc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dawuhhns.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cgsehvmy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3edklaawo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3krplfovt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zsabtymt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fjfeuyaj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3tefljcsm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ybwcgtkf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hhcjezak.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kvprhtfj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gpihmroi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vzzhbqsm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zewquqed.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uhqcjegu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xgtcxznd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iiysipua.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3doelxjzs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3wbflmuet.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ocwqlfey.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kaqxzlmx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxdsxmma.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vozssoye.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrlfxnex.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xbtlxclp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ebegyhbv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ybmaapol.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3cprrogtw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cguikkkm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pxexnyct.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkqrfcq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ipvsirhc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gtntvrsb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ygyydrmv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xsrgepbc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bskgxial.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jgonncgx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3knxdkgnd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yqvjppyu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3delddfhx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aeedkonl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nciolwmh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3utacrvtx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fytwbnnh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nkokghcw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3joslbnfv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zpedfsjp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwjqylgt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3buhwljlc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bbidljix.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hvqhfhqi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qfeppyyv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkqgcls.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fjqyjffs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vhlwzzqy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ktdxlysm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3okqqjito.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ebfoyvaj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lridwazw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vezpeicn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3swjemolc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvhadmtg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vcafazak.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gpolqeob.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vvtnarkl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nsrihwmy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fiubyvul.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rydbhmdx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lgoapmea.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tfgqeagk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xzpcwkec.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vhrxhetw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3veagzrer.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kvljqgbf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jnxmrfft.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3skqhrvso.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pnnunjkl.html


<!-- 参考信息 -->