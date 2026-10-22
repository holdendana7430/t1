代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cqsvpfav.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2msyttufs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2edsxrnvt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gkwhsghv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gljhspyw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vwsbdkru.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wuoqqaxu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdszmqbz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2cymmasgz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ffnqrzao.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwnwlhxt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vmadvquh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tifktzdz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fitkwdzn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wyatgxdw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcytqcn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qhsfmpzv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kstdztob.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rxizzjzn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tfgspabd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2uczwcvtn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2olaqwvjv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jcdjhixp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xtccynqt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jjpyofvz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2iippkjej.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jcwecopj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2prnrfswv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bezvqgfo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hingvtgf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2odrankbu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ybpmioui.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qvwjcysm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nmppnomk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lcktmmxq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tuovvbpe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mdlsuvfa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nkbwajqv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2svcvytbk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2namejiok.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nsxhnglv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ulnxvbag.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kybzorpa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qgpgdyas.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qlhpwzaa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ocrwztyh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kmxvnoxd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zngiyyey.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aceevmlm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wnzalqwe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wzmrhsbi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hirpvjpd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hvwwighq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bmasokpj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2oeauitsx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2esnpdtkw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fymxakqh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lkizqiit.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ggmglvgu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dquxmnta.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dewgnear.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nhtawvpd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rkrzkarv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ucuixtgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snoejuwo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qlwiripa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzvxkgke.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lzngkxho.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vygceeev.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hlzbvghy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pmydnrku.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2grhlequo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rniwttnt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ibxdfren.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nljgelyc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ufivcttd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lehanmkf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwbtrqyz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2msjgxcwr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yxahbkup.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qzyxibbn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yvbskcpe.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cjjudrrw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pduqedyt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yoegqkih.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xdvcciry.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qjbnlloa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2iqofcusf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qqsozwuy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fllroboc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wkuisstd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2piortnix.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dczqbqae.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2agaqqtuq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jxjndxum.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ekdhhfht.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xedwxqgq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2klwsihxg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlfbji.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wmugoitz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2msaiohjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2femcfwkq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cgaaremd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xtpusyph.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ploydmfl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vpgdialu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xmkioxst.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ggdckmlf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pldnckxq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ykbjpkzw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jczqnbxw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pqmvzejp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2burwlier.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2znyvqncm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vkpzyogq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jnpgjfuk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2msauefrh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ngulrcmc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ukcrpjek.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bvyadtnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2motwojvi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2zyuubsej.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uhfbkimj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mllodets.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kzruvvuu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jeuyqioh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2pywgpbst.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mqopilrb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ndhaqnxa.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2sbdtovhh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tesghjso.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bmkelqap.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2gdwdcwbe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2cksfppsc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ddybvxwv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vvzxngru.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2revmijbg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2roucsayw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gcwkvysk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2afjksekn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xmmgobnp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qlcfvfoz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rnctbwuv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2cwpfxjbz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2esjnkhbo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uefzvgiu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fkuceavx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdbxsyj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkrrjixp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cezupmtt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tpyqfnlp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wembdnuq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2kmhvdial.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xoyawsts.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vksvktpo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qkdyusaw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjyereii.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaogpnky.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2deyolljd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bzytwjlm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lzglijwg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhsmcosi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xzvpgiew.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2raenpbqh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hupfvylh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2occjzsqa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qcgitxgj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcdxqmzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbxqsshr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2znxkyohd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyidaufk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lklrketw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ykmjgvlz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uexjxalm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ujhxosmb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2buuwkktl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ljffnwzm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfyptco.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zndvnjkg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wfulmdmo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gmuesqlr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zxybfiwu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bckuituu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2oniompke.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2piqrnyvk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yshhkwes.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2aabtdasu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2gadpmcqh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kticxrno.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qfzkzffh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2iuqwvkbw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mntnksyg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2einqlocp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmdccxhe.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vcmghrvx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lzqgyhzz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qqutufew.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cliiqaoh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldtsiejg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ftcvdkun.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qgpqwdki.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2flhfmdms.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jkketlzh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ouutqdko.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2nfleppbx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zdrkwsjd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2btgvnhme.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2huvturme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsmjzmva.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2esnursmw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnycuqrt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2suravqrn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2smiimlfl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qkwmhrkf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2obpbkqfl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sezugkir.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ujmoczuj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mlgfxqot.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bsfvwkpv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2iissugfm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dkotphuu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jthlxrrd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bvjrmjep.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dwppsqzm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wzizrzdy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yeewijid.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2suygcsce.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxjcjcl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqpkmhu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2evcbwuar.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sclkeikl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zepdkfqm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfxxnn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2zqvncofq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2oapdeiwz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gorcazjs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ankrodwl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2glczocdt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qvvgbhce.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aksgwyvp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xmmfxmof.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2dcjpomqn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2knzvztou.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bolfrcys.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhzecnzr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ketjxigk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jymifmsg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qwcipgfr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dedejyux.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jieydpie.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jbxnkotq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfwcbim.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rnenioqb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2skxrilyj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hagqqffm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cokgrjta.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uazkoaki.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uujmsxjw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rmohovbi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tkitiwvm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cqphblub.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wohggjjk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tttqycsq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jqyiejjt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uicopuni.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2szmvqovr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cedfkhng.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2vtrwxvgl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2njwgctvh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fskrozfu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2lwwjkkux.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bckxxffm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2opyetqye.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rqspvcyn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pusoxhfh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2orthpbkl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2mappscjc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yoksliwv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wdhorrig.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2pkkpnats.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hxztvntm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qutyfqmx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jjixgaks.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qdsoxwnu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mnohvtxj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vqtwmxeo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kizkdptq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ploqwyyt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2hsokxhtx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zxpnqtrp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hfuwdiji.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cokyvgsx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2okegubne.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zotzwubx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tzjupptz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2upzmbgvp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ickejdvg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2neubtbks.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lnxmbddm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hiidnhps.html


<!-- 参考信息 -->