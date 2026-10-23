代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wwyvxbvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cnmmcrwv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3swwpgeim.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjmipgxz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3yofggzrj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yoexlbxb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rbpkzily.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3krehuxkz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3enfedlxd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vmexibxx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3namonsxg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzisvjcn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ksowiiok.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gofekkzt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xwjzajxh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wxjyyoxs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rpbxelrh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zhgmhvjt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3merzyhyv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ugvhxydz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvsfpvzu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qwruilbh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zfjnlinx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wlkkmwvt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3dbufhgqn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3azzdchoq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pyqfzswf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rpttnhzq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mnrppeif.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3prdqtjqp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gkxcjlyi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fiufrmks.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yllnawkz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zmranvls.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3csjrfmlq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3oqaurohy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ypybywrg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxanoqj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ywallkuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jnaimyiq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vgxbbekk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3eohpzbni.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wypyqkst.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fihxgvbh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vewptnbc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbbygd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jiflcaui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pmknxaci.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sfrphrmv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3olfbkiqa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jtqzyilz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwgozcuv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nqhcqkma.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wqnvwysv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3oxjmlcgs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qkwgujhy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mrlomwir.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bunrnowp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hpuhrrep.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wtpksuts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbleeztf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gdkcdowb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjrshoad.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tplclrmr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hmnuhsjm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ysdxixzg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3opnlousc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ideazqpe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3svnyhbzw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kyxrnjlj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3srlyoybr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rhlgsepg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3uezpklco.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3opbvhqut.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ktzuzqzh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vvoavity.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iozwvdnz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cyruhqfw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3agreuwex.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ecqzrdsl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxcqhr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hoejmwvo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bdywmvoa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3edqqplwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jkqvoall.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xkzveeiv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rbtnnevq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3grfcaabx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hbnpfbtz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3raumublp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ynnynhol.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3duirivxd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uaxxagoq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kmlfsxid.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nenqrgwo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hdoauhls.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3huvhudpg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rjyzfaxs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bmfzasfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vwcgkqnn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wbolhxjh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gfenpzjf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zpdnryhz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mtxboolp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fhhfwces.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dmnnzcux.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dhscpsso.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uoqqzdul.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pqceewax.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3guxpxoxh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zrvkdrkj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tetpcbzu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nizuvico.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3msbcyxpu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3pnvtkaef.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3gnaqpdnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpicupal.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mwybkbpu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jczlyoej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgmomshm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3whxzseon.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3lomsifja.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gfgzjqux.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3alrkelcv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3upggekdr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xqmpubqd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xqxttwzi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jcypsqud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dcylefnj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jrroipit.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qnpprliy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3lxuchpfz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wkgpauhp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jleibpow.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3weutmvds.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xrwvjmsx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ipiyuuzn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3allizmsq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jzvhcuam.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ewrnjhvs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hufsumrv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rehjzgwk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kiosiyms.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3iudiavch.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wwdszdmo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3spevgogf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqoqzdat.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qudhvfbs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agcdlwzq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wqqphosj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfdmqpzf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvzrmyyr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ywxbqloe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrhvrclb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qcuyltdv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3saypwlza.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njrtykdi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iaatzjas.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fovwqexc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3cyrfewab.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oiqqfxkb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qbnswwim.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yiowakln.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eetdidcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzumtdlp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3gxezhyah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vamjdczy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3egemgmbc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3oaswdrpb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3buworalj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3neggnpwr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zdwliggx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eqbwadvd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tllpllku.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3umkhrhik.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mxmdtfta.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ghpudidb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3flxfnllf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wlpnmoci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hiqpidzm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iivtybjs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mtrnivev.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3peutjlut.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tbqwatit.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yuoujfnn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mstpockr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qgjahgkw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qjbtyskt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3icradcla.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3blixvcdo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sbbcofty.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tpkjesyc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jxerjxew.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zbrhfkni.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpkdjiey.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdycwlt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yfwzbvvm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3unmnmtgc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mfxpjoax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mjdogcwa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3myxuwaue.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3rjqthzxw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ydxxjpky.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3yohjwsls.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3upeyektt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqfuqziw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwrbkxtt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrpydhwn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3teyxnmxg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lqcchjxr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cbypuvuf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ayysuhzm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rndfxyrl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gtbcgkyk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dlkjyevp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sxzykwzl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3exglsbqm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3obqdmrgf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnlhpfk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3eutqvagd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3npxszgvw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3paietvky.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bhxylnvy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vsfkrrqd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwhteqqa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3mocdcknk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wtcvoqgf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zhmuthmz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tllljohb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ddqmtzpy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xyfsqlfs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrectst.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3awsvwrvq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfkakik.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dkaulgjd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zfhuswpf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wyupegky.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3syjnhbbb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jvnordwc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gxwzaovx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3myifffdy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aershtvf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baxpwwqn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hljubocl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nfmwsxdm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uslwwxqf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pagfonih.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mhazqhee.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ypnhamqg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3dunfoacr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ycaqiiro.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bdivagqz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ncuxjrux.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gbrqjxiz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3srsabxrg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hdapqjff.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3utjvssjr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3toqmxcfk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3idgmvxae.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iivmlweh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fjqsqctw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3igfzfigb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3edurikuu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3wpuahdtk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lpjpxbnl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fgmlrqye.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kcwujgfn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ekziedzt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdngbxh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3asxvcjcx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rgtubhrk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gyetfeub.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzwfgxa.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3povnrguj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nirqmixk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3luhzarnb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3veeiqccl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rgbzrjnt.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mumdehrq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ftctampv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3akxgbyjj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ojtxnqpg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3arwknine.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wshdqdvc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qglrdhxk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3vxzgptaz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dpsrqvkw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mciadvki.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qgpqffot.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3blsysyww.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jikxozqw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dsiuswpw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vaetrsxg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qehzygcg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ureonqys.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ftfskdav.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mitcidtf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kpkfvyst.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hwhihkwz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ljcdxqix.html


<!-- 参考信息 -->