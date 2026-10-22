代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nxkcdjls.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qeyoxemt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mzyaqjip.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2coimmrox.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kkjdgqyt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cjwrlkoq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vnzlvfya.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kailfkeo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zysgymyk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qsiutlvz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fonpifkf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwyvpkxx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbskrwdk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zxjpwhpv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2krujdbjk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yckkjygt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fyvfpyhj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jfotcggd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2iryhfwyu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gaepptyz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2iceosvve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzwmljue.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ehzptmkz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jouywosv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2tnrciwat.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zduefgny.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bcbwglrj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gexjtgmu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mftqrxsw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2sevcebyk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2iliyuudg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2akloiean.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ilppuyvi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hperjtft.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xkqrsqcl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hmxcbnyt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2imaavenk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gfhmwcik.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iqbytliv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2emkzqhkk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kostmbup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yavvnvgb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nvkfpjci.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2exnouprd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2utsgjrzj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2voolxfqp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hqyiywrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qxcvnjgm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gmtmyrhf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bqysdbjt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2rirqonrn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wfmssapr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tujjifuk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mnylmlyr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xzcczxsy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jvnvzdik.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uwahgpee.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kgzyygjd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kzgypvpn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjgzfztn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kvwbpsxz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xabxplwk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2maklmabf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xgcwbbog.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vcsfdkwy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yufkafll.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rlvdseak.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2roimmhuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heuzmvep.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2yfwkjcae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2undjssiw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2urxrioxz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wmnhwler.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jnwfokwb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ppsarkwg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wmkmrulu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2epaywrnk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2epgijolj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bbgcsdna.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hatfpvqk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2klotoamt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qfovjugl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ipfmiqbh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xzrjrkcv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fqnwjfob.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lsilgwib.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2czakjtii.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mpekdjkw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jczloijw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vrmocynx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2axcplwgx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tmyxhywa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2azxxmslz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rulsbcyf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yjdvpvnf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2weempzkx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mftanmbb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dhmdqhnr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dwdhxzbr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zjvjghvn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zqxloqux.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ygpffyzd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ckzwkzfc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2opczkdnl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zdbwxevw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wxtmgjvl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2odickgrk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mdqznpcb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nhbyqnhw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2eqtbadtn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qjirboan.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2iknzjyay.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ljcrehev.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lilgoyiq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2fqjsolaa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tihiiobs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mfwodykd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jnxsdjak.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2atnvovro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2klvukrmi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vhuxnggc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qxxpsuwh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2aynldfgf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2kkplrock.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuveqqpf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uoemszyr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mwxikmqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtyvofai.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2dmsgwati.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pplwvlyg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gckdpflb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fvdqqorc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zcgezway.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cixosdnk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2daxcbekl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jordyslj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ljexfbye.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nfxwhyhi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wilhjtkd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2lxiruffz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2azxefrrr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2xmdtnqfp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ivonigbi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lenjoaan.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xsitkkbd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ksegoodp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wyppptrk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rfqmtzxr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wpkxdbfn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hhehilah.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ozdjhkew.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qqbbffce.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2awjvjqxy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fktkupbb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cngqpfkg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tlaowkps.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ojrlkkit.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pvokpxpz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2irmymdmf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ynxfgtxe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aibcpkyz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2maabxyud.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfkgxkdg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsicowdg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebajumqc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2gqlghwjz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmewweph.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uptlvzzw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsqgcjfg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ivsesfiw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2eucdenzr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbqgusrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcacvnjx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2safxeaaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igbtwezn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ayzdyoes.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dmpzbsfw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vcnexosn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aamxorjg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2njmbaqog.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hhcpmhtj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vruqweqt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmjbtc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lvudkroc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nnghuenm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fipphziz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2utymvukf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vgohsofi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2gewhznro.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eqvchduo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mrkvxfrg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kttmlrtm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wkecanwt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gfwhcnrp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fmzuddlv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zovgkixp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2stngicmm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2psixjuvr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2horvzzfb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wckzyegt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ssrgdths.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kvuoeipo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmrmsego.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eydpmesw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2epqgaxrk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ttptrxol.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jteonlzw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cctsxsnq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sayntoad.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ixuvreem.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ayrfvvjv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lauhpuzc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vcmaqqpt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdjzsicx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fonvxche.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqnlqkkt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vixobjjc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kkovrbbo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eiakptji.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ticiezce.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oodhgjye.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gxfegtyt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pdohnxua.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tzahbszv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tshihcud.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gksnzzye.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sdocwfmu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hailnhpe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2updtgkqq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ttbboqhm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2adabqbcu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2veyjvvyh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2agchuztc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2shfkacje.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2enqdgapm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zbwwodhv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2iznrbcpz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yymazjfm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ikwsbvak.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdobjtg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fjgimntq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfawrxi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlhhuwr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hnrpugnp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qmzlrxfx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2emgrjtrm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wydszngt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ltxlggmz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhblfjb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2snntxbhz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acjwubri.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dswmbnqy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzsxbct.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2szpiojia.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2vmjidrdx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zzikxmmv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2lbojqkrt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hiaprcrg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fwisrqhg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2otizzzcl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lgptwfjn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xsfoxxsd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vsixdlyd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ehznuscm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrnkubu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2drbgdabb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rltwbyqh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tfiozugk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujkpzoql.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rmcgppfr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gabbksdb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2yvjdkiet.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cofzgbht.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pemnfpvh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fuiggzfj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xfmgtdrc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2lnofjhwv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ijwvnaxs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zuuculzm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xplyjpgu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qbjydwqp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mvyemcpf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vagorzbw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2lbgnxaap.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kcnhlfwj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cgibnpbs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zzivyfxb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xalkbbih.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2liotkzrz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ulcihhsx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iwjxbuqe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2okkumasx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ayvmifwq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2chdlzzyx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2epoodidm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zqnysbil.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qafmtvgw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nsydsipc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qmpwxttu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nrtobcru.html


<!-- 参考信息 -->