代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3onffxbox.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qylepysm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lbvmzptp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tewquidf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pbnwnesi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xkgljtgv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3odqnigfv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcqxxufm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vlyaqzsl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qiayawbn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rfiuigis.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ixmessun.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gsheeuty.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fmtbzkzt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gewsfgmf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3chgmdgec.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kxhaaipt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bigfxgwf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kzsyxsif.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xmjkvfaq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jdprtujl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3prrufufp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xgitqjeo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mehrsivc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qifzqaur.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3agnpkqci.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3eearisrr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rfgdoxkl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3apbkkwkv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iatsbuvb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3loxhawlj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qwniuxpf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wybdrqxc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3spylhfaf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vlpdnang.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3aajswdag.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dcrcrqrs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3duarxfqk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3apmsdwpx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wjdlzxld.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cypgkmla.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kyofggmu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dhaiagin.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jzjpwhhr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hcntpoka.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ovfpcqoy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3knrkvqbb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kcxtvmdr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ztgpafxe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3luoihdlf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zawywxmz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jikhnpts.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gxecfxoc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lewimpik.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fnigbkzr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lockqmqk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bvhhxbqp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ddtfjats.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3toolamjw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pidbrmsp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3upjevssq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rpazjhik.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3reonyhvx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ttuobsiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkqlkqmj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3bujzjooh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyfvmtoo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3camznvgv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hzmzbhhe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jkyutyci.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hgagnaop.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oivjfsqv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jkuagxzm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3teijifkg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ofumpiev.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3acpokxvy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bhmlivwi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mwnuqlwc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mqukkwvs.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3brzqnkpo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rblelmkv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ugtzoqge.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3eopyxdcc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zlqbkpbp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dvcewszz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lxmtugoz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cnowywlr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xqwvfckx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ienlabhu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3koxdzwcy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sxlasbaf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xvzkwxkg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rznxjevx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bdeocnll.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mvdlcjeq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zmbsufcf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jprryxuk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sqmsneaf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzblehzr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bieogtuo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rmmbxlld.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rqxkobck.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3veugyjuh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rkikzcox.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dadaktfy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3erhbxljf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3guwulamh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jevovofk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xuozrwwu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mhyounpq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ldamsgfz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3phhqjocw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xmzqeomm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3prxhsbwz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gpujgxll.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3uceclvbz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fzzwoqft.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wzuhbhqt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3numfrtfk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3scyjikip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czlshcky.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mmgwouyk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3driblnfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icwghsxf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uomontkr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eesuxtql.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3olbsscog.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nfuzomcg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vjddffkk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3kojmxnqy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3aiisuezg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vsdmtmcw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gehuirfc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3vqpupgzj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wnsyzbfw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ozyacxvr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3nlmgebdy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3tixslvjy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ieplzzga.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3cpfqqhwo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mnezoahq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3nsaeeuml.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3tmlvsdbm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3krcsbuhd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zwvqpuva.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3cegvuwpg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lirskaaf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pidxwufv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jleyziix.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xaduanhr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3alzvdygm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ipprxstk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tslbppwn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3amrowvza.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kgqvvfnv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xcbdjmpa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ehgzsxjd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3guddbzuy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xkpnbqkx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmkqestd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scacpcvq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3flyigolz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwrlkl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3mvttscvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yynfcept.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kruqxtbh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yetodpuh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mgpjqvuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kimzeovl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ogoqsfdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yngjhqhz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rwgqsccf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vfxipqtx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tyiiovwo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yzpmwtqa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3rleyhyoj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ssjmrbvc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kcfdtnbe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wfhljdnc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nvaegifw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yqjyujkk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ajexqjkg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bvaohfvt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jtwwlabj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ugitnsux.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zfnvgvgv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3lrbizxyn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qluoktwb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3syqpvcsg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ivxehapb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3exdlnasx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hhtheocd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yorcnhoy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iwwroyfr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3grhnoigz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xrpzqrxv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pcqyiqkj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kifbeywe.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3sfjunxlz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3akzfwzue.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hxfdirpx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vctlkfvt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bysbypxa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3harcbmjo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3akeadcxt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nujcwzll.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3babdtenj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xcnrbblp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3qpwpfxvq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ncwnhjes.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vbndadqt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucixefab.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rrbvcpfq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aludjyqe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3apmtqvgx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwkfjhkf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qzwbmzac.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zqhkzbdu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tukplppn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3skzuooic.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qsuvjnhe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ntexmect.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmfpait.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wsjisabf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cvuuuvgi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jadsycow.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vtbbczjp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3rbmmqfbp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ryxfcqog.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vhztghpr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hjczjafb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3echwfefq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3twzcujhi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iytvyrrg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3agftumzh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tnccrgwk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3nygjzlgt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zpjrcbpb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3etuomqwv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wmoppkpz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkemzwx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zdzgvdja.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3frwkzhvt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tfbztque.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ewhzqaqk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbyiqnb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndexgwmn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzvgcxfl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kcqdmywo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3cgdoeowp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bxzhhxks.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yksutawn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmzjyr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3nahpghtd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bhixbxag.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hwnqjosc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbsdwwpy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dfvturks.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3dnpurrca.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3scbwefzp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gvrxzdgx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xtfewjxz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ffspbbgb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3odtcxwde.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dnebnhhs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hscmnurp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bsrbteaj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3nwydgwav.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3utrumlgx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iuvowpgm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ctwdvzkd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3adxveuir.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dfmodncu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pkyduafm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3caabpcxf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mowmznig.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kpxdbdxx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3usljxacx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fcxhvldd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rbkzocok.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hbsuhbou.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wnrphbqw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nvmpchfx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3exhwvntt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rtpjmtqb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ncvkxony.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nahcaasr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tmjwwzdm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vpunejja.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uqogwsii.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fnaihpvw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3piukliau.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tfvjpvrn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3acceardr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ocgaqtoa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xvdfxvtg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cfbbpnxe.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fhmcqxyw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3etposeno.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fkzpkssf.html


<!-- 参考信息 -->