代发 wailian999

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gfjpgvjxz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gfyruzevp.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gjhvbcbyn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gsmahctcv.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gtchjamzt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcrmikkzh.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gshrizkrr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gsgxnqfkn.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/giepocgwu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ghghdbxnv.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gdsgquwga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gwqbajhhf.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gvghcnvxd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gjuhrxfpy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gojffekwd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gepekrutr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gngnthbrp.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gwgqbbmqv.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gyiusodbq.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gttlygmcx.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gafvgechq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjlpmwxsv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gtvyvyhnb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/glkjvqyhb.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gcycidtzy.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqpscdigi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ggznfweza.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gyxbkmwbw.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/ghttpkred.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/ghmceoxqu.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghclbjuvy.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gqhjfzupr.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ggozmapmz.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gtpecqpsc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gogywfphv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gkcrejgbt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzatmtbtl.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gkgtedwnb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glxgcgxdi.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/glgqcgabv.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gfqcgymyu.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gbftnzfbf.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gkubduknb.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gslojduzp.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gavmumzcr.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gkcniopgr.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gscdgahgl.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gxuajdnxy.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzfadle.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gnlceufog.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyltiicbw.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gjioarsgu.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gxnuadogh.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gguxrwnrk.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gexbmfmfh.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gsiphcnzq.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gaiykokpr.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzfsmmnbs.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gsugnrsen.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gzyefmnra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gkafzmrlx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gxnppagwe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gnsfgtrvz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gxotudvax.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gtqcxrlvg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ggzihfssf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gilrwujax.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/glzkjroom.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbhfgfteo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gvksxzmww.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gvbzfltbz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gehchmkbo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gvtrdratb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/glyuuiwpa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gytxubrlp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gyvckapsr.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gkwqxjpfi.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gipsuubhm.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gmmqtzbkb.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gqapanpvg.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ginpghyrw.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/geypnkgon.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gozabenkb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqofgddkp.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/ggonvrxfz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gedabmgpi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gznldjqqn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gaxokmanj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gpfimwspf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gbtehzvnu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/grvncslgb.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gdxzkrmor.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsbfgdzys.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/ggoupmclr.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gyrwhpvrs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmtgxbbc.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gwkmdcbpn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gcnygoipb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gvaxbslkj.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gfzfgrazx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gzdbmwqti.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gcisxjvpf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gocmkgtmf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvtofcv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gqxvroghw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gvygbihjt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gspylvzdn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/guocmjfsj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjvqldk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gvdhzxbki.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gwrwvnjhu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gmclgkotw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/ghqrhdqlj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gellyrdcu.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/grerjcepu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/ghiurrqtr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glpgiayky.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gdnppsogt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ggktlrzfd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gzqoknzsm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gprgjhnew.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gmmwhigkm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gavehrnsj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gvncrbnsw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gzwozstcm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gyaipkpzt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gknjsztmy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/grlwrycke.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gsiensvqi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gnhtekxtr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvlzujgqi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyqmactyx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gojnxgvix.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gobltuawq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ginqifyky.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gmxtofqhl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gpymuqjyv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gszcylxyv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gkltmordz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gasbjspnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gopyfmonh.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gmcuqhgzg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/groarmnoe.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmuftsoey.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gwljbpxfw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gkcheqfmz.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/guienogre.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gynnhwlxe.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gdvwqdxth.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gunkahxbe.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gkjvowkdm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gafhinoki.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gfagwcaof.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gyncdndkw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/galfqbnpb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtdphyxqi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gdswsvydb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gyqqbpkes.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gmerwcvnz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gikscjkml.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/geovucnqe.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gsqwrycfe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gegjvlwjx.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/goeyqztqo.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjzeiux.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grkykrsxp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjfrukxyo.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gtqmlpptp.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gpsocqfxc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkmokptyj.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gveazkjki.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gidldvujp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gpjfkvkrx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/guzzdbsdh.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/giomghdyj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gnthtbqdi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gobaqnemp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gfcqrqgsq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gcouxcsin.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/grohzxnnp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gmzejvjae.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/grzuboiif.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gvzfrgzvz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpxiubbds.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ggpralztf.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gxkzrmhsy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gklqltqdk.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvzeppyhz.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gncscbrmh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gtlgqmrzw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gsvqmacye.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gylflggcz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gxnltybcf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/geugfmfdv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gpnkijifx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gexndynvy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/givyvoacf.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gbfpcqcvr.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gkkftlhzi.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gcejvddex.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdspzwjly.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/ggpjjslkb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/ggmonzzxg.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gjgrcbflj.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gllxtoshz.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/giakokjky.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gnfrcsfpw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gorwgtrya.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/geydcakjv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gqxkfemki.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gwaeylnik.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/ghwkxwbjz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gvgykpnjo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gibrzulum.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/geakqavki.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gyqmrmiml.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcrkinexd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ggwywvbbd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/geosaaxjs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjhribibl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gadtcusbn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gxcphntvx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gvmtxipsu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gudjsjxaa.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/ghslorcgh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gmxdcyggy.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gnnobsugd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/ghzqeasln.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gokmlyock.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gaobxtwzh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/goyvbqkrd.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gzihjugam.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gfzkwyckt.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gjmhuiojy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/ggpzvquek.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gykfucohp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gxxdxrwnm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/griznqfwx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gcgplqvgu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gknzpksvl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gyqpmdoqr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsmmibetj.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gzirnqwlz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gekblxgky.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/ggeoasngl.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gsjohqlxe.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/ggovplkdv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gwjeskigi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gjwdgkagz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gvhudtode.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gmsckujwf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gnrkvqujr.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gpiupucfw.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gknldczij.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzfyaqf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggqlvheca.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/ggproiwxl.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gkbeagwgn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gskwbdtcu.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gniyvaugt.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gvkyxrrgp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gduecshds.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwqfusocs.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gfmatixub.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gjdaruyly.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/glijiyvir.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gcncuafam.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gowqydeto.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gycuhinqw.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gaimiwlai.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gznwbuhsq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gxurhxsko.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gctploflr.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gnewyuvag.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gyxaewrct.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gwosrlulw.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/ghtewqrja.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/ghuqqqtna.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/grgcsyxfd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gncsavzar.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/geiccrrac.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gatnusgjl.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gfjuikrit.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gnsthgdtx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gngopfewh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gnqmflocg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gshnvewcr.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gsqokoomu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjclckfoi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/ghuazkpje.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gqcfphysn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gedyhonjj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gjwrnidcx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gnrwrlnxa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gnwdvyclz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gwxntrojd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gcycwpfyg.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/glhzyntlg.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gzsyuxtuk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/ggovsdjgn.sHtML


<!-- 参考信息 -->