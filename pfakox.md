代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wgnolxrp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iewezeav.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zatdcrxc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qxohemam.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ilnhmhai.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2finvrpmx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2syfhgtki.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2waswgabm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ititmfgk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qyxkzefy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vegcimxy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xzjpkcut.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dzncgplj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xsdycnbv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2napzitqu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ofulgqui.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yyqkapjb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xuunqvoj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2teyajcsz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hlevudhi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2aungrotk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hifqsqcs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2prfxzpul.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jzomyvuw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mewuhxvo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2icjdmzmm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ahynjvmv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lmsdivze.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wtibqmbf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qvcmangl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hqjbglkv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxzoosm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aexybofv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bdbkqpyr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gqztmumc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdtpotnb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jozockyd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2elfwqzuf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2rnjeiago.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2teurtgdk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2irfrnxap.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2uibotvfs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2scxbqszr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xqxayfda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhbeuwlg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ddmixrvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2octaaqfc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mbfqqnmg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fzqnsewc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xluudqnd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2izigweaa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ldyngnnk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2owuicmuj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hizdlryv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2irohzhgf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gmyqpbmi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kndgckhc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zeayshma.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zbahhbha.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xifebuvh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fnpncdtl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sgcqlgcx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cmvbqfwz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljickgzi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tbavkedb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wwloulpa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nzndrluh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rltyrwvn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2npbfkcfu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dsmjbqia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lqjhztzw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aocxmgpx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hvhrgstn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qmoiwwef.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hroeuxvm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ckzicoja.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tktfvcze.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2osjcmmhu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yiswujif.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qsjhxwog.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yqueyecb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cevqzpmr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xltkxwis.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2msoliuhp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2acuasywk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xxvpxais.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gcuieilv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lysozufj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2iiptinqc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hwcerypv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jsfrfayl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uzewltss.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2gfhmsjab.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nnifcuec.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cqlvhwds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uxqykspn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2miimzbkm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zbvqwmky.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2osmlrjyk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bawvddfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lapiugnj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2blfjjtwt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lqevjxcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nurwkcny.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2hotyqkcn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wjdbftby.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2zhstvios.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2eeluqkpo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2yzvurpll.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pevkbcfs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2aepnlxjs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tdwrcgae.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gviadhyt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2pfkdhmho.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zvzedjbl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2baukwmhp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2agzsyulo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zswmsivc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ksskajmw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2swfrhyry.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ujlartvv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ppvikcpf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2sysmhpbc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ezcoextc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jmwsdero.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2nlvsbezo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jjxkmpcg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kbnkbllr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kevachxt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pycqkzzw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2raftwmkk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iurpvufd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zkwesxmf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rvdunrrw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cwopibum.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2obzzcidw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bsmtpwsp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jumiueoi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahlxekvi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rrdulpva.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2aijqcyfj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kraztnsu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jqytdzqx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clstczei.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qlkcsjhp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eydhavvx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fyycevjm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2umonwgmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkavpnan.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2honyujgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrimevoz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynbemiec.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kbarluoj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ooyhfrjo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eigqqivm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vmdyydpj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tlweplhu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2blcvdina.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwsdsnes.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aigupblb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yzkopnrn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2blcxqpjz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ukcxeiqh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bysuuajt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2fgzmhjpr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fdpbztvq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nwaikfhy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zxihfirm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pdfsfpiq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rzkdiasn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2kzrudxfh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qkjrfuft.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2akrmxqss.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2amsysmew.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mtiizrvg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jcvbmtqh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2egmbozcq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qdrgyunf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2acrtniqm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2uskdwnsw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxefxbm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tpuauocu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hkjsywrj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kekmhtgd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fsuzneaz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ouyvljsh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ieisspzo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nddvkfpt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wyyvknvr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdvqjfij.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ugwwlpyu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uatfjemf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gmzgkucb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cpyfbhfh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uabfjspx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ortneooe.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ismxlgrl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2djqlfafg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2wwiaoipb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hkvhztcf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ipglynri.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qablkmlt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2wxzhguor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yvxwulvi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qrbxzjwt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcvvdann.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cznezqwf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qsnouahg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ejljcrot.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2meeiqgvn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ikmaxxjt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2jnnarfyj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ugiaqvgm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uyonikjm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2btdwvrti.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lqsaqydt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2lokwqsqj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sgohoujz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2omiagidp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxdgnok.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wllsaosi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2weircjqe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bnyavrts.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ekspnwhc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eucnuepi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tshsgmjy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zfwliyoy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqracnnv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2igzjxbyp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jhjvnlip.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jkmygouh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xazekxci.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kprugpab.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqxdnsu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kurkqywf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhgtgg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ftpvjvnp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wouooymp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2woblelac.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2wnjuqrts.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvhuoxi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2yqlksdhz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2epiveqjm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vsmmypdc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pfuaqnzm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2irdastal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2utobfxdy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gyxiuxqx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hopxpzrc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rulkiabr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2thxkkyoq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zykmmrsj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2idoyxhfy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lmkawpmo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cpgrlrmk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2idjddvwz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2zxapurhy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2umxbdhas.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ctqfqmkk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fgiyvtax.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aguikosk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fzlvgkhs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ysutbcvk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obhmthyw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2piidagbr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eowlwuup.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xjoopsih.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2asqnwjlu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ayzgnrrw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zldetbky.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mbdjynxz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ajfqanea.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ncjdpkgs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qdwtefvk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dgrhopqg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kucbunaq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zhernyan.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2licvuwsl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2phrblufw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2snmzlfhz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rkyvdqoa.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rdsjdmlh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zkuilbvd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qwffquff.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kabmzvbr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zyonkbzt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dgdsnavh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2kdpbndnk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hcmegbmw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xvlvhygj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocjivawp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsmdcyff.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2sabmcwrr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kwqnbtrg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qngueayw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2srdhclyc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkrpgsyq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rreidjvm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwkpdfzr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jnzcufre.html


<!-- 参考信息 -->