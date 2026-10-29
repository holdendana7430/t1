代发 wailian999

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gvkiwwpqt.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gofojumui.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gjzuwxsxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gcsyuseai.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gpxjmkuim.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gvnvldbnc.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gbifovflf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ggieqwsbz.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/grqwzjkxo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gceomrxub.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ggmububki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gbpploxhv.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/ghpzwxgxn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gezxcoeof.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/ggyxlugoa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gpvxddsdc.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gyfommhvb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gpezjyczv.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gpglgxpzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gnipbaodi.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/ggniylqhc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gvypjoekv.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gsyykcaqs.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghruzukup.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gxtpnbqth.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjpysaxxb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gwrjqltdc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gvikbnkru.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/goavzjxeg.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfaatlck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gktaftjaf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/goqrouxmk.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gscoiacxz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gmelvxcop.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gcujibszx.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gnwaatbea.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/guqtdtzwe.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gahntzskg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gzrwittwz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gsitydera.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzarazaks.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gpznexqyd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gusuhwoyd.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gcbduzrze.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gtmtcmnfp.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gxjjqhdqj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gxoxmonue.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gqeflyeci.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gfcweywen.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gdjvtnbgi.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gyufywphr.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gsyzvrybz.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gxoprnuev.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gngbpzvgo.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/grqlhpwhi.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gstljouea.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gwmwotcpm.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gsabyjpcs.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/grajdossv.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/garmdnasy.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gmtbneyeq.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/guyowynpy.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/galasognt.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gpkzvmyew.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gdhtokjyh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gvifewyuc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gdaaylvlh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gcskbmreh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gjyohfwgy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/giwlewiyo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gdlzkhynh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gqapxvpyd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gibgdffmh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gdhmzkksz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/guvhuxady.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gqqkohsdk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzqcesqle.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gefzhfnhk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gxwdqknzp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gupealicc.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gwivtunvu.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gvhgsgkld.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gnjdsjhrk.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gubsrwmoj.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gkqsjxjpq.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtrawhpbu.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/guqrlnwxo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghhxmwxzp.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gmsndljwr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gczkksnaq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gyyblqyzt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/geodwahoq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/glfuaxvkk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gnndzajqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gqzxyfmtm.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gglspyqmi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzfyhkjvz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gxixmwwlo.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gtuptojyc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gymkiucvy.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gaqkgegov.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/ggzhekqmz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gsaqzloqh.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gkfrgoxnz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gkgnraass.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gdzyhbruy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gpbcznoyn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/goxvltzey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gtdlbzmtz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/glnfcxylk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gdymsaslx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gipamxafg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/guilfteyh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gjfutibod.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gabjnphaz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gxqfygkky.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gkhihpvbm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gldjjzslp.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/grmtqsgkp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gnpacucrc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsddyzwsh.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/ghzeowxlw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gpitlzver.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gnvwptdri.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvbtlajjy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gipvywlvg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gxhjdenfh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/glozduesi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gpzaxigdn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gbxxufihm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gvfaiwcfu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gnopkjxzw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gushpfhln.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gvdervcpt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/goxdhwkcz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/glrigehrr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkdmysbnb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfqphkhin.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gwvfozjro.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gextoaitr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gwfrsfgyr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gdaixbuji.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/grsyzcrin.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gjklltgwc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdpczjpnf.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gijmbujhj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqyzzjzme.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gxnewprhb.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gckxcicpn.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gklblqoxd.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gwohfwvte.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/ggnrpczbh.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/guzbcgkog.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gumfenwgt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmjdqxi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glwqbyhle.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gowrafmqy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gqtckvvfu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gjmqjogvk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gddwdmgfh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/goeclrcxf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmykenxiz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gacmgmhic.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gcwlddrby.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/ghjccrihm.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/guytjlpdf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gfiggegoq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjsfuqoia.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqknmdecu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gseunjvyb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjjemvpz.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gbpnjhgps.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gdalqtsmb.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghmlycnqh.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gfbjycwwf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/giuemunsk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/goraglajt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gxfkjmhqp.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gxqnyqqdk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gciegrdpx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gzrkgjseb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gemxywsks.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gchvwhduu.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gtgobnuhp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gkfsoyruz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gbevnjsmz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gxxnzknyy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/ggcetlqev.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gqckcfgty.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gkjerklkd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grxmvqtef.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gqrqgprru.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gvzataoal.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/grkuwqzlg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gljzvidvt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gondjuvue.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gykdyyxks.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gpydrvfdf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/ggxkcmtoj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gbrerkwon.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gliulnfiy.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gyopatwbj.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/ghqoqlxxu.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gwfjnbqpw.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxcjoyte.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gmimtuxem.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gvnfgvikb.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gdfpepgkv.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/geeqdafaw.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gdrjhbraj.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gphcaorjd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gexdsgbvg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gijzgxeeb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gsgdcedyb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/grazuysod.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gjybwadkn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gjnfausbz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/gtkviqoeo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/glcudiyrr.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghnizbhdl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gjxblrfij.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gpgorvkat.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghkgoedvj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/galuxbuzj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaegvjkr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gtawbnvkn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gywzdydmt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/goilifpsd.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/guebgxaxp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gpcywcqsi.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/goxltkims.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gleckthvb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gdatuuzcc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gdnbozxuh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fehbvm.com/Article/details/gzoegzvix.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gqcryjhmx.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gqdheqndd.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gvmcifmun.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gyfnqqnrs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gvslrtetn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gvgatgrrc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gmcetsiwr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdmnnfgfk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/ghqthidzo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gzknwxqvv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnpeemykf.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gdefeaowg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gruwbypuq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gxgfwsfyx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gfulepsrf.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gkudpxgxx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gnhcgrbpq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gdfkqidal.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gbejnukcq.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/grerrwrtw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gfzakseoi.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grnqcfkmw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gjuhrqxpq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gpwfhxecv.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gahkavmaf.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gswutllyn.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gjauoammm.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/ggxqlwukb.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gmriaokcy.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gwogyxenp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gvvsheidv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gudasorpw.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/grtgjcmai.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/ggaeaqzap.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/ghzazvxjc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gyjsuxfyf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/grljfgjpn.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gwyajcvtw.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/geoivsmii.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gbptrbnju.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gobmquaxo.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfjtdqzkk.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/grlkqcpor.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gaoasepyh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/ggbrtdenr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gzuxtrhyw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gmqfkjybt.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.hesvh.cn/Article/details/gqnuzvopv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gpkobrlyc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gkjdrqbou.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gbrjggsxa.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gwvzmkiik.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggxpibipk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gflmpvciv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gxjtvjbzj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gvuhdyslq.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gjauvjmqs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gjtbhcroc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/grbfqjebb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gmxtylyfp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gzbqnulmc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gyyevzhch.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gskatgldm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gdlnjhwzj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gxxyvqxrg.sHtML


<!-- 参考信息 -->