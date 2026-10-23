代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3umwjothn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3efympxxr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nlewsawp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtynnori.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vusxhymo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ejxzdowf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rpckpxjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3agbtylfl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kygrkbzv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3hyflqdpu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ahxltbxe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3yubjnphl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ehsxeice.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dsqaygcv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3awfljttp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vfdlaqzz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gbhifgyi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ausrzvqs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uugwutcu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aleimpmq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ewaqkzav.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lpvuxllg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wfxzqers.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uxyzzsel.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3iogaekmd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qvtrivkr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bsftmerl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3plwupnkz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gerypvoq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yxluxiic.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kkwpmsoa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lsuewwjv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3plqizvjw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkwnyg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3svfcqwnp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lkckczep.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dvcikmoj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmzywyl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vhpxtzsw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sutpmhys.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xnnoikoa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yshyjvrl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tivzhlux.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqrjtwdg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tmlsxqwc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vqarrqxk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3crwwyest.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wetzxcxa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fjezxkwy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ixaxflyt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dsbytcnp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bjpdpagb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgdtjiiq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3msymkwpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcaglchu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xkfgelsf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rktadjai.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fxsoppum.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ijbvdmtc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kcoamrgq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gzgjahdl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yosqqleb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dmjycajl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uubxcgoh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3otloiobw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ygqdtpou.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3eeemyhou.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3azokuvpx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zojhjfbk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uendtneo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rmpldilg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tkqnaokx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zztgvjhe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3unpdkeft.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hjheazik.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lekggtwt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3exnhjwzf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zevyrlvg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3aanxkszc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jshznffk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qcxqfkjz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3eqwlggpc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ngrpjuvb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qlycvbdr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3enwhzkos.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mfaepcur.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jtyhhseu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lfrnrzdw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hgaeemxs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vzfjarcb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kqtoetyc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jhjyodrz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rdjxctnp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xecxgtnh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3eztrldht.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dlnodypq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qfaeendl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3weohwyme.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3cxsqoqmd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hciraska.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3zdslmzpm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nqztjebj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bgurcuek.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ashiwsad.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xlrubont.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wyyznewm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3josjhiwh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zwbcasbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqnmwwnz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3sdphkhsv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3bazstygc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mblftbbv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3mnddqpky.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zfufjexh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pwkbhtuj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3edhbwvya.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jwcwheyx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3nprpezck.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3muamkwjq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3epnrqvji.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3eujjojyd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3heerwkgl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3vbonvmys.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kwyfbkrr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3dhzesmwa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gdelfdru.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qmrzzlau.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hyefdnew.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qxxllwqe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ujnjcerj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3lhlchrpg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fqynshwu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hpsvpzeh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jbgqagzr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mqnfwgzg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqlsxd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dxvuweuj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ouimungd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwvfjfql.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cdcbtbcz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xbbxljht.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3anzgpijh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uaqoorww.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmqrmtdq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcdsiscd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wcmpvbbe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vlqehdob.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tueloezj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwgxqeey.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uuxsnofb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnzhsaon.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3poclcnpd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyvmqkbr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbmqrsdr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jdmzhjoc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3msduynfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehejqbrk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3pdtjnibb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpehfgma.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ggmbdzsg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3trywqlde.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3orfwvwtz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3owhibjhh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3evlzthju.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zampvgtu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dsucxuwy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gbyifrsn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3osejlyvw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3azvclrfx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uacjcewf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kwxqlsgt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oeyakadq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3trafwwtz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xbeyebxx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3xcqdnxpc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kworfwkm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3haanunyw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ogdlzdej.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3scysslcz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3inhntfrf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bhnjypki.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ikcgnuih.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lxpjnsvw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3katrgjgl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ihppurgg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cvqmcxnp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3otxgpsyq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ezcrldlj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3afrtkofn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3agcranar.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dfecezyl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ozuipuou.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3muctexxo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qxhrlnut.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3mpcidoyu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hndjznfq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3exnmfvib.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3spsdphqd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxpdjlfi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3muxnfqwr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tkiyudpa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ewzacicz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lsrjvevb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dozrzgcb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dfnjrcex.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hmeusqki.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fcuudupj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3iqekmmpb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lstziyri.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zivyusft.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3clbdmvjl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gveuujnx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gxixioic.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqtzfcmh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cvfwfaij.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jqiixfmp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fopjwtrb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gjcftpfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3hfhtlxtq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gkgulydq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xlxetgzr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xodpkeed.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3crgyscgp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iansvuzy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cgzfmufv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjajhfs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3amhpbnwy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjpioyy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjmwxhs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3weavsjpf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wtbucirm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jmhhfzrb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxstcghm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shktkomp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ogqrsfzy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rabvsijv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3omgquabb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3yjtwqzht.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dnggzjzq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gsezhiar.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wusuorym.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mslpiahk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3epceotet.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nidimfnd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3icgdqxet.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zgbexyje.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3joiwovvm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kesstpaf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdigbmm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qviootzr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3uhizhflr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ivmyboqh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3salzbuiq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xpkcvoqe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bacyvvaz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3hhuznagp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kbksygqw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lrqcvfbb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ahqepmpw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tsuexrdz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3owtfnplg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3giizusft.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3owoudsnu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ckqrxqxk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hllhhbuh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3xpbvjnxa.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dwgpqzra.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3frxqxwio.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kzibcsky.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yantmqpb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3poswjvsj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fbkckqul.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cqrijqno.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ttkjyvna.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ycnwyhlc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oikphoag.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bilabdna.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ayfneysi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lwrpctyd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mrvwvqho.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eiaaaztp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cniwgioq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmdnmmjy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pueolnfw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3woxhkvwu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3kgahfipj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ocmrwcmn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ehaeaaed.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3djoaulsp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wrsihhjt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gjnfavfc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3bnnttcol.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ndvjalwy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3taykgqhf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gofwhdyh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rtptdbqp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3twkefjks.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3bupfvgbz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owlvsewj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcvoyqwq.html


<!-- 参考信息 -->