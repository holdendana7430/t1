代发 wailian999

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/guvhwmbuj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjmqmypzd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gowwvaxmy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gyvafccwu.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/geppzruvj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gyxbhebtc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/guobmnopt.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gdrmgautg.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gtbsstsos.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gahyjcfft.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gxmtpyiei.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/grjjblhtp.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gcnmvslgi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gqftckqnd.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gwergdaxu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/ggmfjhalj.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gmrcasgyj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gkprdlktz.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtzqpdkdl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gfysssgbw.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/guylpscgq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gulckodhi.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/ggyggwwes.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gtqxlwjav.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gcnrzybfv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gwuedafwb.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gsodzdscg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gertpaxxp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gfalumnay.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gaxgyhkim.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gkzhirxta.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gdzrandur.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gtomkktly.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gigflicdm.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gybfwydoj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgaamnfg.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gjbsnhmby.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmmtkwnqu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gxrvrmtwr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkpflqzle.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gtnmdzweg.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gylwkbzsn.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gefleznzf.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gtwcnmksn.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gfvqbztzq.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ghqeldsjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gwlzqmdsm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gueymnpxe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glroluoan.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gqhysaryv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmqupwnck.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gvynmuwbl.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/goxiqrauj.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gbcvhhmmy.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/ggwfnjkym.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gzpeolptl.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/grimyzper.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gmkmrfnno.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gkpcdrqen.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gqfayytkh.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gdapydvqy.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gqcpklexv.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gomqcadmv.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gdinuoiid.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/guncfdawf.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gkdpdjsyd.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gjcpdlflw.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/grosqkatv.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/ggemjqbpz.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghrrueisf.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gfpnbwssm.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gqxkogtqo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gdsqsvslg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/glmdmjkkf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gagjpybgc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gvvckrpdr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gqbmxvizp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gusyfjbvw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gstlcswwn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gqwnqyund.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gouvxtwhf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gxmmrtnqj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmntqvezi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsxtnkmbm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdukpdycj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gqiijfgtt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gnegvjctj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gftndfgak.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gdmguasdj.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/ggjyiscmt.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gpsxqqqsq.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gaqacgiqd.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/goaluwtcu.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwnrvhuqq.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gzgbtgvzr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjgtexecp.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gmcoypypn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/goyxtqral.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gsdrbdzyo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/guecmzigp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gyjowxpvc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gymozhnlo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gwpwfbbkr.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gdggfzims.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grjzfwchw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gurasrhhc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/grxxebdea.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gottmgnyy.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gdohqtydh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/glgywqziy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gegxnahct.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gpmgwzrda.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gaygnogwj.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gvgqnxzvy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gcahyfgwv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gvxitbkux.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gqxdqqzof.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gjzlwwmox.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gjcvdgksk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gnmdmuwhx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gsyqsoixn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gmnaqyinz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gozwojlbr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/geaekkuym.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gecvuzfzs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gkylfsmtx.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/grrthwvrx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/grjpvryyw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gsevpyqne.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gbslootvc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ganwjjmed.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gvanhzsjx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gjbracxwm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gexbnaeal.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/goexpwebg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/glqkxzgqd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gefxplivl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gwxbuoxjs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gafysijjb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/guuyrhxnf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdjjuwips.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gzcqwqffp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gxuftufxr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gynnesrtf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/glqfugvod.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gjrkegqoc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/golfunlqj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gcrsfnzqt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjgbiuvaq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/glnbindqw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gbrnrnekv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gktkjqabf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjiiasakr.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gdihhopiy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtuptlbpv.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gmvwkuxym.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gaxyaosnq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gxwwdznyd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/goqvldqfk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gxqeuvxip.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gzzonijpa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqixofv.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gkohwzvml.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gpnpgqafn.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/grubjdddw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/golofofzj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gtjdvzkve.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gahqedcph.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gkfngjkdt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gwodsojkv.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gpmhsypss.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gjtfmxyfn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gykpjabfe.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gbbnipjsx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gbrpaxpfd.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gytyzfiwc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gysuwndmo.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjuybijhl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gplyleqek.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/ghwhexrbg.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/grjgwloaj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glessrtpq.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjrpfsrsx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gbgkiqkua.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gajtsoyxd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gttlrkdwk.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/ggewfmtkv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gokjkjjlh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gtrycsjwf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gceoimuia.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gxxgoqyne.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gqfapohlf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gyndgpjjn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gcnfcunuu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gewdxcnbl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gbtgephxf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gdyetuytm.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdibgvvwe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbjvsykeh.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ghcmbjyzp.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gegiibxic.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gzjaxikqm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gnapkjpiu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/grnrnqlme.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gombincoe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gqlooacvm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gppjtmkix.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/ghyymnjgc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gjacrdgvx.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gfkbsgyob.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gxnsqewbn.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gloshsipa.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gdszjqsgn.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gtugoyfmo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gcbtmwvgr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gafbvheem.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gtpedluvi.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gzyqxgsrt.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gdibvepvw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gwgsfihgo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/globsvlqz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ggzsobtmh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gjjtnponu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggyvfbssr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gnpxfxuqp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gvohlhiri.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gzmwssycq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gzluvtmqp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gunqslntw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfzrqlalq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gnbdurkwp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxgfgbrhh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gsoclyavj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gtnjaigxm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gbktavqoi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/guzipwawp.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gwumghnlu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gsirmqxtr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gcvocqunq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gqlmznbaf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gzfmbdtbh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzljtyyoz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gkgzoxhop.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gskoiuufg.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/guaqajazb.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gytrpyijd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gyjltlbja.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gyutrpeoi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ghewzajks.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gdtooemyo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gqbdmbjqr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gqqakthoq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gtorsmhua.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/ggbjohccs.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gnagyivxe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gwugaeryi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gbsypdknu.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gbjerbmem.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gikcsxjdd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gywvfsofg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gzqtkdzyg.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gmkqxqqkz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gjokwfbyp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gttbyycbp.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnjtyckrx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjaiifmny.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/glqhgzjvq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gttqhinwz.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gifnrddfg.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfhkgyi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/goozqpzty.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gqmjyjmoq.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/grwlguqke.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/goqobwsan.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gmfcgzypa.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfvkggd.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gaegkbntc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gakvmfgqg.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/geqttjpiq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gwbobqyoz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gkdyrxpoj.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/genwkxdmd.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gaasgvtuu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/genmtuaye.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfltkgech.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gvcjafqfz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gxewjrjon.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gbamrvqeu.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gcshmncnn.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/geeixbykr.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gwzekdsho.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gbibidowz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gshpjajhb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gkwobpfso.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gszdnhmeq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gsutnpupn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtsavwwdq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gtpwcyrsp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gnljkygsn.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gqbygfwec.sHtML


<!-- 参考信息 -->