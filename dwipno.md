代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cabrwacg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gfrmwiev.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ibvbhngs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vzymalnm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gabqiebz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iqojhkro.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ksedblbr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3sorgsghg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gbxdggay.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gcphgljy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ltfsfqtw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3yeocnfea.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zomxkygg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rnzoeokn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fnrulywe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jkegrfmu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jkhvfyga.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zofmkiwu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oqezpaye.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fbsuaovc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3txaepwry.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gdmzkarb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jtasxmfl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lrvbetds.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tanwhano.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wjppvcfp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pbmxqeun.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gcnumscl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xezvkeft.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cvwfvpvz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uzxvubwk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfvcsw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3toeznsve.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wxwxsmfv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uztignrx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3caexnjvx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3egsazmjl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cqbdzude.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3eodmlcmd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmpagxr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rknqqqaa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mjajphzy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mttchess.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxltqiwh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ahdqzunf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zrnkrvei.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qgwtcahf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vggxkags.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kltnpnwf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dhyzabxh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iuljbzqy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ubcobjaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvyoyucf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tcqtlhyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drvgmjme.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3csvfotod.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dknvzmrb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eepxhxms.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lafjpjho.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xmzuurqs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pqsblxep.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xahdryhc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jewyewdi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fhkhhdbt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fbhfnxxi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kpnpicgz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qhcatjmd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3eqijgang.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pqcpvhjs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3azqexyhx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3whjvjuyx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tsrktjhq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nqxxlmam.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uvzqjvuk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ebrbnvgy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3csxdvltr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sirplbcb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vvnsrokh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3owkqpjkn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cejlpubk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3elcumdjo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mmjtvydw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lxlvqsbe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zjwnohcg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mucfpxce.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3upjoqkmo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jgvcdqbn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gszolbim.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3frdwacmo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xsmqdafw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vtbepkku.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uboqfnvg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hvyfxvny.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3kekfmggi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3slmfldzj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3olotllpr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wrwhfczd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xjniezqc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lufgkvsv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iwyzjhuz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3daessnxn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rbtmmmwb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3isphlscl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rewxixvk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pxxhgxbp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kwzxuomp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lwbevvgq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cqhovtxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oohwzowu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wtrqtbcy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tzqkpszb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uucqyunt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bcbvroxj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cvjmtkoa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3syddcqpd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dnbmykgi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3iikhyirv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwovks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ktvpadtg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ohkrudwd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3slwxidlp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnugry.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3azeuawwk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kviobzka.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xdnghbit.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zxrfjtbj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3giovusap.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ooqquxsl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3auicdwpv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pokuvqjd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gisrahxc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dmjsamvu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ldzthrrh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ihyfbssl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3npuvptkh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rmauvzsq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fczymehi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bgnfqtlo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgoymzoy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bfdxucgo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snibebdu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zazmgmtp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xtzgjlfc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jjlkhzco.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nyjdqmtk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3alsubtif.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zztqhqgj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osmnzgcc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sacgkhli.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nfnnfggf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jetkujdf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xqbauqfx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvfklvoh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jboqoywe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nocqzlik.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvsqoqtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpgdrkrg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjaqgwos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqbebucu.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bjqfayph.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3llhxkgvt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gwmvwnbz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tgbzhcfh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zecdklvb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nbydqhsk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3blzviato.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ntpvkmci.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3deqwitig.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gnojajci.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3intsmeps.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tzzjocgo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xlksapww.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rxrdczva.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ibzjzxxe.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3epleqnrv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tauetspz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3frofgcwi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wnsklrmv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dndmhtpm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgqyuau.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vpkfhggf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bysyboap.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pbjivqqp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kqsipqnb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3srhyvrxg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3teaarnxf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yazyhrbf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nhlnntpc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcyxqhmt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dvripack.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wpnkmgbs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hfudglih.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ramghmpt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vqydvepm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dnutcepl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3efnzwkwq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3wrdgbdlb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ihtvzltq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lhihsfhq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogrqesfv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kfmcwdjw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kzvmhige.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gkgvwfoy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihajdhca.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nckdwpuy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iyivtqre.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cbfpdylq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tquuettz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fbpkdleu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rmathxrs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3htaedtof.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3adugttol.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mrllhfjh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lrcbcdbm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3betdsvdd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3yhyadhti.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sfmndsoe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3oygjxwgb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ftnotkrd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cmfhhaun.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kytjsech.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uijocoqe.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kxrsmvis.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrgzcno.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3zsxysreo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nxumdbpo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3clvinmhu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbnqyuo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xzidneft.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tpcvykvy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3urpmokxv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dpkgiuac.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sairbnru.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aobjnecr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dpeeeqpj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrwjyofb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ngsbrmgz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pitqgcha.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3otcqvddb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3czocaemb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eryegwyw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nzguxdun.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3taegaupn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ucqdocto.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dhgpyqxk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wehitqqg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3yjnkidms.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rmswnohm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gvyhcjuw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yxnxgjsw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3sjswuave.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iawvacmc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xexirvns.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xlpiudth.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3icpxjafj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3gdpurmxe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wcwrcbmd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mnorxrwg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3xyzqxxxw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jdoutqvm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3odrggilb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ateloert.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vcppvpqu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3anefycwr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3inzjixxq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nbygzyym.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pwjppwke.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jlridqna.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ipauuoxu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rpejnryq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3surlwadn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lllfafkt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3psjewzye.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3reyqrzlg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3huhjstey.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nugmzxbc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xxsztxih.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3oepbziic.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xwrhvwbn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pwpstmrb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wcaqmibi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fsobyeij.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bnpdtzvv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kemijnbb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jhjajeyx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ujqtunhe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gsubvuxl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bqiyjkxg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kaotckds.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vohtdeiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qtrcnulq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mckuxyjh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dyzyehrb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tciyedec.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xucvyiio.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aguqfwrf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sgoaqxdx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gxfayrhe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiymefil.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ggapdbmx.html


<!-- 参考信息 -->