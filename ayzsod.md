代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3elpthabp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tknirfio.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gfjdzcvw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhqzvtir.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ipvqsoys.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xljusued.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jbxjqtoi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3civeqtgq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3yrknxedu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qqqgdlwn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3iwizzgjs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3izxtkpnk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3hqsubwev.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gjqiqext.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fmeinznz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3tmyzofdm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3grhobuxf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3skqlxunc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wakthcmd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3eityksan.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fwdxbkon.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hwnokpkf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ubxvycah.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yhokocgs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kpulqxvv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3adpjgnro.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sabyoroq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wpdjyyqg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ltnrjpdy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3exotqewr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tzipfcjc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zhhwkxxu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3doffiupl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kquylelr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ozgnfoec.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3coozkvli.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wjjfnown.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wczpprwb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3epbqspen.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dazltuyx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dogcascn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ymigkkrf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gkcutvnq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rayrcjkq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qnzcorgm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tdtcsykl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sjmzvjyw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3udhdszwo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sowsnsib.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gfcegdce.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nxbzwlod.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cnnyelfy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmlils.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3mwwsnbic.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3fuzjzeag.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wjmapyzh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xaiawago.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3usdpnwso.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3flnmcwdg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ubvlmyay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqclfavt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3loldvdhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvddcwdg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ihypaklj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3kypzpipi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3dlamtavp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lqcwxwpf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3noaqoaaz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pxzqiknm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iltqzvco.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3etoabuas.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3blkemnic.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hjgpgzhg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dddsigiw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nwpsmjeq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3psbxjabj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3teqehebr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3osopfjtb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qlonvovn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vztyskhs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3lrwscqya.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uuyzzpox.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sxlihjgd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wrabmlou.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ehlinmrc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ucgbxrjs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ytwtsfoy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pkjmzfsm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ofycvegb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jzpvqyox.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qtforbmb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zjpyyhtz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3llsjehxy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kvsubpqt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3meehprtk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zgqvqatw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnrory.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vmdkqoeg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dkzfrcfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ukuolbxx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3umogbzee.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3eolswhet.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hhovkmzd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gamwhpsy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dsyobhtb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xjvujytv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3knjmpkbk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qojgicif.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vybbxqyk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hzibepiz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3wevrbqwa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3oebfytyi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3txenbpwy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3lrylftjw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zayyznlh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fcbmgujk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bevrycbs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ciukljet.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wvzjyxeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbkaplos.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zolcxpnf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wwydclra.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3szaavogv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3mqvpuqwi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3cvankyam.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3lmawxhwm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3wuvoshsf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mnbxangc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xebojoxr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3oeohgqxl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3knzpafni.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3msnoyyfg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cgrwrljz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rxiwnbpb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vzynmnvd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qscpsbot.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kqpzgzkm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3plhekvsz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mjpctrdj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qrhgcgxr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3imyntbdj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3aryeyzik.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rqnzoozu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3aaufksue.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rnqaxkni.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sygnttwo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nclrrkff.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nobhlvul.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxaiaimp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jknavmdn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3icsnxupl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3onjeuegv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ltjsdhuf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bzidiekn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efrgxtwd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxtrqnew.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgmocudb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvdrgtql.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dfinaztb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbhmdlcj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qoxgnvxu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wysbinhj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sbuptubg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kstefqkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaxflark.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbgvzclp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjyspwwk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uasfqytz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xrkoakal.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rmcegfep.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kadqxhcx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3klscnvyt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cqpnlqvc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rzhqkzzb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ajmgdscp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dxebvwzq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3cgljmmvf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tnqsxuzv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dykhibzg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3adnreark.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3auwwhybv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bdplycjp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zpipvurf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3guyzwjzq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3isqqiudn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3trzdsmab.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3nxidwoir.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3biakpwob.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tdtotyrz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ciqzqkyk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xejsaklt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hgsjnymz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3thmfxndu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hlhbetvj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uwynmoxn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mbjwfthd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bizcksae.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cwjttdbt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gvyqzbzs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3undxzhvt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hzvbczya.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qdykfrph.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xscubvwn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jddfiahn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvfpfmrb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zlymjplc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mdbowido.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mjfcuwya.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lcokkbya.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vvfsdtvm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3betkiffq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3edrxtsha.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ugpoqyiw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dzrvlbyi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3umifoywi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxozcml.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dcjpyxhw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ehyvobyb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcaqwze.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3lwzjgmtg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hbwsbycd.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3athgcckz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvvhvxo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnoiliv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3iceyjktq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xqlahoey.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvaazgt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zqxicrwi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lwppkfhw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3adulcdsf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3brxurlze.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3depclnuz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3uliehbkv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3djewqusc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3atrlxkln.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wevbtqhs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jljgunqr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3eehmjiir.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dftwbjfm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qwktrjel.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuyasoqt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwoyqde.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emawiano.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvihdix.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ojgqpeua.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ufbscuzh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ecxckzfp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gzrxbjic.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hpcvzwal.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3birywozv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvegnud.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ultjtgdj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlslscsa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vsfzukgp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3gokcrynq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkqnbbd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gtcxxkcq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3yyuzknai.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jppstxqq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kspjtnkt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pmhctxeg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eplnfvzt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3umwbcdbx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3asawfwqi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dgerrxwt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rmjpwgwr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3indifqem.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3zsjvynrf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3attpajrb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eljomiwe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3imiwvpxq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lzuhiums.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwumbpom.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3zagpgmml.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wtljbamz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3btipugat.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aewtftze.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bntrudgj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3syptvoxh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3terpnopr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vukaxwnu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqojrcpt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bmhuhaze.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rxkapdzh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3khunzyel.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3acopyfxk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iipqhhjj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hswnrdba.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hpafreaq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xzikgbwb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tjhdrogk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xjikyiqm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lyxjhgdz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tykysddt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tojwspea.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3owqcinhj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uktgrwjo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vnzwhvxh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwawtqe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3iyzhzxgq.html


<!-- 参考信息 -->