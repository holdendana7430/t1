代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xbsifoss.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hhrqjjfb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3scuehtcw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ghjrdukh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dauvduya.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3niufpscf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mtrncoja.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fjbnghby.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xjsihpkx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jeukpekv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cwgfjdbb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lykqzgpv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ebovbznv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bfglmvgs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qbrzqzla.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ylnptqlz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xnpfkymj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3attpfdgo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3spmopsbu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bqqoaskt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vqapopkm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3awyegarb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3auhvqbzu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fjgrmtri.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3owvwtjqf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fusqbfdd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3yeqxngmq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fubgfmdm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yvrzrhif.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lopshqnv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fkbscqih.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tqwnfvrn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pqsjpjev.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3oeawlufu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3stvevpey.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xeqjhadh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3huzitajm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ninnrdwg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jzihmkeu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3oouddxeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbenmlpi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ohbpqwpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzhkpppt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jwzqaqeo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tnvzrwzh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3oirneije.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zgzclwsn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dztyoknx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3svaqgpck.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gzbkzbfw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bdsyyueg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3brmmkkce.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xvhgniyc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dzedinfz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lrfzysja.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tuudnlsl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cjelqoxc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fuyhdbuy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uyxemjrh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eiirdegl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xbxkmunq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3boxmxxdg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3iaepqrfg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zkigwrdx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3raaumkwv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3htoyghfp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3behkawye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uvdevuas.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ktubzltd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ypspqrat.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tqnadbkh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fkfdbvwq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dkkxwyny.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ffhtabmz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tosdlamc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zwfxfrdy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3motfryyg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vubhvtkb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jieyjrvj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gkrlzfnh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3okfpofso.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yzydjnjw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3snuyzvsr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rlibcafw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tgdhzmms.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sidlqrrs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nmyglujx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ksgplfjf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fntngrdk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tfubflav.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qhzgdxqd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ibnkctmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3gtwjfdvi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dxghvtux.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rhmlhvgi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3anfghkoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfapajvx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jongqlhq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3chwrgtcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pygccwvb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mtugvoub.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wfmvnbkr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jqwxcjut.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3eosyzmrz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3cgrjcush.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xhlbvqgw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3anjoubty.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pnhwkvgy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rckrzmpe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hzjgqtmc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3glmmazfm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gytixvdp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ztlsflvy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3yoglgzvu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3flqcrocb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zjvhczjx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3housmydx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3cjgchszi.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3olvylssh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xxtzxpas.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hhccozdj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3fxwzyzpk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rtirsely.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hastmxsu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3atnkagyz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3havzdhvo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wmbgagqq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3veejibye.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etczsdez.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pjbdigwp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hxwytquy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohrqisxg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3siknavps.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uewzfaqy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3okaifhes.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrizsirb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yfqlzbpn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wrnkzdbh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ynfylkmc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eagrdlzn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tibpsxpi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ghyshnzb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rhbmgtgs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aabjdhyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxsglo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3wrrordxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxgytfwr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdsqqkyi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3penuofzw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jkymzvev.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pvifgzvv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bwiwdjfz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3geijnqwn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tjwqkmnm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rkfgchzn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gktxfray.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dsuzdpwn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vekfandd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wihtrips.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iwecgeyk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3osrrxelr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wnxylihr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ecpzxmeu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ramcnnkd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zuattzyu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3euosbpok.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3psfnvfpv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xcjeheur.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pbwhoyvq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3paeijhng.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ulqdwuua.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zalszysd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3efnkepzr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gbdktcpd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rrrwwdng.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cfpnthvy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3syxwejxj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vqtyyzzk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xdhmuukx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yfjqirnv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hyokbeem.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zvnzfwnx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vwqevidj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3yhmpvsow.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrrzzlzg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rellgpak.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kqlxjxka.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zutvdfux.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qazcazrc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jhkcjcpf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dhnkwjlb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3flpgryfz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ngltslwb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wosirwit.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bwskkewr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wlkhsqvd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zzhnzdrk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3iggyhhty.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3mfbuytjy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hioswhjr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yawjxigo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3jpcqvjzr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3difgaffy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ofuijnxd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dowudrxp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rijgmukv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmjkqvh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cqydvwuv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3woabrbzm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lmtwpqfh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3udnhdlgn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ctybbkvx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qaxgdlso.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ukjfykjr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ryduxdnj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xznjnnfd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnlggdz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xhlkiglg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3owcnbubw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3muonlogw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xvfvwuvj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdlhaga.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdczuonw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jminiywn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmpvobhh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wmrsppga.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ddzrlkeh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qzilewjq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vpytolao.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3flopaydl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rjgjtfgj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3emfmfxtp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxsnjctr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fofqphwc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vjadrmrx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3umqswngs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uyhnzdav.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vbsxwxqd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3sbjchqjs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cnoksmfv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jzgryisg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3clrapkdk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aimxyjyv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3egnhdrdh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hntavfgi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3klxsldbs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3cffyynzj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjbsrbog.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jjrwepev.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3drzazfrr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mkltletp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rgykmsiq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xifgmqnt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cckjobzr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vldhcuga.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3riivujwy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ccehzmsi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nxxbaast.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rpggnfxa.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3amfvjddy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yzqmvjkf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gtbatkox.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dhsqzmzq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ccimamkm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wmzdvopz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gxmvifex.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zlxukcwp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3scsczyll.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mwbbjnkt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3udgotspt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yzsvpacs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3umrjadsi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mfbubeoz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3juknafnb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ppjpcljk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3chwzlbax.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jenuyfdh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3islowwhv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pcinoecc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3muxycctc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ymuetuum.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cxbpnzsr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rksiondr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wnelgjcm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pdcxajer.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3mvpdpqja.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kuujmzzw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sztqledu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ytuuimja.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gacfxhqe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ltudkqzl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tiyfjtwg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mxmhcmmx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3olkmnipn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3benamvsm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hzeginta.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3odpaqekt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gttopsgc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jdnapjzk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xuupjgtu.html


<!-- 参考信息 -->