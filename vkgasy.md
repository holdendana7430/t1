代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykuuumea.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wpipjagh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ikzxfyhc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ihtdmgud.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3prkphgct.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hvcwxofv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bkwefkne.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xetochuu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zkhzmeey.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vfndeeyh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zamfhido.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zzkosbdr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xevdwqph.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3msurponh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vmmznvzm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bnxqfgbo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nyglohuk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gqzujppd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ulifhcrp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3smojnuxy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mterjoyo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jvqsqucr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yustuxou.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bghrhfof.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3amkusjbl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3yartolct.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ldkeukcd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yxdeomdf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lwedckho.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtxkuhl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rzaoxpex.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fkyytwqc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eheeahoi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ayvudmmb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nmporvpe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3anpzzpvr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3biehlpbi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3optbspct.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jytqxinf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hljytyka.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wtndwnco.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fgoaudij.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vrgatxuq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fylourpl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3psitdxwb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3czukcypu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hpxxdnfe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qhezgkyi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nuozqyth.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pegpioqm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3iuggxglz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wzlwebtl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3oqujpzyb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wzudqnad.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qaxbkymt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vurbworq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snpxekem.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mexhhrqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amfskvhd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3shkjlajf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hjorvwsh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mggjgaaz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3piyeqnpn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vvmsbfui.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zbrlqklm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fsfkwukd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fppjirtf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jmjprrgg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3odoolzzh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3thyxwhpt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xrtvfzdq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3scojafcq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3izieqirk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pjvveldv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bodaoojg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3axsohghc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3egvwzhdu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhnjra.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fepxamiu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hsrwidvw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qlzhdris.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3whlswtbi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3suvlyerj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xkuroxzo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3evcdsanr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mmaonfgi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jxaiudkp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3joytrzer.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wrjmvtis.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3laqkaein.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ybopxicp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nivdccmf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fbdaquda.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vpwyujhf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mlqkovkc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3upqtrixl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ocgidxwb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ngbyltox.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ryfnfvqk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xvhrxbyi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qgfpnjeu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hjicdjjk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ojvfnrui.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3riwyawfc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3uxyfmdiv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qyotcxyk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jvcjzles.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3myxucmyv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3chuxvynp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3wiyswndi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3tdyuidlh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3iykhmbhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipuljnbv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ivkopduh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uuuacfdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxihduik.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3amvwmugf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jtumhjlj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3riywcabb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mzjrrldf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3otipluos.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mwejnlbb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3kjdxitin.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3rmuldaqx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vceuspbs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3nmjfiput.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aewaeray.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gqlctxco.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dslgkfib.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3aztfwlbh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dkqigzsp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ragntjjc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cfbqtnme.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rpklffmb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xxdadklq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ckdvznup.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbmohdwf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kjomtzjk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hpfviidb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuxyqtul.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mqfuudxf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dkdelonl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xmomoweq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gyewvopi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yvvotsta.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzbdwkpy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zkswghsr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nnqbbpoe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xyxhuscp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3phbudrru.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gssnzgxa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xubehdkq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjcmebif.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ysxzkezu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mtguihmx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xyuecqjz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vvabmcol.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3dxkksotj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3puwrzvih.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzvfyyna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcjnvwrp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xixqghwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwhocfnr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tsqvziex.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkjmqmm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pfyicucy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3srntxytk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mqimyhxm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3udnnymrj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uguqnjqg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3zlymakgj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qycgrilt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bzcgzcyk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qbrlatfg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yptrnhjx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qbkoulfp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bqnxctqi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3exbidqxn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3plxthpud.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vfuvjdsk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fsbtxzcq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3reyudrrl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zjkbndmo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hisqbkwx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oulzfidd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nngjjsjr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ymkbroaa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ykylxnev.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3omoztscz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3erwufxfu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gbgfiust.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xcgvycyt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ddvxonlt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3quormjyn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bwfhtngj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zdwcekrt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3inhqredf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nkfomnta.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hrdzfpqo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3nivjvnsd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gcmbgowq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnjbkyzb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tzeahdtm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dmylauhs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gjvqrdpm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aygdrplw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3suaxneqi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xtptvzmu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fsiexqlg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bhlyfjow.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3agorfgzd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mhgalyqn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lupcrhvs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bzuqcfou.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xmkrhzvt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3phkudedf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yrjkzeal.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3zqpkcwnl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3lmomrelb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vkfxagbq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rozoduue.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xteqiygq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gwglndjv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3snbsqqev.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nqnnteeg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3yffrodbi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zrxfsvet.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3makztnnv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qgvldxfb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dpyesdya.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zfvijwmh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gexbklds.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgjoddj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3avckpyli.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rjduokmx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qpcnmjnd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3agvegqmj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgzthdj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfaikay.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irhhavis.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wslpbimg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3sakvszeb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3upwjkzsl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3izxeoirj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3omgsvign.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fxbihxqw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3egkaaume.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gpcpkanu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ogpcxhkx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzrrwjwa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ebgqttza.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3uzjljtis.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gpaetkmj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nmlegszc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3laajefmg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zactgbjj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mjuggehv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3psgnvuxj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ogobgexs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ufrvbdxm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wjuzrwxb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3agiwsyzo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3vbtfazjs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3agkvhmud.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lofvqxjm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3znhjovmc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3umnudfyu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgppqxa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3jbxnfwud.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fcnhodsi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zzbornmv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hsohevbs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nemyodru.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qksfveda.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xxtylubv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mumeqush.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qtswrpjs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nygvrlrx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pdrkshkq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qjfvnqpd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3byiduwhd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3imyvpbco.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zmgfybsj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3guoosbib.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zkrvyjvn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3nbzfvttc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3olfjlddx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vksrdyxx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wbetaslc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ttyprdcb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bhojldbx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kctjfzbc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tvqiafgz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dvofqsrb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3izsgfkdl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fevichsk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xwavhhsu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ggsmdnbf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3nupiavfs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ykbxoess.html


<!-- 参考信息 -->