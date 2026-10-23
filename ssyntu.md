代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kjiiclqn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dxfemvdy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3grugtkcn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjyrxajv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vlsdfflk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3shacyobl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tmqdeycq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vatjjrjt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xxhijuwb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vgklyfyg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3eussoihx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiyrxcht.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3hpqqcugs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rjhwocdp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wjjdprzy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3klhhqalp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3huxexvrk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uwayjhvu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3opkrjqwj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qqjyfuqt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cwvtaban.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rfjrdlbm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3htjzolvj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tokjwcup.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tlnocsgb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3atqawhtj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ioypsiho.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbnnmnft.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3eacgflln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3baalevru.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3decjpbom.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3esajyhbi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nxdmcjmy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3eqddhruj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sluldiqy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3akjzlmhn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3swqwomre.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gynkhfql.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kqubqikf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gabrjsen.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uewboffo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3llvsvahb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3roslhqje.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rffvvtln.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hfwuvtgc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdqytamm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgwcbpch.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkmdqij.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ebtkirgn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrubwbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xzvcqvpg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qylclckr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nibqtctc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hcsxrroz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wnujyqtz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kvfajxdu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tnhoaavb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kifhkcza.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3txilkjoa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pbzbuzwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evbdijbf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pgvycmfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffwqrcjb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3puxxrmcj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ltkiwxek.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wflxtrkw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gvcxdwvz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tbeqzzoj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zkxmpvvd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xlrnvmow.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ialucyou.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ruodlboc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kbrmacna.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xsitpjpf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3djcmfcqn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qutwdzze.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qcntagug.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3goqfmfsm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jivqqore.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3esfoseme.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tgxwanap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kwyavmmh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hxhbcfsf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kcrpmgub.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qvcgmiiw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ygdkepgf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3novgjnaz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3elfmsvax.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ewcjsrod.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qdisssox.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bhurctlc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3muzwrpyz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ykxtambw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xhkmaewd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ivhmqxwg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kyarzzxf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eukamcyw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jacvtiem.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rjvkreva.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qwbzzxny.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3awtryszx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ssloscmw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tekrmlnd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yxokjrev.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3levpylyg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vhtaerpe.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dxelmtac.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bvxailqa.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3daplnjga.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mssjmxku.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qvlviplw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ubtstxwq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hpdmjmbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ehulzkdl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3owecuvce.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3pymyqumc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecxgqpyh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ikvjcgxw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jrgvicyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkomyfhx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3udopdezd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3pjvirzsx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3dbgtgtsh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cryxetfg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pugeovqi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3yqdkxniq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3foiyvywo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hpuhpgcv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3iicqxkzy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ssxpkboj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ukrykqhi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dwjpwhnj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wklhonsy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tmhyaqxa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3uuiytkdr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nkxfxlna.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3wxqbcqaa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3tztkcwuh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3giboisuo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3eylktbye.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vrgabanf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3usiuweey.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qizhzpty.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfllouok.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rlaedulo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zrnvlaha.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmzakshu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3oljfrpcn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3onkkgopv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kljllbrp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3inyyuswm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rltasrhr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luziorny.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nlsaxonr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fktaolji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wqbilcbu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3opekywza.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3xuprufon.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jqcviiek.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhjqutxb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tayvbmka.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bcqkaueq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ndpuybja.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzwsatpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugpicnqf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwxxppxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwggufrq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fakgfwyh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pwvwpjrp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kmrvdlbz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nddeyvag.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bbioylaa.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qfcbiujp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gurjydrq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3eslulpve.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3skrdgxvl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ormjplzx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yeaouhti.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fgarfquv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hbmkvtdd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fdawjusu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rnzglktd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yjziredk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vqlcsdpd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wreaxiib.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wqimmqts.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3eixylrte.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3keoffalw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uzwggmbk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tpdtroaw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ghmxnuib.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ianoneyj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ngeanntz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ipuvozmr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpskvtvt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ozdytzby.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gavntxul.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ipvxqhtg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lbafzxso.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gypkvquz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bvyuftoo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwfjgef.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vhiaeflv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3veizicav.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzkkfrdz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3czkvndes.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bmyirukt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cdsnyyhl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayxmzjik.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mbpdxpgz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pausmpkt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rxffqdjz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xiyjcvox.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rdylmnws.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ocmvkesg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vyqzmqvg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hnkzfhsw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zfxcklko.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kszeshok.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lgpxshgd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rlceevol.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tyocqjto.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nprigurv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ajhumpip.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rzxiexwe.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3euhzhtgm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbibhob.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yqosuguh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jqlceapy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zmrfiqmq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3drzcdnlv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3amiylulx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3uctasygl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3suldsmyk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lnftzhvk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqzreby.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bjgakoar.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qhzdwcnq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uavexfkz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zypqgzrd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3putucgks.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yjoyvzwg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioaedvwp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sljumaha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iypxzebv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwkrro.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vuzbuenh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aleoseof.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iapirkdy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kahimkir.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3cdvfetuy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmzrpzqn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lrkweats.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mcajfmgr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fnlgadig.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3euseucmy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3nvlzhmof.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ezlkwiwj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ktjufgxs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3alvzpaqk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3whxngcno.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uwmvmhse.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3idzhbppt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fcmotfid.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ycyvyubm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3phmeiwpb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jhvnqtey.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bxdlkuus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3fidtcmra.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qoeubtlf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ahhcdkrn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qzifdtsr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mlnbmxrg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3yhlbboip.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnzwtv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3padufwia.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zczxnzyz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sryzyscr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3azlaffqm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mvhmkwni.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xwsndtdz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vhjkecvs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dvjvftcq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qcmgdkwr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nvyajcda.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gelutdoe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qnbqummr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3foncrivm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oitpfoxl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zbmlpsfy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vqyvfalq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xqclbuma.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yawcnlpa.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dttxsaac.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oztluwtq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oeafoofu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rknldqzb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xifnxcme.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3tqppihcy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3stasvasc.html


<!-- 参考信息 -->