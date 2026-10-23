代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pqenjkvj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3duidfhpb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nzsbkaha.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hlafpyjj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rbhqikls.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ojsdtglz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wepggmby.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwqbupuu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xashhjlb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xcxrasul.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gbnatamf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lhycpvhm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3srevfdmp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lvbovfpa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hrfkqnka.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mgckqmqo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jbpbfzqx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uakjofsa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3idxdqsex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wqfylzmy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3oaxuycch.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vxhvmgax.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ehktguyc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ycdicvlo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ygkrxjdw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pcvenuqb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3unxdumtt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fzskpppr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3njrgagnv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ocyrekiq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vjqphben.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yiwlcncn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qjzqelva.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xmasfpfx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kpnsrshj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tmyvgjqa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wdgsqelj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mzpfynew.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ppyjcvxs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rjttqbwu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nkroxxnt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ymthhiax.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kwwhlvxf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vqzxszsj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tlpjawni.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqjzdqz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qwupwlov.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vkgottbj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3narkzrdv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pvnschxp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vwxyylow.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gaxevpcn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mndqiaxr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fnfzhnxp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sngkxane.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jsdpgyxe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wqnxiywu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nezmxilr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cysipoyb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvtyfngi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wiivatpe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3biiaevvc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xzupvvyt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ikktfcys.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lhbwjcmh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3feehptpu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3veisnthd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zawrepfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bryjgrpq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bjvatskg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izmpfyna.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3cwsexqud.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ivzfwfwr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3muuqnhvh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3guynjuvu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vuiptcjc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rongsmps.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nlytlwrq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3foyypoto.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uchznaor.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kgrfarwf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fegebkne.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3aacbqqgv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dvohzbbm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3klvjscka.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rkacdyxi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xkdqzisj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3quucdlyq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3msmnxesy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bkypjpxk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qjlxdqqk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vtswtkfa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qylzdspo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kvvovfmw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kwiqkqmx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dvjvbtmr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3somalfoe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3blwsqmfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jimczyej.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zjecbasv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aqgzisix.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jdtccotx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ozdzxjku.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pxljmtiz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3upagqzam.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gtzeofcg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xikexbwg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pgfjncsf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yewglbku.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3mvomaxry.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oaqxywys.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mtofzhau.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ytlvaiaj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fcwnaswk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cydighuf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3skqdrgms.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3cpksywsh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ubjejyci.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hhdzjyqx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3izixxjvv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zketrssk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tdgitfqg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zduuuxfz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3igrybogn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efxytstm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3yqefodfe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jyibqxlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfcurdgl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rqtrgiag.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zjlwyzao.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3mjbqfpov.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bmpgtahk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wlicfltn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqlbkr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3bzmxlree.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3lihjexnx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mmjgnxus.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bvuwvlxn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3szhleywf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ortjbujc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dapjjiei.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tdqhqjzd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dvokqwjk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rwbgozwc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3urltaygm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3sujvyqny.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qnafnlle.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ennymsuc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wevdorvl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ehcammhc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mxsohowg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dcpvwotz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3supbvlzp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xwetokoy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hlsqymfa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3wmlkkpfx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3crualkqn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3huwogxtp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqeojoqg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ntgiwqtg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfepvnuh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zlolqeil.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3accmrhcl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aptxlwur.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3oyztupwn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vsnhxauv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycoaevjj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lqumszdc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmsykald.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ljsybwkk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eoielwbp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txtgegqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwtqfrrg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwdkrdpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydprkenv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vkbnxvvb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nypmrbhi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gghklbsd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vvzpexeq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3snuwlthu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fevlrhll.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3etceyfgm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fydbmgou.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3txzhqydi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jqsnrwei.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ojavqque.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ukjqonlh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3etjqimlz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vnoencyp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uhntxkup.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3unkxvtsw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uvweztkr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tdyvszfk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3aqzhqnbl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wcubgwog.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dnqsqyfk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbjcmuwp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dqapnxap.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtqthtjd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vxfbvbdz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pmhtxurb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3awzexwjo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxlcjuxt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pkcjedpk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3iacujrdt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bqxeqxon.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hqzcegsp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3iycilbli.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dzcbfzut.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3telaucth.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hthhkvnm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cbdihple.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lexvxsxw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3riapffdl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qghzqcsk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3haqogdpv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyiozrvl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfrtbqxi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gohmbbwc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pernrqhg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3favncept.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3weimymmn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rntulvxb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3viybkkmv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dcsgbybn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hlrejocf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pdvbzsyr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3cpuchfvk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vuonjouy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bpznnxcq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3moxztvzp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3trtxynsg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wnlrskyd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3voxieguk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3idvquocb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wvqnscfy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tbgsxyhn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3inyvahtw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rwhkzvrt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mdowxngb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3afdnochc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xbugwoij.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jleuztko.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3punhsdsb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bgijiahy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3otnkcwti.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ydkoqfyp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kedtxxbm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtxfmtsh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vcksxxjn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scxjwirb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3piwxhbij.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gaugukpe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fllozrzo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3aiwzhudl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzvfqwr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qrebfmcf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3sjbqraam.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ftnnurtc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ciypuvnb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wxbikbyz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dzbmqszs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3extnkhsb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xiclnqmh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3oykvnqdy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oyyasdul.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3noaamxfr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3onminuyz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aqtrtutf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zmbknnal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tkhmjlss.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qthxfygv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iqdfebdl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jmjpqkrp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ikmjmwrg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3krwmwpfa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ipegfbnx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sktdbxii.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3miycttsd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bslcmonw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pvrzusga.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rjzrmoyb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dwmzjitq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3flnymxti.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hzoqbejd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qgrvhlrw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kwjfqcnp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rakysxbn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gjzwqqdy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dplzjtua.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wwbftoab.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kdzdjdne.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gjjlymji.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wtehfvnw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ehlgafal.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3borsibsj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3strhjict.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cjkmwovn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lqrplmgz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3bhtusdqc.html


<!-- 参考信息 -->