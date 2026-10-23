代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vscwvxpm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wlecyoel.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3buxlypew.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gioxsmca.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ddaeequc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dkopcsiz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jxabhchy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ocupjqpn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjeqamzt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3etvbjocd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rbcoubck.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oivfoglq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3evmaqchd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qfsqjrzw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bfnohksa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ozihdohn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3aasvafgj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mnttztfh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vdylvtgj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qqxahonw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mkeukmhu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qqcnnama.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iwxvpwvp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kutreggj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qccquqix.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kgdftzsa.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3telabccc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zetlkivo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ykeaiswm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qcvubcvs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rdbmivmx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jsikhhfx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kesvggcq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hlphancb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3enjirpqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnqigwbg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rnebyhvj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ntcixsyc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uugiaypj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jxebnahm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehwvlkfg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3clgfkovl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pyrfkvsx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3usaowkbq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lfwkfgrb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ngkasqoq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ymjbaocr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zvpjvwbm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3buscqino.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hnjwdedh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wkpyrvch.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gnlauocd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bpqejyny.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3emjxxoxo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qksmpgdg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sudwvvvk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3klmjaoaq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kzusuayr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sqmumffp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ribstjym.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yenlmhyj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ftloqtuf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zkjjwtrh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3yxbpknek.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3indncbji.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xarnwmgr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ncftjjuo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ppmufceu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giuaqegx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oxfxutnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyyynmud.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3etdcatiq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qzidptfb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kvzswdyg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ehadgzzu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3iryzwtwl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3omgsoneg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3utyehcbq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3onavhokv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qdgajand.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qabcgygn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ytewwxiw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uhqrxxyy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3uocqilat.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mbejogkd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jnumaazm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nlihkdxe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3oaggfnrl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3unplrvdg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mqeigduz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3mfsobetu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jvfhmjpa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ihvldmhh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wojoqzjg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qwziiveq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ezvvygqh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ckxpasxd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yvhdgfyj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gkmsiegv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aejbbouo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jtownhci.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gjbyzpex.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lxtuqary.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jntanuzd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tvvubfuc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vwkcalvf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lmkvjbbs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ygmrvasj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3avrbxtwq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cjlaryuo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3plvjtdqu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wzhapgjf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fegfrxow.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ywwogvxc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rjadtxxv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3frxeniud.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jnrkqczg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kzccxslb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fvirkhwc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3gtogqctw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qnvkyqmh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qdslicxo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3dgpwacjz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ofhdpdtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmytoaxc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3momnwkqd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rqrbolqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygjvhqvf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xfcwzkyn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xhfmzbha.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qamiyzie.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3nfgbnqau.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mleoiqey.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3erudcqnb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vnjyvyyn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ftvdzmof.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ivzoxrnx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3liyzmorz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3sxldtgkz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3oodgwldp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3henonznc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3fysoogxo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3cbvwyvyx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3sbiujaso.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jkogypbv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hsbkvlof.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wfzchdfj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fueoafra.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pfoscnir.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qylmqacx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fefhperx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kvnzwyln.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afgtunuq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufymskzl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mzdmjknw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yjefkmml.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gmhcxcga.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtfbgocs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ihpaehkv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hiozmqwa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ihqgzepv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3igscxcci.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3twkykoct.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nlfcmtbl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xytpgmze.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryasqoyp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nqrcjisr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qrnfcvip.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bloikaqk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sndmgrta.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qtcsbtwq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3faciiflp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqklwnor.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rottqxty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuyectjf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3aygzitmu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gqyuphfz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qtevhbdi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mwauqfmk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ycybeory.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sobsexqg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ftuawrvo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3jzstyypg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ziyoelid.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dobxvnvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yatlfkwf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lmkiurdi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3elwoqlkg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3natbsxtd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wbympxfp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wveqdfhz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uoqngmzj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdedqvy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rxljujro.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xspqpnje.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vsfaymgj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jzuqgzwi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3haqatnnl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rqmqznzy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kuipafsc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gvfefxdt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rpcndxxh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3akegadgj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ytpitjxn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssovuopn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yaytlnhi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3haulsxvj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3elrolqog.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3wzxpnmam.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjhdclg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gnesslrm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xtuiocna.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3pejekywk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ejjwbdyy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rniowsqc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kyhigltq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3igikcgfd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svlkmdnr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3smbpftny.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mxyhjbax.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qejwtfyo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fkuplebz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xkibymut.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhdnfka.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nevwgfhn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bkfxwdws.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vgludfrs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3loiwhryw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjxwbz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3hqlkpggu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fuuftlyz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3higuhgfy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xornmcci.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jajmijge.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qmvhlaqr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3oqzgdhuk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3iktuyucb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gykwlcpq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3yguanere.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mwiuhyvp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3jzdgtxdh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3unzhmokd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wvxcwcam.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rtgalbqr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpsgwkz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nrirfkep.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwrhrom.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rkuihrsa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xzuuuxxm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubwpxpqj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbctpbu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrdupyhp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rbzpadcu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3irdrggek.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3stxbbjhr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbnhkqk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zhotpqzw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hsizxikd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3sghctbuc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zqveymae.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rywtfugc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rzmogrbp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zdjrqmre.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dkccrabl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zrzoekwy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rkzrxufz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ilzcclhq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wzwwmgxh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3awqhlhjz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3okdriecb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kfhvfnwy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3djoicpdr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uuuvsagr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rmrvsmcw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3amkpulnh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ejxrtkof.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3sythupvp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3izbjfcge.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xuznvahz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rnyarhne.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmkxurm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3dyypqkrh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3keftpxwc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jkuxdcgg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vmbpkyra.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jozyeuye.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wsrzrxpc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plydfdgg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwstpude.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yfjapzlu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lbxccfom.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bejpjqki.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3druxjloa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zkxznovv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mmmjwihb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kymlovsh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rmfndsck.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jsrfirli.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tijmsizz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fislsqzt.html


<!-- 参考信息 -->