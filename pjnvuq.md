代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tvkmslmh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ketkxilw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2godvtepl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2chmjtbtc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vjjarpti.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tpfzdmgx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fudkfloc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2phmuifkf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eftcawuf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gnxtlafz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zjlgadim.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehqoldzt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2trmmbvtc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2clexserf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bqoargaw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2oszypiye.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wgquyvll.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xqhxonkp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jwgwqfpq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2putdaiow.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rqpdwrgi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rslpeohf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tnokwvka.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2czqlpbeu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mfzddgsv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cxqaxmnt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cnlkjfsl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2szprxaav.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ydvyzjxz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rigskhvx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ehrdexie.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ovfwdqvq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dnyvcurn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2keiypoyb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lxsbmjml.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2oaktzaeb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rfunpuoc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kkuswsvr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2epfbarrx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fyeiwszd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zjiuhkdj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvtcolng.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mwctsyol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmelbuhk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nzkmyzfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rnuupqgp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sndochux.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2aygkumbe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ldlbmoyt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gpbizjsd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tsnnpqxs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2iueuynzz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2muykzsyf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jyspuhet.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dcaldrev.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nlmixelm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiutdghk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jjdfqpuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzwvozfi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ltiulpvq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lxrfvhai.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gehzsnqa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rjhhkrpx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sahfqgyb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ekemebdt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nstdxodz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfqryn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2punntpvl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xjljoxtg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tmzheklx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2joaungec.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xppuxuqy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ialfywdl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2alfzgrun.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rhezlevx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pxteefdq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2erupuecy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dyzynflh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2agdrefhf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qsubpfbn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2avuwefik.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2smqmzjvn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iejtfcbb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2brinodun.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gnpcytgm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vzhfrnmc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ctnqedai.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2najtuwps.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oxnhxtyg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mjffolfq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jypevvae.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ydodstjo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2flcxavut.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zjswvvyc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yagxssad.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hsylvbog.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bnqgsteh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2brcwzana.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cfeqdwcw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nxnebdec.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gqrbghzs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uwowarnz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qfsbemde.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ctvbvpdv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2akopsgfb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jaaykovk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wpoafaof.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jrllkvqa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2imgtsclc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pgxqskrj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vnvzsrin.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bmkghibk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tktsnctn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2pkyvpuvu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2akurknnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etljqton.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dekkfwpa.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2shrbmyug.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rbytaxzb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nxdaaerc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2edkblizs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2azwphfpy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qepbloua.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mkbnyvqz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nfbqyuvt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2mtjmtlma.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2yrpknegt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2kogkudpy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zjuvnvfh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ylflzbit.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mrjznicc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qjukbntd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jgdxphxl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pcntglzy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qnpkitju.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2chxnomsi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2obhfeppy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2udlpuqjb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eydihgnx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssluvcpv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyilasio.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dswjgabk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oyyfiqod.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxbajlep.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjzupwhs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xyzprsle.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dljwyldr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqhzlcmx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fudgkvcq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxetec.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xocmureu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2arntsxjp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fuhhspfy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tjmojodz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2apgskvza.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dgbhhzqi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2evmpmyha.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tslpmygw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fllqofyb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mozcmurb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxtrwyxt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdapnvzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bombxnkz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tyzwktba.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ocpztqil.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jmmlmrge.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kvgmyfpx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2tcnoyikp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bydmmsfs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhrisjh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2obpcgtaf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tzzledwy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2dwkeuats.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nzltthnz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xuhkmblj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bkvamojl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lezvmxgz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ffigvhms.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2eaqddrnh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zuicqxqs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qidnqrsf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2itbhvksj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mhigudqz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gwhyfzqc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2anqaarnv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ojebinim.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lpmjxnhl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wemlkuup.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bvnbekzq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fpfgzphs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kfhrkeek.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wlosrnah.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2deuayvoj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2juhyltoc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vfyhlphe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wjbpyzbd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vuvrdquu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2abrmgyvf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jclaetwe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2owkfpryk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xydkdhus.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ygzaeqxx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wybaftfd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekkviofd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jixklxpm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uwozepnp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xemlhsdg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gdwbyqhj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dauaenrv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pffjkxxa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2xlfnoslo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bazdhyrt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jburkvzr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mcgwvkdb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qpkfrbfp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2pzshaqbz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sdsjqnwn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2owddxuhd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2lsdsgggt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdtfmwv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fvhthrmp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2isdfsbem.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbkctaf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ktrudmdu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ljzpcoor.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2rvtsdsum.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qponbyzq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aemtqtsa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wolujjok.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tanhwfin.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2lzysavsx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qqlipcku.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nswbvalw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2fpzwobks.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lczzdeyf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2reoekvki.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqifwwfh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nyexarus.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxirxow.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfftlxc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zarcyovm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2aheuqfae.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cuqfkjib.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yzxgfjbj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2anfufmfo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2evjwevvj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2lzcpplpr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oewchtsr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eshavcpy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2awlffekt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2vhmgargp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2etimcosd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2uzduayca.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2paoidwto.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jjqjfxpr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hmokjxrb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rdwunjkr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ftzuxbyy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gvcycfgl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2nhrnmtos.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fowwrdvo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nshuyhrp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dyifarhy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrfkzayz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfgpknop.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2svraywjk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nvoakzcx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vatnzcdj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wobviaqk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fsxpnohc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yntjlbts.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rrmvrrxs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fichfnnl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obhpihtl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nmvdyrvi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bhifytaj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ytskjhwu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yvmxguvi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ayogrcih.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wxcgpjxc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kptwezio.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gwtwidmm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mnyupczx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dylnhkmr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2szmxztbh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2arlxwbwt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2irvbqfxp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2dwxodphm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oyuqnqes.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ouzwyweg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wwvxezkj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2grtzchwo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rqckfklj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wrqgeovl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2dtofjwjq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrkyhlhv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hvycdtax.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xguyqulz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2oxhcqczm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2qwexecaq.html


<!-- 参考信息 -->