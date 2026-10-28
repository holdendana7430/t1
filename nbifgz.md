代发 wailian999

[U105] JS：节流
来源：http://hz.yuanzhike.top/gtbcrhadsd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtzvzpqsen.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gthjuuypsu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ppjwa.cn/gtjhrifbpp.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtrduhpngu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cqqwz.cn/gtjstqfjzm.html

[U108] JS：随机整数
来源：http://hz.ppjwa.cn/gtojeaviwf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cheryme.top/gtoschgzyf.html

[U109] JS：数组分组
来源：http://hz.dashuyun.cn/gtjdfqaybs.html

Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtkjdgemcw.html

[U110] JS：数组分块
来源：http://hz.andypj.xyz/gttnuqhzbl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nanxuanxn.top/gtqfanhvno.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtkkqcahxk.html

new Map(Object.entries(obj))
来源：http://hz.nanxinkj.top/gthdospfor.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtuypfowmi.html

"7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtxnqjfzwl.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtnrganvtf.html

s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gthxhwcjud.html

[U114] JS：JSON 深比较
来源：http://hz.dashuyun.cn/gtiqchjduq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtlecmvlfa.html

[U115] JS：生成 UUID
来源：http://hz.hammf.cn/gtikuiaiff.html

crypto.randomUUID()
来源：http://hz.andypj.xyz/gtaowerdyj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cashguo.top/gtdcrgjxez.html

/** @param {string} name */ function f(name) {}
来源：http://hz.havefunace.top/gtqvnscjov.html

[U117] JS：单元测试
来源：http://hz.sxryk.cn/gtbjkdrnli.html

npm i -D vitest;  npx vitest
来源：http://hz.zhaomingkeji.xyz/gtlpebxvgf.html

[U118] JS：开发服务器
来源：http://hz.kuanghao11.cn/gtfxvxgrjk.html

npm i -D vite;  npx vite
来源：http://hz.ywan-chungtsiang.top/gtwsjkwcsm.html

[U119] JS：生产构建
来源：http://hz.jiagoushi.top/gtzomhzyjg.html

npx vite build
来源：http://hz.sufxvd.cn/gtyilszrlh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gtdplqkgzv.html

import.meta.env.VITE_API_URL
来源：http://hz.jlsjyb.cn/gtcxywyvhr.html

================================================================================
来源：http://hz.quarkkingdee.top/gtoqimqiet.html

统计汇总
来源：http://hz.daxiang520.top/gtzmvrsqun.html

================================================================================
来源：http://hz.pycfn.com/gtrcjsfeya.html

按语言统计（条）：
来源：http://hz.pengpengdd.cyou/gtvemjkcpp.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gtabumuhnx.html

PHP ............ 252
来源：http://hz.wangdashe.top/gtnkxokpkz.html

JavaScript ..... 252
来源：http://hz.nanxuanxn.top/gtopxvgfnc.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtqvgcowpp.html

Java ........... 212
来源：http://hz.shuidangran.top/gtkesrjckx.html

Go ............. 212
来源：http://hz.nanxinkj.top/gtjbpcaupy.html

Ruby ........... 212
来源：http://hz.xylfe.cn/gtlgnkkphu.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtvignugcg.html

C .............. 30
来源：http://hz.bjfxy.top/gttpcrfvwv.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gtxjncutam.html

SQL ............ 90
来源：http://hz.sysykeji.top/gteadixoph.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtibimutdf.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtosfyuvbi.html

Swift .......... 15
来源：http://hz.fzhhl.top/gtcmdoyslf.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtqlmszsxm.html

Perl ........... 10
来源：http://hz.sxryk.cn/gtxqmysphr.html

Scala .......... 10
来源：http://hz.ydjk.org.cn/gtobkbydqu.html

------------------------------------
来源：http://hz.aizwys.cn/gtdjpiosil.html

合计 ........... 2106 条
来源：http://hz.yj202588.top/gtqpnvsyon.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gtobehzffy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtkksnvncj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtkbkldpar.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtujswnbxk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtklhzzjvx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nanxinkj.top/gthskxousg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtroholdve.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtqorwreml.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinqigufen.top/gtmvmbvnyh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtnarvwbim.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gteqxvfzma.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtycnthepp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtodljtjyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtayqtoynb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nwbrower.top/gtvjnlpebe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sysykeji.top/gtqrsjycbh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtwzyibwfz.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtiiiggazj.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtxvatwziy.html

S C / C++ 专题                          60
来源：http://hz.jinghuilouyu.cn/gtkoofistz.html

T 其他语言补充                          60
来源：http://hz.vqdsnc.cn/gtdmwotxhm.html

U 高频实用片段                         120
来源：http://hz.ppjwa.cn/gtqukrdgyv.html

------------------------------------
来源：http://hz.cheryme.top/gtfndycykk.html

合计                                  2106 条
来源：http://hz.yongpay.top/gtjmlxbvju.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtoniyvvow.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtzwcwkspp.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gteyzgpcxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.birdmap.top/gtdenoszrj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hammf.cn/gtwwqvjpzl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shangyingyoupin.top/gtdzjxyfzk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxuanxn.top/gtjogjtbfd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.redwolf501.top/gtgxlnidll.html

—— 文件结束 ——
来源：http://hz.aibaodan.cn/gtasllzqqq.html

================================================================================
来源：http://hz.tanke756.top/gtnxxvdkzu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sxryk.cn/gtxgxnithg.html

Common Programming Examples Cheat Book
来源：http://hz.hywenlv.cn/gtipvcvbdn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpadsujaj.html

【收录内容】
来源：http://hz.birdmap.top/gtpslleuxr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yongpay.top/gtcsozpwup.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gotoacloud.top/gthsnfcavy.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gtymmpxwkh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.birdmap.top/gttufpicqs.html

【使用说明】
来源：http://hz.hnqzz.top/gtiabkuuxn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zycfv.cn/gtcmbmuslo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenlongwang.top/gtkviwvrye.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtmdcpohvw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.meibo888.top/gtwoutsimx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtnuxqrora.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinghuilouyu.cn/gtfnhjcbtg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gotoacloud.top/gtewqwiazs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zdqjudy.top/gtbrknvknh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ybcxt.top/gtoquxpppj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fengsongda.top/gtwgleuowb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.c1oappe.top/gtkbubxhfo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shuidangran.top/gtqszmvzuy.html

【文件统计】
来源：http://hz.wangshuangyany.cn/gtzhzqilmi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gtktkugufl.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtqzmqrzll.html

目  录
来源：http://hz.tanke756.top/gtuzypkihp.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtezrpmrvx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gttzrxlyrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.andypj.xyz/gtfaxtymup.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sxryk.cn/gtefnnxevl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yvedp.cn/gtnofeinpn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cheryme.top/gtgcbebtua.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtaulxhqsv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtfstdtljn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtiuboxbin.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gttfbcxfpf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.chenzaomai.com/gtuylvyxtr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtkjwzoqad.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtkqrmtegv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gthrflbwnt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtbmkiixah.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.snrcjt.cn/gtvltnjgqc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gthfnkohhg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nwbrower.top/gtnoauesoo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhoulong.xyz/gtzxtlhxkd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jyoumei.cn/gthblzxolr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gthfvdmjvt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gotoacloud.top/gtanrbbkbx.html

================================================================================
来源：http://hz.52xcode.cn/gtfdsnhqox.html

A. 基础语法与类型
来源：http://hz.birdmap.top/gtzozwelav.html

================================================================================
来源：http://hz.guowangkeji.top/gtycmemtcs.html

[A01] Hello World
来源：http://hz.guowangkeji.top/gtxlgkbgmn.html

Py:   print("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtielrnwak.html

PHP:  echo "Hello, World!";
来源：http://hz.zhongyouzk.top/gthlkxzxib.html

JS:   console.log("Hello, World!");
来源：http://hz.yueranfly.top/gtcfhstuar.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guannengcc.top/gtlufhfaht.html

Java: System.out.println("Hello, World!");
来源：http://hz.hfpthk.cn/gttzrdptgd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cashguo.top/gtwihdflzt.html

Ruby: puts "Hello, World!"
来源：http://hz.hywenlv.cn/gtnfvulpxo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.pycfn.com/gtizmxmpde.html

[A02] 变量声明与赋值
来源：http://hz.ydzc1.top/gttogkhklb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sxryk.cn/gtshhgjrba.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gzhubu.top/gtukpnyfbo.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.birdmap.top/gtvgwyewrj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shangyingyoupin.top/gttiimbxlr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtdgcwyuhx.html

Go:   name := "Alex"; age := 20
来源：http://hz.fzhhl.top/gtzlrveqfm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yonumen.top/gtvghcqspk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jqgfzy.top/gtpydghioi.html

[A03] 常量定义
来源：http://hz.nanxuanxn.top/gtfvqnappj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuetiantiany.cn/gtczheqhqb.html

PHP:  const PI = 3.14159;
来源：http://hz.ybcxt.top/gtzpsebllz.html

JS:   const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtlernhcrh.html

TS:   const PI: number = 3.14159;
来源：http://hz.yvedp.cn/gtwcpnxinm.html

Java: static final double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtxneerqhy.html

Go:   const PI = 3.14159
来源：http://hz.meibo888.top/gtgolcryph.html

Ruby: PI = 3.14159
来源：http://hz.xingfuxueyuan.xyz/gtdengizsv.html

C#:   const double PI = 3.14159;
来源：http://hz.iojbl.cn/gttjafkday.html

[A04] 判断变量类型
来源：http://hz.aizwys.cn/gtekaghkyf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yj20258888.top/gtcjpqlzxk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.kuanghao11.cn/gtvjpjrvai.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangkeji.top/gtmrfwzsic.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj20258.top/gtalmtgfkp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cqqwz.cn/gtpmimruua.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.smart0.xyz/gtbttpkowb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ywan-chungtsiang.top/gtkuogmnoi.html

C#:   x.GetType().Name; x is int
来源：http://hz.fzhhl.top/gtimtomsdg.html

[A05] 整数除法与取模
来源：http://hz.jlsjyb.cn/gtkarrauel.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenlongwang.top/gtsbsldoma.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.guowangkeji.top/gtzqimekpz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtyawwilum.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtxmegjoky.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtidtxhsol.html

Go:   7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtvngdtzll.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtvtxbpkbz.html

C#:   7 / 2; 7 % 2
来源：http://hz.0kj1m.cn/gtmlsrkqzw.html

[A06] 字符串转数字
来源：http://hz.kuanghao11.cn/gtojfrsyte.html

Py:   int("42"); float("3.14")
来源：http://hz.cheryme.top/gtbnjihzhl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.smart0.xyz/gtammtgmwm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinghuilouyu.cn/gtldsfgrig.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yueranfly.top/gtpfasmfkg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.316326.xyz/gtfemebsag.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sysykeji.top/gteyacwimw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jiagoushi.top/gtglujndys.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.svipenyu.cn/gtaaeiaepa.html

[A07] 数字转字符串
来源：http://hz.c1oappe.top/gtyngdqepk.html

Py:   str(42)
来源：http://hz.yuxming.cn/gtvnmexssw.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhengqikj.top/gtkrznvioq.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtcukeuiwh.html

TS:   String(42)
来源：http://hz.ydjk.org.cn/gtlzpnjfpq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jinqigfzy.top/gtyhbbydzv.html

Go:   strconv.Itoa(42)
来源：http://hz.xziqi.cn/gtwxivnwyk.html

Ruby: 42.to_s
来源：http://hz.zhengqikj.top/gtnivavhen.html

C#:   42.ToString()
来源：http://hz.sweek.top/gtjlwczebd.html

[A08] 取整与四舍五入
来源：http://hz.xziqi.cn/gtpimbngco.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.birdmap.top/gtvsxiqidc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhongyouzk.top/gtwzywsbjr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ybcxt.top/gtkqwliasd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.birdmap.top/gtxkjnokxj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.smart0.xyz/gtjgusncui.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.sxryk.cn/gtnfmypqzu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ydzc1.top/gtolxueiaq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.guannengcc.top/gtjtycjbad.html

[A09] 绝对值与最大最小值
来源：http://hz.tanke756.top/gtfgceulil.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtepdnikig.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.0kj1m.cn/gttrobmqwc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.shuidangran.top/gtazkekept.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hfpthk.cn/gtqehtjtxd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.daria6918.cn/gtzqhdsngw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhixingplan.top/gtnesekncp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.pycfn.com/gtqrkdnmnh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zycfv.cn/gtdlgxkemj.html

[A10] 生成随机数
来源：http://hz.andypj.xyz/gtjmxhsfqj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zdqjudy.top/gtxlsadmqv.html

PHP:  random_int(1, 100);
来源：http://hz.ydzc1.top/gtkptywkkc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.meibo888.top/gtmsowazsu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.aizwys.cn/gtbexxxhtt.html

Java: new Random().nextInt(100) + 1
来源：http://hz.guowangkeji.top/gtxiddglig.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.tian-w.cn/gtkudyvgje.html

Ruby: rand(1..100)
来源：http://hz.hammf.cn/gtdvepksyz.html

C#:   new Random().Next(1, 101)
来源：http://hz.yvedp.cn/gtqnibrimi.html

[A11] 条件表达式（三元）
来源：http://hz.sweek.top/gtelmxxkbs.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.nanxuanxn.top/gtfzrtvbdu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtlmscbuvq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gtsuwlhkdt.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtkvdehmnq.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtjpclnloj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.havefunace.top/gtsmvzefei.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xuetiantiany.cn/gtssttpuaf.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtfgagdfsk.html

[A12] 字符串插值 / 格式化
来源：http://hz.tanke756.top/gtuicelbof.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.xuetiantiany.cn/gtitloqjrb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jiagoushi.top/gtxtujmdgx.html

JS:   `Hello, ${name}!`
来源：http://hz.jqgfzy.top/gtnmylqiob.html

TS:   `Hello, ${name}!`
来源：http://hz.yangfankeji.com/gtsokmitws.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yuanzhike.top/gtdiexmaxf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.c1oappe.top/gthktekzgr.html

Ruby: "Hello, #{name}!"
来源：http://hz.tanke756.top/gtlxzqnvfz.html

C#:   $"Hello, {name}!"
来源：http://hz.jianghu66.top/gtmulliktk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.316326.xyz/gthbqeuqzh.html

Py:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtdtxeumou.html

PHP:  "第一行\n第二行"
来源：http://hz.meibo888.top/gtiyddmsdr.html

JS:   "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtyqtwfyzt.html

TS:   "第一行\n第二行"
来源：http://hz.cheryme.top/gtnfjzikeu.html

Java: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtzlunmxry.html

Go:   "第一行\n第二行"
来源：http://hz.yanxiufei.cn/gthgfqdlzz.html

Ruby: "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtjroystva.html

C#:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtusaxnsvq.html

[A14] 注释写法
来源：http://hz.zhaomingkeji.xyz/gtzfdxyahh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.shangyingyoupin.top/gtaljyvqjy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtlprwrrxt.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtgrxfydrd.html

TS:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangtech.top/gttapmpcpq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.daria6918.cn/gtwkjrfigd.html

Go:   // 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gtahalamcj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.haohaochexian.top/gtssxaixsm.html

C#:   // 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtquwwsdct.html

[A15] 空值判断与默认值
来源：http://hz.gotoacloud.top/gtjbopjufh.html

Py:   value = data or "默认值"
来源：http://hz.tianlin.xyz/gtlseximuj.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.havefunace.top/gtwhggogwk.html

JS:   const value = data ?? "默认值";
来源：http://hz.guowangkeji.top/gtmqijdqsr.html

TS:   const value = data ?? "默认值";
来源：http://hz.cqqwz.cn/gtdcnomtvw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.aizwys.cn/gtwtigmqqm.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yueranfly.top/gtywougxms.html

Ruby: value = data || "默认值"
来源：http://hz.hongshengwenyu.top/gtpnpvqqos.html

C#:   var value = data ?? "默认值";
来源：http://hz.sweek.top/gtwramoswy.html

[A16] 真假值判断规则
来源：http://hz.xziqi.cn/gtyyqgbnjh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.9152youxi.cn/gtquhifdqb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.fengsongda.top/gtbelpjlte.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.smart0.xyz/gtgdlupnue.html

TS:   if (!x) {}
来源：http://hz.bjfxy.top/gtqvpqpajx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cheryme.top/gtkdtjbmmd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jiagoushi.top/gtwfvnghwk.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.tian-w.cn/gtdxenmepc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.kuanghao11.cn/gtxxpuojfn.html

[A17] 位运算
来源：http://hz.52xcode.cn/gtafpgjdyd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtexrhaalr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.nanxuanxn.top/gtnclpldmb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gtshdvtmze.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.daria6918.cn/gtpxgousgf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtddfxynnj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhongyouzk.top/gtpbiamoaj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guannengcc.top/gtlzokeoup.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtxyhipkhc.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yueranfly.top/gtyvznlrlr.html

Py:   ord("A"); chr(65)
来源：http://hz.c1oappe.top/gttrkgxsuz.html

PHP:  ord("A"); chr(65)
来源：http://hz.wangdashe.top/gtiukvtkkw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhoulong.xyz/gtcxhckgdk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.dashuyun.cn/gthmeqdose.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhoulong.xyz/gtwavehqse.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jqgfzy.top/gtcihgicnl.html

Ruby: "A".ord; 65.chr
来源：http://hz.cqqwz.cn/gtkeoohlko.html


<!-- 参考信息 -->