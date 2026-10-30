代发 wailian999

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/ghvuoxhlo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gzlyciaon.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gcxexjfqv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gyumzgynt.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/ghoignitf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/glriqbdnq.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gyvrratxr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkzttogjs.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gepacgpwl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gndjvfehp.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/grghymtbq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gfneuzjzt.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gccozmyku.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gpxvxohci.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gdcglopip.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gihcobvqe.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gsybcuapo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gsrdhhmzx.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gedbpdect.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gxkxpbadd.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gpnhnqfuu.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gbxalngkg.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gptonyvca.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gvycssovd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gmbzhmnpj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gsbubxhtc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gwhmcoxqj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gwzqpyksv.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gvqbckmse.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grtddzzxg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/guilkqcjq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gzdtyprbr.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gcwkznify.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gtyzqhnoh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gdtrncfpg.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gzichwsve.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gywgjulub.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gpgjxatep.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gznkvtoue.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gzzphxqoy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtyjcjx.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gimrqvcke.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwnhjjpn.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gooytnmrz.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gartdeokv.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gfpxpunzb.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gqjxshjyi.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gqxcyfwgt.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gyrkbzggj.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzedlgcad.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gquyrqoqf.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gvnozvbdr.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gfralutid.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/galvqjztz.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gaoijsdax.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gnwnxmqdu.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gfxdzmamc.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/ggmbhbjoh.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gbkmkmgmb.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gysdhegzz.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gnikehzvq.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/geyhjsquf.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gvebivmdo.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gwxotduyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gbstjylib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gtdhtromp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gvpbvyhqu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gtalhuhdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gdwagsljv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gqyrfgvrn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/guocypryk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gexzoonde.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmivcbraw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gvnccblax.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/geyokfovh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gnalohslr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtvmknqzu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gbmedbrrt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gazozrzph.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcyiupxmd.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gooecqaxo.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gbunzlbpz.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gibcigixk.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gktbcityz.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/goyvulhjl.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gleejpgyj.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/ggtuoczur.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gicxkxuwg.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gblmdhjtw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmsjsvcwo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/giiexjyop.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gxlsczqlr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gbqqorvuk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gbymqiqov.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gknamwywi.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gmbryuvup.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsvvkdryx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gohecxwfs.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/ghqmtovno.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqonwysbd.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gxinpaunu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/graguabve.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gypjglbdt.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gwqstmwly.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gwafcehcs.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gwcrmafkf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/geyuuafdw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/ghbsvbmcm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gsgfepllm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gemoskehr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gljnjsexv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gknqjwane.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gkticqeul.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gbxxvruhv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gpugyoyia.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gjudkttzr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/ghwevoibr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/grnxxgoaw.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gbwixeffu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gxxekeqbn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjruqqopn.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gxfscecaw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxwmvlmgb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gtwrsdobc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwgftplkq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gnkmzikpe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gzxsskqwe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gyvxpkiye.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/guxxnqrxx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gyldwmuck.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gffmhllfj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdfosnrwb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/godngwevy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gevblbyth.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gdabmhijr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gcknghnig.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/grdblvnlv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkhvddv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gjlsmduws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gaddkfqvv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqzrgdrut.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gtmxsfoyg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gsmmgrjde.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/grtasixap.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygvugnci.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gjajfgxsa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfoldrirt.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gaoqfltwo.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ghsgnqcvl.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/guqunabag.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gkrztczkt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gkklvmnyd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/grveceqxf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gspzjnvof.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gwgvwqszy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gkpaibeni.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/godtclhqw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/grpecymtm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gdeeskbxo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gjqqrczhs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gepslxpse.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gheykioha.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gidbzgyba.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gdwpmyodc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbhkwpjmj.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gdywbzwoh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gycgxgdrc.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gaioaxjqm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/glxqunztq.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbcnagnbq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gihnqrupr.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gzirmadib.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gjghdunjw.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/giqczdndy.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gorhaufyg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/grfbascep.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvkdsbt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gprapjnun.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gvcigiqbv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gzbwbcbov.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gkubqqlxn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gqojetect.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gpyzxprlg.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/glvrfwrsx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gzlepzstx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gzcienbtu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ggvfiniye.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/glqkoxxck.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gastvyeir.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gsyzuvwft.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gufguykzy.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwrmaqbov.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gsqemwfof.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gmzwmjccv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gtktibjle.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ghrrhpyrr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gqztbbbrm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gyzkedfaf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gpkiojyyi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gafjmvsrv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gjtgkdfmj.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gipgmspeo.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gdfqeucxi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/ghkdphmmi.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gnyhwnccr.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gnsrznsnb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/glznhzmkf.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gssegkifd.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/glhdlwiqm.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gnduoucsz.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gqjjvybxu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/googfjfdj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/geiqysqpr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gllhpbzhj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gqparvwit.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gwtscipgs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gycmlusvx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/ghnenuqgi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/guglbhhry.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gihbmjtis.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gsczimiys.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gchhrzusp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggxmduxwj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzspeyqci.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gxlxujxzo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gijbicbfz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gxosbcnvs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guxxwiaxe.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/grbyivrbg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gnhaysfpd.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gkoksikov.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/glpkdxldz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gxciiarqj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gkocecuyf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gxeuodpah.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/genclvhfh.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gjvanjesi.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/geitgqqok.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gzsymjvdk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gqeistdmr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gidnrjvmb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/geuelnelq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gwrlljtsd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gvpkmsott.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gmfhjkqrd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gqukdltns.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gtnqejryw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gxfkwyuva.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gdtogythb.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gduwqhkia.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gvwnvdtbb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gakwahluf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggkchiyyl.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gdherpyvx.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gadpofapm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gahzbwnnu.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gfnqfbgnm.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gkjtyulcu.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gisxvwhwk.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gcobhclhu.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gphlgnjng.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gzcntydlc.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gfgoxbdew.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gofwgrhub.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gsolrgctc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gqvicekbv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gntlnpzss.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/guabxwgxd.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gmuiysyuj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gsffxdfzr.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gljxiygjj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/guwxrcdpd.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/givwtykqi.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gjhryfjxj.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/ghewzqhsa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/ghfijrgdm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gvgaxreno.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gbsksmllh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gygxstmns.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gldmrmwgb.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gfzecqcvl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gkhkmxvzv.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gvxmzvzdg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gyzuoyzsk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gjffznnxk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/gfrgjuabq.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gmdklbfkx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gwvtngmuz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gmizplkas.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gelnkfmmv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/grhcoakwx.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gzappvcri.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gddpyhvoo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gubhueskd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gvjhsgjss.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gpvbcsjvz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gigcnlgvp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/ggkybglij.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gxsgtzeaf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzcmmopns.sHtML


<!-- 参考信息 -->