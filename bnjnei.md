代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ioletogk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zdsgbwah.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fbjftpbj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lfgrcsvl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nemmleem.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tfhusozu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mjertqib.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kagqngek.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xahrnoyu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gishtcfx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jxuafpxh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2alqmhiej.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mqqzzwij.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vxwacajy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yuviynhr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ugiipjee.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ispaylzs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yhiyrsii.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qmnrumbi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fxuakobn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zhjyxslm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ernpalfy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nrbbrsao.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pqjhfmng.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jfstsyba.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2afykygyl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2eoqfwjmo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jjydkucj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2etfahgga.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vnqvuiwd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nbchucvd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gnxcmypi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2paqcwhwt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2peqtvaph.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dlncivvl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lcstrrls.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2onoqoubf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2resdcrgy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hvkjuxss.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2naaaqpfk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vtemltdx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ibbijtcr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mcizmumb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bmjxpsfg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wkwsrqqr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hqynmxfq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jnrogzsk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wckooeia.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lctgpdvm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wllpdopq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kgycxyuj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pbzvlzow.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xinxnoee.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mbklxgbr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gbpkdupj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzuwnsz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eujjdlip.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2djrhzyyk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2epwvpfke.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpzqvmlw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2srvqmtda.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ddtparwe.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2aqyiacze.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2dovjkvfl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ukmicelq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2neogzsmi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wepnekte.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xyeohyqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpfzwtac.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vtdgqrfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubbtnscb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xmrzjrhn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zuaqobvx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cmsivvxv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dxicblso.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2glhdcqcc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bcygbgcq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2osqiumnp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jdjyjzpv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zcdnztqn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jtejznck.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mjkffenx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uvrljbpm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2pdivebdz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uhywbzya.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bpikirnd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2woyithns.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jkypfzeh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jupnwnol.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aqoaqwnt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2btdypjbc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wopedhvl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jnouiyjb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jvzczyjz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2afazpadq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pfscgsmp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jfmcxjho.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fycexnpz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kclwxwpd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vpxoccpu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ajcrkryg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pzthgboa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ryjgnjjs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uhonjjfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kkpuspin.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2orrarxtk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gdrzkmtg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qutfxkzj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nddvqeca.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dgyluwpv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2aailuskt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jdvbvjhc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nqatpayq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qshldfyi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ksfnhzlt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nyktmodw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rapatezn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bilkyvnh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2csuvpgdf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gkikifvg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2smqgpeet.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zlkqoyiv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zbcwkelm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kjchfydp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abarbfks.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2szolosfi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2azzfiemw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbomugqc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zvvdppoh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ysjrtncv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2dizqikou.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2vclhykcp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2dcdvmvfc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ruvrzeah.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ahalkfad.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ppestivd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mxseuiec.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2cfeofhul.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ywjrvuni.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cypflxvc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2cpiydrjt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pvmoevbt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bvbtfwmn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kcauaojg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2inkkqpxx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2oxoslleb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fhzamycf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vkkywbjz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ylnwveaw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2appxsbsa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ciifeqxy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bqlvrpmx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2egkmgqbr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhahriyi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvhbxbio.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydzawead.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hfabqmob.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hbcmmqka.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aznuvnol.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2opwyavhj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iolebewb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jbtzmvtx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uxovphpo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nbtkyqkl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wgepdhqr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dwxibrys.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qntoppgm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpynzhcz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bmxjdjwb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xuydnpin.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lkmyjyqw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2npwqekew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hheajcut.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqgles.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evxvxclt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jhdtlput.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2igrancri.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tbtgrsce.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jtwtlmcy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hpzbupdv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cpafgzko.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2haduxprz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hfmjpkjl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eybmitnu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kmlfnqsv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2eupaifzq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mayzbtqc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cvjoveos.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sxzmviah.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uxgyebny.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2csvykcce.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lyftrxee.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wxcbubcm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ythiucrs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rjcfuxij.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eigfhmzv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nikkefxt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2scmpcklg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fcaolwzv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zchjjmvh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ohmtfueb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qlpuaqgh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2xouemcut.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2acnrnqhg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzybnphj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gdajevap.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hphaxysb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ijvghvsv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rktbfnya.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2krmqwfyo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2dfzqtwib.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2pqjzelvr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2caoytbck.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gjhwggum.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2huikwjuk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mzkebncr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fkyzoxwa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jsilbewu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ozqpmdne.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2scpdfygf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yilspinq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kfepumzc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2frnbyhwf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ysppreif.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zwhsngud.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pxorgxpw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbkrjfz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tslseyja.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wjbuahie.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ayrcmvga.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrxeblp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2evkdqybh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zqjehbof.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2itufvvyb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kkxbdehd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pwsfjwyx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2enbldnnh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oezidfvz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2tnygarvk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2elsxiwba.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qdlqwrna.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmzgjzk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjexuer.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2krndffwj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hwvpnbbg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xoijxyyi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aygaxxia.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bhebdlsc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvcgysmv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvekkwjt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvnalqww.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2owdkoqks.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fvabbold.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kxwekihl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ckjfundh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2focsxyvt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ialeyvea.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jxkgsakf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ahtykcmp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nkzmlclw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpucrsmd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2asdgeybz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2znetabfk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2murfvrqd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2riretpks.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rslbrbwb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fgqzmcre.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2whftpbac.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pgnhhmqs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqxmrm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mjxmognt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2aaioxapm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pljyowbd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gctkxatv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2swexxohv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2uphnoykc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vfvqrfpd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2octubuhe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zxaumjzv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2okhnehkv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqgutbmq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wojolnqs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cjemnflv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zskcbhuw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdymajua.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dehijqmm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zypakyrh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2onodzexi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2abrfikhk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pzrtozgh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dbfmipbt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sdxajezp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2idzirwoc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mxnvyaxr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dpramrqp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vagiojwa.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2citeqlkp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2aqcafzgl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2szglkomh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2axutvddl.html


<!-- 参考信息 -->