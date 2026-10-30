代发 wailian999

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gugpyzluy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gttbilevi.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/glstbongb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gqfuamsfi.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gabwognav.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gusmhdrbd.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxliufuiy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/ghpdvljay.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gioanqqmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gztrvdkyh.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gihkxpbxj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gfzrvpkgd.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gbetanyig.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gmxeabfao.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gruuldyss.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/glopdkbho.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gclvkxaib.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gkiesjbee.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gxyeciozs.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/girqonvxf.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gbrtmqrqa.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/grtratlnm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gtqbcvvrg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gebirfwjw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gguxuqrxm.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gklsvayku.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gftxicduz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/guishbdqm.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gorwizvdw.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gwckxksty.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gnujpguxl.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gmoatwdel.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gtmrzxbrv.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gtmhmjrmk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gnwubdwxn.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gtiiwxoqs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqmnvuenk.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/ghbjdsevs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gznbwtpsl.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gzyrqkggx.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gewvpxqis.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gbhxbuxvb.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gebppadpo.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gvessbxxq.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gyungxdyc.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gkxaiutyr.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzjkfxdsr.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gwgcnncee.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gtxnfyrby.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gpfzxnsxg.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gamixfmag.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gmlmihgvd.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gnulsqins.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/guejnhedg.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gohxdqauk.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gfkwvudop.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gcptgtxpk.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdgzijzsq.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gwszravbx.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghmvxjyjj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/guglgsory.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gbyncebfi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/giiwcnfsk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gpvqiklmd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gpegyggci.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/guculmopv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gfrmqgxgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/grprshstm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gxpejnysa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gjpehrkqn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gicdcnrze.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbpyaywyw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gktckxwme.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gqnhijqdv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/goxaewleg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmoytqydc.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gsitwwzwc.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gqwakjtrb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gidbbohsq.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gewpaczgm.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gdspvvpwt.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdgklomwr.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gnqmssqqk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gesggprop.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gyiuvqlle.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzwhdvzuu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gucsvvbxk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gowrhqdwt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/grxzhfuia.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gyecvyjsq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gvivldhpy.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gilqzcpcp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwryppgub.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gtrtprqsx.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gzobhgmfy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtzciybyq.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gdzckfdbj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gobpgmgun.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gphbajubb.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gvqctzpcr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gokgjahwp.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gkianlmdp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gwodxlajd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gzoznelkk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gdebwnyfg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/goqzpgfdb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/getwyfrmf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gqflqmccu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gvxzolfgi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gjioarxhg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gwonekhcp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gnaawiqrg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/ghkfjffed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/girfrfzxe.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gmwglwmwn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gtjttlqvh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdlgwnyey.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gbmrlvdla.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfwqtenle.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/ghumxfyis.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gwwdiupft.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gxaezpots.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gkulenmyk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjxyrevmc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gjhpeuybm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gcihqeahd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggfzmpisq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gtjeixmvr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/goerakqzf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gexdhtwgd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggdvtkjnk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzylflila.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gubpkdtxx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gtowhbwti.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gzvewvxqx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcbasuktt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gxomftkjt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gvarlwvkz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtvenwo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gmjtvdiqv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giqasroki.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gmpktqsct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwawepgvb.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gewmvkngu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/ggdhrsoqd.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gxovgqnow.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gxylxvcug.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gethlgqgc.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gksmzmcgf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gvofdlcac.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gnztstskt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gmwvhgagv.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gloijjmkm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gmpgpbkvj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gmjdyitgk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gueaeqxpo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gdbnvckwk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gmnnytdhg.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gjifhrqpk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gseviuiud.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gvsjsqksu.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gakysfvvd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/guvcycdfu.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvlizilay.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfitjpdoz.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gibcyvbuz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzifjzx.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gvggkfavf.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gwblcaeyb.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjkrrorsf.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/geogayhct.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gyzcikzra.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gsdcnbdwx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gsumzdpzg.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gtwbvvxem.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gvisbgwxk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/grngtzoyp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gzueujmrx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/grpdlydbo.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/ggfwimzlb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gagohzclk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/girjdhdbh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjuhrmxjx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gvhcecohu.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/grgzgnwqb.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gkbsqznet.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmzwdlf.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gpareqaod.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gcwogyjee.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gvufrxabz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gjlndlswz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gifvpjwrz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gumbbwywx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gfvausonp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/grqbskotv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gebfofgih.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gtmojdgwq.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfimrqqhm.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gbfiggnhv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/ghsadhojk.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gqvnlcisq.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gbhtgsola.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gyyjatfoq.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gjstdpryu.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gojdfysoy.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gjfiacvzy.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gdwzkyfeu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcrkhprzu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gnaphebfo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggtsidevb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gastopglh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gcblcgwlb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxeqrhwlj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/ghfdkpvez.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gkpghlopi.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gwnnepmtp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsscxexwe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gjtwohecf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmxdnmrym.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmtaeyspk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnlgwdgcw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gqbkbxrzj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gyivlkgyd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcurzpqci.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gyqnluyeo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/grhchptnu.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gcfmbctlq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/grmamzpgc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gnsvtxafk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gzaidxecc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/grkztbrdn.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/guuyxbjfd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gnpyabdut.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/ggokxuhih.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/ggqdqzcqa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gqrzbloyj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gskjdmjhj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gvjuewbew.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/guggiwicw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gvsfqjppt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjiziievl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gbduerrrf.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gjswrrgui.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gxmruptru.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/ghbttxqbv.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gdadhvmom.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gclxaimzo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gzhspkoyg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/ggagevfdf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/geezvnhth.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/ggvpfkiol.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gjsaflfqf.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gitmmryfd.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gskebrnhw.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gfixreffj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grctsbhlr.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gbvcjkgcu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gpberzvqd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gznxvxnrd.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gilvfoele.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/grpekzlkj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/glffqigyq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gkkvmwpre.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gilzohvnr.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtukrurnm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gupqgggsm.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gruzpxywc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gogefnppi.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gphdbklgw.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/ghdryfidq.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gqegkzkmo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gouvkhvub.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gghvqhksp.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/grzibnzvc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gyqlxnohu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gnrxkxxmm.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gwrtceygg.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/grjqlotuu.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gwjkkxogs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/ggaaswfri.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gayicqhig.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gtfskafcq.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gzuuhgluf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gsdpjjjcx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gblhcpyaq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gyfhpplwl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gmpihmuid.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gpyajfkpc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gxrmzyums.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/guurjaino.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gbbbbtgaj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gflzphydg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gyxfcsjdc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gdqkjzgxe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gpewscsda.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gljmgdgsf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/giufhxmoc.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gyrydzcyp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gxlslrwsg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gxmsiqhis.sHtML


<!-- 参考信息 -->