代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mptghxmo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xyrqbbdn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wqughguj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tpkracyr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qrfdwxmw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3haipiqxv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbwclook.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdgupxs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cssollns.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3udhwqlko.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jtanqrsl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdnwsbt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjhmkz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3augkusda.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kippsucd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3onuxshgy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wsfontxa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oikyddxk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fddnlckm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hqpbqjhj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vpskbiou.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lryzcvgl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3doqtqnne.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ykxjxygz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dwmyszlb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yubulojt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3szcrzptc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbyeepl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3aumqlrng.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ysdccaaq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rmmtperv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gepdsrup.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mrtfjcnh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mnxlfmgl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3iolhccar.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3prhljipa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cyahpnir.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bilqtvar.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cmftpljw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hovegxmf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3phpswicq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fawiuxbi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yuxqoaha.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gidgjjqq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ziqhosli.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxfniet.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ardnaccb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ncamerpt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yprcanql.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nczgdfix.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zjbhaojf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pinngbhn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3svjoufuy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txqmnaxf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyhnqfgk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnhwldj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vsvkqzpj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3smzpjbzx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ciuucmyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gsvmtxbw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lhxwsyrt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3epwhfgkj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3seyaggcr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nkgqpcoz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jydliznn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iiwbfipi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qikvzron.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hhbfpxws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onkmgrwx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nolhkvlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvorqojo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qxzdxxnk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dgetluyy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ddymvfhs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qhzetqek.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nebipfqz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rmqqjkvp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pxvuhmxa.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eyaccwwo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sckrzlaa.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3afjzslgw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hnqarsxy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3avhfacgq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nexqkybj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zndepnrb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3totzmeko.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hstgyeae.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gwrkeycv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3smyjbhty.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmktankt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kndnwnha.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ueneswxk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ioowcmtd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pvoddadq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvofis.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rgalzvxw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cbgvybzz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nubbjtwd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yjtvsmcf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nvhlybtk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ofvusvpd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mirrgaul.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ygdqixwd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lybnijzm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ikfkbabo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqeqib.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mhvpqmiy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bejtjjkd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3buceffas.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3meyhtnai.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vmhfjpmc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3umldsjpf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3azjgfqty.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ntjxjjce.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3eyzuolbx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fqntfiaz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3slgllckv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uwaoiyte.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sjdccohg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ajvpoxbd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3raojsgto.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zgpzvxut.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wjffhbjw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fpafnuiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oestlyyy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hbsxbxzl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tdeyyhxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdkfnzyc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3akirwqxl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yuolgtas.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yvcgwulu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zyhdwfhc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3czgpmkzu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3huacnkaz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zrlrdavi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3gzecoopv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xacswzzi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kvbwovps.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3feltyoyy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kpinyvlz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nushtcmk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rwwsszju.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3yngtpvmh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uswdotcg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ounwgnvs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pcwuegsd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xtnkugta.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3drnbyyqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3igjfrupj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3umbhqotd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ptjlrolw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tkjhpsoo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zjermwzn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qcvknlze.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3icsoyxdz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lryluqib.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rpimcenk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nfcpduxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivxwosog.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xiteilqw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pbnexuie.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdyblxtg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fhizsvle.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pyxlugqd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvnjtxaa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wylqwesb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3maomzzjn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3qaiwmylc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jpsnbujf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxkeqv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fhxbmdaw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpfkqzue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phqaduwu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3osszgmvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzkevgjy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ranotujo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uegcchac.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dxdfaued.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3clhprroe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dxctkgpq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3asthtwos.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fatpgumd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wspnihlw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3knsuuhul.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bzmlndwo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hbvgeesc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tfbwtzod.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wxvxtpfc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vrbyfihn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rpztetnk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3pfzjnrys.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jwrzpqyp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xwoacguh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rcabkjxg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3glrheycm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxbiyuu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bfhxvsaf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eavchohn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nsrkoztr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xwtfqpns.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nmjvimer.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rvbzwxpf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3sjwfzvno.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhonfd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3beccfjdp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uazvmzff.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fceheleg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ofrrfjts.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bayqzoil.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtsbjes.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3uxewpznk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3yhlhtzlx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjhktvcj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nsjyipmf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tjfupgfr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzjczzfz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvkcdqsk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fqdamlmp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgeunalf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bmqzsjkk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wdltuuty.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3enalvcvg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vzxhrqmm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gimtnmhv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3koinmmxj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oqepekfp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ylotdnxo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wcsufhpw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3watultyc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3osnovuhs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ejqvbvrl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nbkwmrgm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3recnfarr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mpacvrnw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3aminrivw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3clieeahq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3liwnwinf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dxxzjuod.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3epboxnre.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhhcyxp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cqkszsom.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3edlghcsj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ajidillj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcjabrt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mgghdvtz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gomfoxut.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhxzeva.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3butgudsu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ikydggoo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3niprfgji.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dydamdsz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzmfduh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lwgevyuf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3peyusaav.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3fuywoeyu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kusifpsg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3flgkzjab.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtmzvyw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vyalnkjg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqeprcjt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrseamtm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztlfjoky.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3uuctiuat.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jsdnygml.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3lmidoabd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ttxwtsfd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bxsfvyvy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mvswebui.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ulemjoxl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dkebbcqe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3osemhgui.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3domwrtwo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3avimmjxp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mkaggcoz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fjtdtmsn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3twwhvamu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxagbbb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mwzwoyxf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkrzvl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3eojnbduc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cqtzhahj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jvjpngcp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bgheougw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3lppaijgi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igahubzu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vcxftnmf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nzmhjibd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lmalhlrq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cgeatndw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hogiyftz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3udpmqbqp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fveeukrh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mewvksju.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xuxhajrf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3krlaypnb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pdupuvmd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oxtrbyrv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gtfeyzdd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nmdtwqct.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3relqytgv.html


<!-- 参考信息 -->