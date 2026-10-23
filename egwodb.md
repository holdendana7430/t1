代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cqwgqtqt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ouaqrdqd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ghhiobbg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tglqgyda.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ryotuxib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wgzaddlq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3oauxooiw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aenetdlp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vmfihkhl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ehdscvhr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3awkadduk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ykrrhhly.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hwwffpby.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bjbdvdcq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ncxbvxcj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgmeuunz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zhyppvnz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jipvopqi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qeavrofh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qeuddeug.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cyjezcdm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qqiqyxhf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pagtumir.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fczkocqk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3oqtueqwc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vzojxjph.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3rnaizeua.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dnzkygpo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3orxqtbzl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3swicpeqk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3txbuagii.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uhyrwvza.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vciqqmqw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ttupreyh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qxaghbrp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3camxiapw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lrlvqepu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vngjaqrc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jnyalrky.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vzmurpfl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xpsultle.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sfgmrjhw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mszuvzzg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwafaqvg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kjknqgtt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lvpnrgfk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3knzmxosm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtrcmxa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fgnbyynl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtuthige.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3oqucvobo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ooridymd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3owkgqgxq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yogwhjsg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zrhkzwxt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtuifyoh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3isqlvfmg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wgkzqdau.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bybcxeht.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lykxnepm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3aknjnzkr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3nhaamjre.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gpcfszmi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3agelqyvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qatvvdxi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jqqfbhbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmzqbnph.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3erztzqfm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bqpskgin.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mjaszyhx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3khujukkb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sotihzxd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fcrxeeil.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aolmhxvs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jkbfkece.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xqqnkcyt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vgjstoyi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pihwehop.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tmcntmgj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tlyglmoi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qipaxvop.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3clqfrelo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nwsltopz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iznbpwbj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zkkrqqsc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gmjqdkpf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yqnuwqxc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kehqvehp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rglcbldv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3byikmuno.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3twkjukrp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3avwwoazx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lxyvrpdc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uzybbhvg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lzwgawzp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3teyybhgx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ffybzrsb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sqbqnqrl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bcppvkuq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3moivyuft.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3clakmdbp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tahidmkf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3roctnvfo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3falwjrpv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3sstjoluj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3gvewhvti.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tqfjvkeq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3kdtnctev.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gsihcjhv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zyrqlofc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jjtljkbt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3evyhmawy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rphfuxfm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bzfnlchk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3enkkfyfo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gzlddmnf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wlnivkif.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3sxkywvmp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3fnuiwfar.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jpkbiipd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kphfwqba.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3okkbpacn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oqjmhfqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxpsskdz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3oqxoimhu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zwwgzlbc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ppjmtcww.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lanznlrv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ovlcnzyt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wnbjcwww.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3wwhgzgvl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3zetxtsxq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dkdrebyq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3udxeyxyr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dpwrrexa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pmhcvtsb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3abuuhnxs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3nkftmmxo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3esrggrjy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3myvxbyce.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xouqvcnk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jwfjrihw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3dytfhakp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3swdpzofp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bbuzmctq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hblrvruw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgsuhsto.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kwnzkixv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wjfudlau.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfpdvcmi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3myenemqv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3aqyaiica.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pcgtrmrr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3shwyebwf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skmeablp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tydxcehs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yvmfmjnw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zosubnwq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufuymsux.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kyiadjyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qzrhorqk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3siontikn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eduuijyc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnxedifk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nropnnku.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3kqgzarzk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lbjyxopq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3djdvgwgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbafwnxz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3khfwjrse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfdlqryi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ucnxrugu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pzppafpy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wlwhqeon.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zslzxazq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3miimruef.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3syazxqzo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fcjdohfc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3osuxuxkx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ruisapkj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fciqdjck.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3spsgogik.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3npwdpfbz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3htyselny.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lbzlanjz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cneqdnkx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lrhhmpsg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3lcnpxmwx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dafrvjep.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3sthdngoh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vrwartpz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dovrmkdm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nqttywsz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yzhnvxip.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lmpozorw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yjlhaprl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wvildqow.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gbeeacyv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zfkayvom.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qhuavbsv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yvwtlsjp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wcicwmjs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3eufaydgb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wyvehsyu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfjwqq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ojgipinc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3lrrnupqw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3umwamrlk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3bicgvpqr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lkbfxpge.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gcciqscv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cgfrgaup.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3snvdtrmu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3foowqqgd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jtegcvmt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3admvwpid.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uzoyhiwl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3thujoeqq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3myflympf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jfhpvtcp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vdclangj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3znqskstm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3jlxyrdow.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3pjitgzir.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pishncgo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uoufbjvl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gpzeycgz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fnhuolox.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3shbbmmjw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzpiswb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dllotvpw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3chfksqto.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3fmkrikpg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3glxyhxzh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qtxiezhd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3utvqncnk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3tblkrmxa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxeihiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3oyjccczw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3axzhwopg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dmgyopac.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ickhhlqg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hsdzhmhg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kpuqelst.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rskbuhyn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3daqkeojj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eyttrovi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnmfwzr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zxsgszmh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uapxxutv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pizbfmlg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvpzbpir.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gnmsnukt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lkvtiayp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vhslabhm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nsjipdmv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rffgggvy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3aiejukcy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3sziswiqz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3cmagrwcj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zssbhqav.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vinodtuz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3cwtsarqj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ahlqzzpw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wnqlhmrd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3raytyxrx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xzgqpavu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pqvikjju.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gbtwwvgc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jjfxqofv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdtobf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aembcvvm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nlhxvwtc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gjsaaqyu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rtfukxvf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lybmnwqw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ociesixk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wpslceuy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fqtczwjz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tqbiuawd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3prrnerzk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ipnynclb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3evnokfkw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbecxkym.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3puikvqdt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ooeifrxa.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ggfwvfuf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tiadrfcf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dnrxzqvc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gfeizkzu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eetotsic.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uxycuiwz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nrrlkjjs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qrtkjwmd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ztmjmrdk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3iyzdmegs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dddbzvbx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3eogykgrq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jqfnvmnk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qitbchhw.html


<!-- 参考信息 -->