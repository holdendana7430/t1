代发 wailian999

[U105] JS：节流
来源：http://hz.yuxming.cn/gtjtjrymrl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ehwqpu.com/gtdxenzqbt.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gteatzqofh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gtrbbvdazd.html

[U107] JS：数字千分位
来源：http://hz.gaohongyu789.top/gtobsqfeed.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtnqealsab.html

[U108] JS：随机整数
来源：http://hz.aizwys.cn/gtfjhufsbp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtoyqrzfje.html

[U109] JS：数组分组
来源：http://hz.meibo888.top/gtawzlihka.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gttcjezidw.html

[U110] JS：数组分块
来源：http://hz.jinyuanbaomall.cn/gtwojqafns.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gttbilitio.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtcqdtfwco.html

new Map(Object.entries(obj))
来源：http://hz.9152youxi.cn/gtpwmvzcem.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtmarjsxum.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gttsefqvtc.html

[U113] JS：正则替换全部
来源：http://hz.jyoumei.cn/gtkgsbinmg.html

s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtwuhmlrng.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258888.top/gtoobcjtua.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtmvomvsqi.html

[U115] JS：生成 UUID
来源：http://hz.yuxming.cn/gtrqqdezfe.html

crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtykgknzyo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuanzx.com/gtshbzxylb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.quarkkingdee.top/gtacfsrjrc.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtdestjpud.html

npm i -D vitest;  npx vitest
来源：http://hz.sxryk.cn/gtlofttlwj.html

[U118] JS：开发服务器
来源：http://hz.52xcode.cn/gtnemmnbpw.html

npm i -D vite;  npx vite
来源：http://hz.wangdashe.top/gtoriziswk.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangkeji.top/gtezsntcsr.html

npx vite build
来源：http://hz.0kj1m.cn/gthkasosfj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenjidiqi.icu/gttkpeears.html

import.meta.env.VITE_API_URL
来源：http://hz.zhongyouzk.top/gtywasvlvw.html

================================================================================
来源：http://hz.chenlongwang.top/gtulfvlizd.html

统计汇总
来源：http://hz.shzxlz.cn/gtxuionhva.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkumytynv.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtcxmwfgon.html

Python ......... 252
来源：http://hz.zhengqikj.top/gtaonpfttb.html

PHP ............ 252
来源：http://hz.xziqi.cn/gtufscsfqx.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gtnphvfugn.html

TypeScript ..... 212
来源：http://hz.sysykeji.top/gtrxocibyl.html

Java ........... 212
来源：http://hz.hfpthk.cn/gtbrlzmkdf.html

Go ............. 212
来源：http://hz.hammf.cn/gtmatwyimk.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtohbwdcvg.html

C# ............. 212
来源：http://hz.jianghu66.top/gtdpkmwbum.html

C .............. 30
来源：http://hz.meibo888.top/gtcgrmbhtl.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtgqcmyzej.html

SQL ............ 90
来源：http://hz.chenlongwang.top/gtjywsfepr.html

Bash ........... 80
来源：http://hz.tianlin.xyz/gtyrqmgknj.html

Kotlin ......... 15
来源：http://hz.jiagoushi.top/gtrsqxzwfx.html

Swift .......... 15
来源：http://hz.jqgfzy.top/gttzozekeh.html

Lua ............ 10
来源：http://hz.nanxuanxn.top/gtwwcmwkzr.html

Perl ........... 10
来源：http://hz.xuanzx.com/gtnsryzgsi.html

Scala .......... 10
来源：http://hz.xuanzx.com/gtlqhhhtnz.html

------------------------------------
来源：http://hz.ehwqpu.com/gtsirbatys.html

合计 ........... 2106 条
来源：http://hz.cdnleiting.top/gtaelzwkix.html

按章节统计：
来源：http://hz.nwbrower.top/gtkrvxwmnr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtwagrsnim.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtvuswaphl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtmeyzunis.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yangfankeji.com/gtqgaxbmlk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuxming.cn/gtbkwesygc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtnsacbmur.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtijapebpu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtdekkrlkc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtvgaalshn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tianlin.xyz/gtvgkbtrwq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtqtfvvqcc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gthonbgzwo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtalcxtgrf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cashguo.top/gtcendzavo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yueranfly.top/gtbaiqofzo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gthobogjcj.html

Q SQL 专题                              90
来源：http://hz.chenzaomai.com/gtqedjxqqh.html

R Bash 专题                             80
来源：http://hz.tanke756.top/gtpoyomnss.html

S C / C++ 专题                          60
来源：http://hz.chenzaomai.com/gtpoqjryov.html

T 其他语言补充                          60
来源：http://hz.nwbrower.top/gtcnmtvnyg.html

U 高频实用片段                         120
来源：http://hz.ywan-chungtsiang.top/gttpqmpvfw.html

------------------------------------
来源：http://hz.fengsongda.top/gtmpkgblve.html

合计                                  2106 条
来源：http://hz.yonumen.top/gtanvrjzzp.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtnkvqcsfv.html

使用提醒
来源：http://hz.yangfankeji.com/gtgpvhxnwt.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtsnmcwuvx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yvedp.cn/gtofxungsp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cucudq.cn/gtzjwrmcnr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.iojbl.cn/gtcajnckix.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.haohaochexian.top/gthhcigxnl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yanxiufei.cn/gtgvyfunnx.html

—— 文件结束 ——
来源：http://hz.chenlongwang.top/gthlglosbp.html

================================================================================
来源：http://hz.52xcode.cn/gtrfcswxsw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuanzhike.top/gtneetykre.html

Common Programming Examples Cheat Book
来源：http://hz.fengsongda.top/gtggpqbnap.html

================================================================================
来源：http://hz.pycfn.com/gtjnkhcxhn.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtdhrapmjy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gotoacloud.top/gtvngpvnwm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.guannengcc.top/gtxeohptxc.html

SQL · Bash · C · C++
来源：http://hz.hywenlv.cn/gtpbtufcfa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.52xcode.cn/gtphnybgzh.html

【使用说明】
来源：http://hz.xuetiantiany.cn/gtrvkcqdqg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgufenzy.top/gtrlipeowp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jiagoushi.top/gtqoyulgus.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.guowangkeji.top/gtuwetuliu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hysaishi.cn/gtakvoctad.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dashuyun.cn/gtaszfybsk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ywan-chungtsiang.top/gtrdnbrpoo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.iojbl.cn/gtnrmacgdd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ydzc1.top/gtgyudecss.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gtfusemfbg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gaohongyu789.top/gtgeymaxnn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.birdmap.top/gttkmbriii.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hywenlv.cn/gttozuwjiy.html

【文件统计】
来源：http://hz.daxiang520.top/gtdvymzpjh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.mhx1999.top/gtteqrjzhl.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtchflaybk.html

目  录
来源：http://hz.nanxuanxn.top/gtsynnxpvy.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtpwwhfetd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.andypj.xyz/gtyfrqgflr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtzzcioxik.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtfoaehker.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ybcxt.top/gteoflbgsr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pengpengdd.cyou/gtjxpaltpw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xziqi.cn/gtfvmkzeyd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtmhdzhyke.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenzaomai.com/gtqqqxqulg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtxbyeaygf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gttkpnnpoq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtjhuoartv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtmvjqlvpz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtwshstzex.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtldzjtwrs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yongpay.top/gtpcuhezbr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtkapqffzv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dianchejie.cn/gtgechsozu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.snrcjt.cn/gtfzdykilu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dashuyun.cn/gtbbbaxhuu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtwothcmtu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtfzcvuqxb.html

================================================================================
来源：http://hz.tian-w.cn/gtpobkdmoh.html

A. 基础语法与类型
来源：http://hz.nanxinkj.top/gtyxkoggyv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqkpasibm.html

[A01] Hello World
来源：http://hz.cqqwz.cn/gtsxmdzixg.html

Py:   print("Hello, World!")
来源：http://hz.vqdsnc.cn/gttdwaeenn.html

PHP:  echo "Hello, World!";
来源：http://hz.andypj.xyz/gtjmhoanzb.html

JS:   console.log("Hello, World!");
来源：http://hz.hammf.cn/gtbrhjryst.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cqqwz.cn/gtplcrqphj.html

Java: System.out.println("Hello, World!");
来源：http://hz.hysaishi.cn/gtkgqdlkxf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydzc1.top/gtbmbwmtnn.html

Ruby: puts "Hello, World!"
来源：http://hz.shzxlz.cn/gthftoanri.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.meibo888.top/gtxkhdqtos.html

[A02] 变量声明与赋值
来源：http://hz.shangyingyoupin.top/gtgigjynat.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtqeiiryud.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fzhhl.top/gtoeizhrdt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.guowangkeji.top/gtsxrynlvp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sweek.top/gtqyvnsfaa.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.nanxinkj.top/gthsojricg.html

Go:   name := "Alex"; age := 20
来源：http://hz.ppjwa.cn/gtlnuvwmol.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sxryk.cn/gthdfscxoy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yj202588.top/gtezwskmvy.html

[A03] 常量定义
来源：http://hz.guannengcc.top/gtkbavctdu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hammf.cn/gtwcbxjezg.html

PHP:  const PI = 3.14159;
来源：http://hz.pycfn.com/gtbgtsmjrv.html

JS:   const PI = 3.14159;
来源：http://hz.jqgfzy.top/gtalidutlx.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtvkkdbjkm.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtddsoblen.html

Go:   const PI = 3.14159
来源：http://hz.cqqwz.cn/gtwmryzsoc.html

Ruby: PI = 3.14159
来源：http://hz.daxiang520.top/gtfoexdiud.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtyyfrwbcc.html

[A04] 判断变量类型
来源：http://hz.chenzaomai.com/gtnmkfbhyu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gzhubu.top/gtzupanarl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.svipenyu.cn/gtlilljgnt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.mhx1999.top/gtsvzlxaas.html

TS:   typeof x; x instanceof Date
来源：http://hz.chenjidiqi.icu/gtagzvibww.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cheryme.top/gtbhrnszze.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhiwuduotai.top/gtadpxinbm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.vqdsnc.cn/gtbodhknrz.html

C#:   x.GetType().Name; x is int
来源：http://hz.xingfuxueyuan.xyz/gtoazpnxur.html

[A05] 整数除法与取模
来源：http://hz.chenlongwang.top/gtlprdwutu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jqgufenzy.top/gtlwvoklqg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.snrcjt.cn/gtubniwxsj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yangfankeji.com/gtrmfcjfov.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yanxiufei.cn/gtxrkyxbxq.html

Java: 7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtanoosmxw.html

Go:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtmdeymbky.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtzaktxyye.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtfhpddgac.html

[A06] 字符串转数字
来源：http://hz.jyoumei.cn/gtrlhmohki.html

Py:   int("42"); float("3.14")
来源：http://hz.havefunace.top/gtwicofzcx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daria6918.cn/gtziscxyyp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ppjwa.cn/gtzwdikhxu.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cucudq.cn/gtvbnyojos.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cqqwz.cn/gtwlwuqpop.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tanke756.top/gtqblcvtxn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yvedp.cn/gtxzseszax.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xylfe.cn/gtmpzetgri.html

[A07] 数字转字符串
来源：http://hz.hammf.cn/gticsphagd.html

Py:   str(42)
来源：http://hz.hongshengwenyu.top/gtibnrdpjo.html

PHP:  (string) 42; strval(42)
来源：http://hz.jianghu66.top/gtrtuveclb.html

JS:   String(42); (42).toString()
来源：http://hz.feifeiyinyue.top/gtsdpsssff.html

TS:   String(42)
来源：http://hz.jiagoushi.top/gthracxioh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.birdmap.top/gtkchjogaa.html

Go:   strconv.Itoa(42)
来源：http://hz.aibaodan.cn/gthlnrvpvt.html

Ruby: 42.to_s
来源：http://hz.pycfn.com/gtwfzrujbi.html

C#:   42.ToString()
来源：http://hz.iojbl.cn/gtbuufvmxb.html

[A08] 取整与四舍五入
来源：http://hz.yongpay.top/gtvjpaqqkl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.pengpengdd.cyou/gtyamhezdu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.snrcjt.cn/gtvhxqakoh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cqqwz.cn/gtriwljsin.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yj202588.top/gtaodedxlo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.c1oappe.top/gtgtbmmgex.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cdnleiting.top/gtguhzlquw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xuanzx.com/gtbkgfzdxa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.smart0.xyz/gtjspqrebd.html

[A09] 绝对值与最大最小值
来源：http://hz.jqgfzy.top/gtwmapfaby.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dianchejie.cn/gtrsjggyat.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ppjwa.cn/gtdoogzxgj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.shangyingyoupin.top/gtgcydbcys.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtbqcgezha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.pycfn.com/gtfudeuuqx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jqgufenzy.top/gtkyuvowix.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.nanxinkj.top/gtzrbqnhsg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yuanzhike.top/gtnhrwqxlj.html

[A10] 生成随机数
来源：http://hz.snrcjt.cn/gtrrkifqrw.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhengqikj.top/gtgsjeqlxe.html

PHP:  random_int(1, 100);
来源：http://hz.bjfxy.top/gtercynmhe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ppjwa.cn/gtriuhxdnk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cucudq.cn/gtrwvglmmw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.pengpengdd.cyou/gtqmdzaxfo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhoulong.xyz/gtowrxdvec.html

Ruby: rand(1..100)
来源：http://hz.bjfxy.top/gtcaxfnano.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinyuanbaomall.cn/gtdbskzxvk.html

[A11] 条件表达式（三元）
来源：http://hz.daxiang520.top/gtwfgxckle.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hammf.cn/gtwiwvufwt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtxdjejqda.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.nanxuanxn.top/gtqkyxveja.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigfzy.top/gtgjbzgxoh.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtzbutviby.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sxryk.cn/gtgmykxhwh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtwftcfuqc.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gttoaagcou.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuanzhike.top/gtfxkiydyl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.nanxuanxn.top/gtjmcnmxsj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhijiandao.cn/gtbpngcolc.html

JS:   `Hello, ${name}!`
来源：http://hz.zhoulong.xyz/gtyvtvzcmh.html

TS:   `Hello, ${name}!`
来源：http://hz.smart0.xyz/gtqyskczuw.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.sufxvd.cn/gtnshuvtwl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.svipenyu.cn/gtwyavkklc.html

Ruby: "Hello, #{name}!"
来源：http://hz.jianghu66.top/gtljgzvfwb.html

C#:   $"Hello, {name}!"
来源：http://hz.tanke756.top/gtpebdulyw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.52xcode.cn/gtovpjsipv.html

Py:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gttpdsfjdr.html

PHP:  "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtboftuluv.html

JS:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtpnmkdine.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtpyuuvgfn.html

Java: "第一行\n第二行"
来源：http://hz.hammf.cn/gtshbinawm.html

Go:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtpzuuanve.html

Ruby: "第一行\n第二行"
来源：http://hz.sxryk.cn/gtiufoxwwh.html

C#:   "第一行\n第二行"
来源：http://hz.yuanzhike.top/gtwalekdsu.html

[A14] 注释写法
来源：http://hz.smart0.xyz/gthafonaix.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jiagoushi.top/gtzozrzsgi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtjfiylduu.html

JS:   // 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtdlykklxx.html

TS:   // 单行；/* 多行 */
来源：http://hz.hysaishi.cn/gtmnxvqzxc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yonumen.top/gtbrrphhxk.html

Go:   // 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtrrwfnvwy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ehwqpu.com/gtomdvjzmi.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtjotigwrw.html

[A15] 空值判断与默认值
来源：http://hz.chenjidiqi.icu/gtuuicykbs.html

Py:   value = data or "默认值"
来源：http://hz.nanxinkj.top/gtnisnsjjg.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtusanntlp.html

JS:   const value = data ?? "默认值";
来源：http://hz.guowangkeji.top/gttgoiyzqz.html

TS:   const value = data ?? "默认值";
来源：http://hz.ywan-chungtsiang.top/gtpbyemoyn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.dianchejie.cn/gtpekoilfc.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.tian-w.cn/gtegsrbpdh.html

Ruby: value = data || "默认值"
来源：http://hz.yongpay.top/gtxubbjcem.html

C#:   var value = data ?? "默认值";
来源：http://hz.jyoumei.cn/gtwbhtfeoo.html

[A16] 真假值判断规则
来源：http://hz.zdqjudy.top/gtrlamyevl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.fzhhl.top/gtefxtbgrt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yangfankeji.com/gtcoitdngw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.0kj1m.cn/gtwssjirbf.html

TS:   if (!x) {}
来源：http://hz.guowangkeji.top/gtjmfdgnws.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.wangdashe.top/gthhwprbnv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.sxryk.cn/gtywtzmyhh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shzxlz.cn/gtoxtizgsq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangshuangyany.cn/gtfcyknryk.html

[A17] 位运算
来源：http://hz.smart0.xyz/gtbokmlspv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gtbibdytmi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinqigufen.top/gtjvzsmjjo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtphfdxpvq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shanyushiyangkeji.top/gtqrojzqqj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gttnufamlu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtuaoymwge.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtamppujjt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtbuonyxud.html

[A18] 字符与 ASCII 码互转
来源：http://hz.hysaishi.cn/gtcycbiqtg.html

Py:   ord("A"); chr(65)
来源：http://hz.tanke756.top/gtljeslicp.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhaomingkeji.xyz/gtmntpwttr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jyoumei.cn/gtfkcphuvv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.aibaodan.cn/gtquunomqn.html

Java: (int) 'A'; (char) 65
来源：http://hz.gzhubu.top/gtavwppdpb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jianghu66.top/gtaltrjulv.html

Ruby: "A".ord; 65.chr
来源：http://hz.yangfankeji.com/gtzfubytst.html


<!-- 参考信息 -->