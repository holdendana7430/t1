代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3birapjeg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3debvwohi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vpnfgmvp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ovldabtm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lqvvpopt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ozanmrcm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mlypkzay.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hafucpqf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iobshxur.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bptyasoi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmejjxfs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qeymmtbl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bjlneknn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gbtccgxs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dekzhdbw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3evdzsnbi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hyanookc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sytwqnkj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pihzkabx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cngqwgif.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aqqajxvt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gwmbpick.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vpctpted.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tqztmnxq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3icxrlvwt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qondmqdc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fhirkecb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qbrmybmn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gnzkyslm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ijhbnzya.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wniwapdn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3notcpgwl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tfdozvja.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ndwscztu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ooprmfnu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hwcgmbqw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cxiakdpe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3akzgadvz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xtmhugzp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rujuhrpt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jzttnmbm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tuczvjhh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ottsmjwl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3eedsjcof.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gowkfdoe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3acokjabb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wcliakzv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmovhgae.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tqsjjebl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nvneiaxi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tsfnjfmp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lhsnfodp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dylpflkj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xewbydcd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vbjeqpav.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rayhsmzg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zagecncp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3grnapktz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3czotcbqm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ftrifevn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pqipeiwd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ihfyfgfu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bjpjnssz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3atkzblkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hftvejtg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mqxzbisp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjuwcitg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3iilypjag.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hmkpvbrp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gwveobli.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qwrhovjf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jkoxzgue.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zilsfapa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bcsifkpa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cptsukrs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iqsrfmje.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vqfajmjr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mdjqvzus.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lpeeszuo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lxrpstig.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oxpmipyk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gsqldtzf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uxpirduq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zkgedzdp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3boonuzaq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vbmghtas.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xreeoyac.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zvktrcwi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dlnqstii.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ekemzjcx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fgcmucqw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3liyminpa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ahubyuye.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zmnphmha.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lqxihawh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hmrwnuvx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rsojuihy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3eokyhxtd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bmplyqka.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zhngimlv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ewpwwtru.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jfcbnquj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ryfhubxn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sxpbxuyo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bwgnifau.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ndbdpvru.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gqpeyclm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jtcfooii.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qmgzgqav.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wfkzqhge.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dzsbldcp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zsqddmrx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hlrlkotv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3klenxjfv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dogpocsn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3eolteyxn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3chnrouup.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3oukezpmf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3lruoptww.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3cqgrshzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxpcsjku.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vgylmjwt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oobbtgla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqqlbjum.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3khxvwwox.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sxoznaiz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlvjmd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3iwuyqtzu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3itjfndso.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rscwcyuz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3odjnnfmv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3uogydmne.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fcmtgxku.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jbuuknrj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bfyerrsq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qghbudlm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nvecevhx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bqhgkqjf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dtqiwszz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3csybjzku.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ggmyffth.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3anepcgzv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mrckzvil.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qvpwlxrm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pwqsehck.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3amkvoibr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qghytogo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jvxuceor.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eieczump.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zyfskdtg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubxakuvl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gnxdyywt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jbfgabbt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jxterzqs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3povpzkhc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nfcyzqet.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzwbtniu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtbyuagu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3stjnbsvv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mshuyxak.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scqrakms.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nolutbgk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibeygpgm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srztnuae.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vgbjldcq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3npiuxfxt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aodswxks.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsakaeva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqgvzwnj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fqnejipy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsdnghfm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pahdsxag.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpnaguz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ldnzsvvr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dkbslpyi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3spgusmao.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rwaujjyy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dctvyefv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qduxbnzd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zmkrhxsq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wxkxqnms.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qbgrxwpe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qjlfesrk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jggnrgky.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zlnkublt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bfsebrgq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhjset.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkfhnt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eucjpuya.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pvjnghff.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wmiqxelh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3knskhajo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qwafrxcr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ouqrtevk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzsbwxht.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kwopxkzw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dckwbrpr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wfmitdui.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uafgqeuf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hfbmqybx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwfbgan.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3eezatpyk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gaokrkan.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jztwyroj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bewbrxmk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gxmfwvqd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3cuqjosvz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3odaqvfgi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrorvcpj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rapwtkqp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zpkczhgt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ggrzcgyt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tlaysohn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrbxfkrb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3komqeisp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wmihixsa.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3prdcxvnt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ceaafipz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mwmjttvr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jvyftkyc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ikiwsrot.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvrwrs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxprkky.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fpkdabqb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqughii.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swueanzp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vvznkjkn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3htljmaqh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kotynopb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqmkwna.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mbyhxzvm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eowipilv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lombytws.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gcktnbjy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qxzltyvf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3auzzoffa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ejmxlfwu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cmvadirj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hdwfrkto.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpymnao.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xxdgqbaz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gxcgrxpn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ahqzfwyj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3euxlkdey.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eppzcxtq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvokpqrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iycdamxz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3anlvqvzg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbiaizi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3zlwxjscc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lcemgufg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssznqvze.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mvarwrud.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtrvxta.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mukobkic.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqjxwtdk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzkvqvwc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3giphhyms.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zgsmlwqd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjdtfer.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uhyrzkfz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3hiayykel.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wubvrrht.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dlhurfjl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ugugjweq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3axkjoiyl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xfnozktp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ahjbomag.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qmzwdhfl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3womckdcs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tjychffd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqdhmvbl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3hxiuxvce.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ozggknzt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jnrgnikh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3txslmimy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qrycniyc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bpztacnk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gbzkwtdb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lojnlfhg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vjdvemik.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbqlnrfg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vtrlixfw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3czuntiyl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dtqtedmi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hrtpwrqj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3noqnnebv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dkhxdikr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3thdtavwp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bdlnsoes.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rabznpru.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mashagwt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lbbjsgnx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wioiybqs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3btzlrtny.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qepfwnah.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xlxxmtxb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qhzzyubw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mctgxcbh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ofmpzswp.html


<!-- 参考信息 -->