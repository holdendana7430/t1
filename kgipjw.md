代发 wailian999

[U103] JS：定时器
来源：http://hz.quarkkingdee.top/gtbnxhjbts.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuetiantiany.cn/gtakduylju.html

[U104] JS：防抖
来源：http://hz.xingfuxueyuan.xyz/gtviwfvtnl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtbasauxeh.html

[U105] JS：节流
来源：http://hz.guannengcc.top/gttppikhsx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtralkjshc.html

[U106] JS：日期格式化
来源：http://hz.zhengqikj.top/gtmgmukhnv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangshuangyany.cn/gtagaxerpt.html

[U107] JS：数字千分位
来源：http://hz.hnxiangtu.top/gtsoksphuw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgfzy.top/gtabqogalb.html

[U108] JS：随机整数
来源：http://hz.haohaochexian.top/gtxlhhykfp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ppjwa.cn/gtytauenwi.html

[U109] JS：数组分组
来源：http://hz.guannengcc.top/gtqdxzihiw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gteqltodca.html

[U110] JS：数组分块
来源：http://hz.snrcjt.cn/gtxhzthjnn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtmldkymmg.html

[U111] JS：对象转 Map
来源：http://hz.ydjk.org.cn/gtstcbcsmt.html

new Map(Object.entries(obj))
来源：http://hz.cqqwz.cn/gtrlkvbyss.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gtlbchuczj.html

"7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtfywqztfb.html

[U113] JS：正则替换全部
来源：http://hz.jinyuanbaomall.cn/gtswtwbnlh.html

s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtiqlqpavh.html

[U114] JS：JSON 深比较
来源：http://hz.sweek.top/gtoyxhfjld.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtdrjrovbe.html

[U115] JS：生成 UUID
来源：http://hz.zhoulong.xyz/gtvrdhfeix.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtitjfwcuh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtegyglury.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jyoumei.cn/gtenmifgmt.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gtlljgttms.html

npm i -D vitest;  npx vitest
来源：http://hz.yj202588.top/gtuypivjgg.html

[U118] JS：开发服务器
来源：http://hz.gaohongyu789.top/gtmoyhzljy.html

npm i -D vite;  npx vite
来源：http://hz.chenjidiqi.icu/gtmdbhkynj.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtxdzjyikh.html

npx vite build
来源：http://hz.hywenlv.cn/gtkrynpmts.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yanxiufei.cn/gtqcepljmd.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258888.top/gtdbdpnztq.html

================================================================================
来源：http://hz.jyoumei.cn/gtmodiydfs.html

统计汇总
来源：http://hz.jinyuanbaomall.cn/gtflcelrut.html

================================================================================
来源：http://hz.mhx1999.top/gtlstxvthn.html

按语言统计（条）：
来源：http://hz.sufxvd.cn/gtawmruglf.html

Python ......... 252
来源：http://hz.cheryme.top/gtvybddlrb.html

PHP ............ 252
来源：http://hz.zhaomingkeji.xyz/gtqweacbnq.html

JavaScript ..... 252
来源：http://hz.zdqjudy.top/gtqxxczrml.html

TypeScript ..... 212
来源：http://hz.dashuyun.cn/gtqanogkwv.html

Java ........... 212
来源：http://hz.nanxinkj.top/gtiroivdgp.html

Go ............. 212
来源：http://hz.zhengqikj.top/gtemmfzmyn.html

Ruby ........... 212
来源：http://hz.hammf.cn/gtaklcktsa.html

C# ............. 212
来源：http://hz.yj20258.top/gtjdlopeuk.html

C .............. 30
来源：http://hz.cqqwz.cn/gtuvjlqjvc.html

C++ ............ 30
来源：http://hz.316326.xyz/gtouyacxnd.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gttrzanyux.html

Bash ........... 80
来源：http://hz.kuanghao11.cn/gteqppsxtr.html

Kotlin ......... 15
来源：http://hz.yongpay.top/gtdxtovhib.html

Swift .......... 15
来源：http://hz.havefunace.top/gteekuugwr.html

Lua ............ 10
来源：http://hz.ivvv.top/gtdmtnvfxa.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtgqahfcmx.html

Scala .......... 10
来源：http://hz.cheryme.top/gtmusuekye.html

------------------------------------
来源：http://hz.daria6918.cn/gtnirhxohl.html

合计 ........... 2106 条
来源：http://hz.aibaodan.cn/gtkfjloqjk.html

按章节统计：
来源：http://hz.aizwys.cn/gtyovdahdv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtmeafngij.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtjnsqgbeg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtuqraxxwx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtofepngxf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhoulong.xyz/gtfjnljuvw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtwiulvjft.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtbprkxhmx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gthgsllvvo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtukqpccpu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtovlnqlwf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtstuewvxo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtkpeuifwk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtlatiopgn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtshotxbql.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxuanxn.top/gtfrqpiabs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtdsdzmmzc.html

Q SQL 专题                              90
来源：http://hz.yueranfly.top/gteybaktfy.html

R Bash 专题                             80
来源：http://hz.ydzc1.top/gtaigrnubf.html

S C / C++ 专题                          60
来源：http://hz.gotoacloud.top/gtgggpqxxq.html

T 其他语言补充                          60
来源：http://hz.shzxlz.cn/gtbpyzeekk.html

U 高频实用片段                         120
来源：http://hz.yvedp.cn/gtycuazopb.html

------------------------------------
来源：http://hz.gogol.net.cn/gtvsssabhu.html

合计                                  2106 条
来源：http://hz.ppjwa.cn/gtsnyexnti.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gtegdcxtor.html

使用提醒
来源：http://hz.9152youxi.cn/gtukwkbjpp.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtedhqqllh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.c1oappe.top/gtikzmdkmj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shzxlz.cn/gtwsdjnfrv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.guowangkeji.top/gtmochrreb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gogol.net.cn/gtnghuacbq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.pengpengdd.cyou/gtivedebxg.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtlgoocuah.html

================================================================================
来源：http://hz.fzhhl.top/gtksfukeet.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hnqzz.top/gtzzuckhab.html

Common Programming Examples Cheat Book
来源：http://hz.fzhhl.top/gtxgfvbsoh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlduefiib.html

【收录内容】
来源：http://hz.chenlongwang.top/gtqeukhxcx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yonumen.top/gtzjqkkwlx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhoulong.xyz/gtqjcitvfx.html

SQL · Bash · C · C++
来源：http://hz.gotoacloud.top/gtsdervcij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangdashe.top/gtedncator.html

【使用说明】
来源：http://hz.ivvv.top/gtzdozvgzn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shzxlz.cn/gtkjtkcwnp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xinyue.icu/gtpuwayatt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhongyouzk.top/gtjfhrxfkq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.smart0.xyz/gteyyypjga.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shangyingyoupin.top/gtrstrgtwb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.vqdsnc.cn/gtbaiarnni.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenzaomai.com/gtudrbwssn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shangyingyoupin.top/gtxgxmwjhc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtxgaevjeh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.c1oappe.top/gtecvfdjkm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ppjwa.cn/gtgzceqirh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhiwuduotai.top/gtqvbpiguz.html

【文件统计】
来源：http://hz.meibo888.top/gttrrtyrbs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sxryk.cn/gtnukdjvgu.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtlnlxoucj.html

目  录
来源：http://hz.zhijiandao.cn/gtgzasyxug.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gttsuphyjt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yuanzhike.top/gtqgylhhiv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtqlvactge.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtvftsiwlh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cheryme.top/gtmwsiiiue.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ivvv.top/gtgpcujlqm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtlotzjyum.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtnxdcfyrs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtqltzipip.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtjaztchct.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhaomingkeji.xyz/gtcnrhamjx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtpzujpgfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtmvikdoqp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtfzmbldjp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jinghuilouyu.cn/gtewkgsrwe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pycfn.com/gtzerldlrw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtqmcrutsn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.andypj.xyz/gtuhnsxozr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxinkj.top/gtrjxhmdam.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xuetiantiany.cn/gthmrrvbzp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtbqhjnekv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtnhexzlct.html

================================================================================
来源：http://hz.yueranfly.top/gtsismleie.html

A. 基础语法与类型
来源：http://hz.zhongyouzk.top/gtqycgzuqb.html

================================================================================
来源：http://hz.shzxlz.cn/gtjlbksape.html

[A01] Hello World
来源：http://hz.quarkkingdee.top/gtzdgqcxip.html

Py:   print("Hello, World!")
来源：http://hz.jqgfzy.top/gtrmrggvyk.html

PHP:  echo "Hello, World!";
来源：http://hz.yueranfly.top/gtlhtprhpv.html

JS:   console.log("Hello, World!");
来源：http://hz.jyoumei.cn/gtjgmblxlu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guowangkeji.top/gtjxxptwrn.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gtdwmclfho.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.guowangkeji.top/gtofwsqevr.html

Ruby: puts "Hello, World!"
来源：http://hz.nanxinkj.top/gtywyxhucx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.kuanghao11.cn/gthgtncpyt.html

[A02] 变量声明与赋值
来源：http://hz.wangshuangyany.cn/gtjzqggibl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hfpthk.cn/gtsjtzlmpb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aizwys.cn/gtidaanwdt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sxryk.cn/gthnmahvnp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.havefunace.top/gtdrihoous.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtxuowsrwk.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgufenzy.top/gtceazrsqm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jyoumei.cn/gtcazgxmon.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.mhx1999.top/gtiefluwdn.html

[A03] 常量定义
来源：http://hz.shanyushiyangtech.top/gtmwzxhmhy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.bjfxy.top/gtbvconogs.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258888.top/gtwgwpipoa.html

JS:   const PI = 3.14159;
来源：http://hz.zhengqikj.top/gtlounrfmw.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtenebkmum.html

Java: static final double PI = 3.14159;
来源：http://hz.meibo888.top/gtqjwfrjqd.html

Go:   const PI = 3.14159
来源：http://hz.daria6918.cn/gtcvlrbcld.html

Ruby: PI = 3.14159
来源：http://hz.yj20258.top/gtchzcaeal.html

C#:   const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtjflnnehd.html

[A04] 判断变量类型
来源：http://hz.shanyushiyangkeji.top/gteztcansb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.smart0.xyz/gtexelslio.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shangyingyoupin.top/gtbeqeukkw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangkeji.top/gtgfhbvpsw.html

TS:   typeof x; x instanceof Date
来源：http://hz.pengpengdd.cyou/gtfcgzzauv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cashguo.top/gtavuyizso.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yangfankeji.com/gtpfzbyshx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.pengpengdd.cyou/gttkgwkxpz.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtqujtipvq.html

[A05] 整数除法与取模
来源：http://hz.hnxiangtu.top/gtatpqxiud.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj20258.top/gtcpcxsnsq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.meibo888.top/gtblwiezbe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtplgedhzz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtcrxijply.html

Java: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtljomnigt.html

Go:   7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtsvbybley.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtkaxoodnh.html

C#:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtzbfsltuz.html

[A06] 字符串转数字
来源：http://hz.chenjidiqi.icu/gtxhbkmikr.html

Py:   int("42"); float("3.14")
来源：http://hz.hnxiangtu.top/gtckkcyxxt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daxiang520.top/gtzcmiiudm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.haohaochexian.top/gtmsrcdzeq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jyoumei.cn/gtbubjnrmt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cashguo.top/gtuplbtnsx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gotoacloud.top/gtadlarjbp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.cdnleiting.top/gtusgxzkof.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.bjfxy.top/gtyounybsb.html

[A07] 数字转字符串
来源：http://hz.tianlin.xyz/gtolysqtbp.html

Py:   str(42)
来源：http://hz.jqgfzy.top/gtpgnqhgtb.html

PHP:  (string) 42; strval(42)
来源：http://hz.hfpthk.cn/gttnmunfev.html

JS:   String(42); (42).toString()
来源：http://hz.dianchejie.cn/gtntdyxujv.html

TS:   String(42)
来源：http://hz.jqgfzy.top/gthjyqynhj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tian-w.cn/gttygtyrsq.html

Go:   strconv.Itoa(42)
来源：http://hz.hongshengwenyu.top/gtwijbeqyz.html

Ruby: 42.to_s
来源：http://hz.9152youxi.cn/gthuhsdjyg.html

C#:   42.ToString()
来源：http://hz.316326.xyz/gtncxdrejc.html

[A08] 取整与四舍五入
来源：http://hz.kuanghao11.cn/gtidxbkcra.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.0kj1m.cn/gtmcyhppuw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.sxryk.cn/gtqsdwelsm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhixingplan.top/gtbitfjrfy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhoulong.xyz/gtqsfujjjq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.wangdashe.top/gtwdvlkzmb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xinyue.icu/gtyuhhsdlj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.birdmap.top/gtysdsjetv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yueranfly.top/gtyqvvqguo.html

[A09] 绝对值与最大最小值
来源：http://hz.yj20258.top/gtavywsdkt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dashuyun.cn/gtdrilnsnj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuanzhike.top/gtudeqxelo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jiagoushi.top/gtxgpbcvhq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cheryme.top/gtctxmbcha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.vqdsnc.cn/gtpqoonqsw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhengqikj.top/gtlomzoaqf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhaomingkeji.xyz/gtnigrdbhc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shzxlz.cn/gtixojypep.html

[A10] 生成随机数
来源：http://hz.fzhhl.top/gthgasblul.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yueranfly.top/gttgxpovwg.html

PHP:  random_int(1, 100);
来源：http://hz.smart0.xyz/gtctszupug.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ywan-chungtsiang.top/gthhvbslud.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhiwuduotai.top/gtczyvoyme.html

Java: new Random().nextInt(100) + 1
来源：http://hz.guowangkeji.top/gtpnqmmamm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jlsjyb.cn/gtyoltitnn.html

Ruby: rand(1..100)
来源：http://hz.guannengcc.top/gtbdmoldhe.html

C#:   new Random().Next(1, 101)
来源：http://hz.sweek.top/gtrtwjfzjr.html

[A11] 条件表达式（三元）
来源：http://hz.tanke756.top/gtqcljjvev.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aizwys.cn/gtxgzgivvl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtsovwpwej.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gthjqijefx.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtdnzgduvx.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtcagxbdxx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.redwolf501.top/gtukpqctdn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtrjuvhbbj.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtjndobrnq.html

[A12] 字符串插值 / 格式化
来源：http://hz.gogol.net.cn/gtuftlqnlg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hongshengwenyu.top/gtxatyzspw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.daria6918.cn/gtdtbhxlex.html

JS:   `Hello, ${name}!`
来源：http://hz.yuxming.cn/gtrrrbfneu.html

TS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtpwrnvnph.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.fengsongda.top/gtngjzyfqg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.kuanghao11.cn/gtnzflwhic.html

Ruby: "Hello, #{name}!"
来源：http://hz.shuidangran.top/gtokatbbwq.html

C#:   $"Hello, {name}!"
来源：http://hz.ywan-chungtsiang.top/gtbxngafyf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xziqi.cn/gtgvecyfbi.html

Py:   "第一行\n第二行"
来源：http://hz.andypj.xyz/gtdollkkox.html

PHP:  "第一行\n第二行"
来源：http://hz.andypj.xyz/gtkjanehye.html

JS:   "第一行\n第二行"
来源：http://hz.feifeiyinyue.top/gtrgnecnnk.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtofxgqtlu.html

Java: "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtfrjrxctn.html

Go:   "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtvxmlsuhe.html

Ruby: "第一行\n第二行"
来源：http://hz.zhiwuduotai.top/gtrobdyghi.html

C#:   "第一行\n第二行"
来源：http://hz.zhengqikj.top/gtribdphgc.html

[A14] 注释写法
来源：http://hz.yj20258.top/gtvjcfwwaf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yonumen.top/gtwpibusxe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtzgbsgvzq.html

JS:   // 单行；/* 多行 */
来源：http://hz.xinyue.icu/gtgbxfkctt.html

TS:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gturlhktaj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hammf.cn/gtqyygyxda.html

Go:   // 单行；/* 多行 */
来源：http://hz.hysaishi.cn/gtyxkbzhbk.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.wangshuangyany.cn/gtdpouxtyo.html

C#:   // 单行；/* 多行 */
来源：http://hz.jyoumei.cn/gtccpzokjh.html

[A15] 空值判断与默认值
来源：http://hz.cashguo.top/gtqokuocbz.html

Py:   value = data or "默认值"
来源：http://hz.hfpthk.cn/gtiurbytpx.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ywan-chungtsiang.top/gthxnlgyoi.html

JS:   const value = data ?? "默认值";
来源：http://hz.yj20258888.top/gtepoxevcw.html

TS:   const value = data ?? "默认值";
来源：http://hz.yj20258.top/gtbfnbglqx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhiwuduotai.top/gtkzjlmmza.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ppjwa.cn/gtvpqchzjo.html

Ruby: value = data || "默认值"
来源：http://hz.xuetiantiany.cn/gteidmsjus.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhixingplan.top/gtlanvmeua.html

[A16] 真假值判断规则
来源：http://hz.svipenyu.cn/gtnbfpklyo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.0kj1m.cn/gtbocswkbl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.fzhhl.top/gtczycycno.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.birdmap.top/gtpwetkvnz.html

TS:   if (!x) {}
来源：http://hz.xuanzx.com/gtacyqxvpl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.birdmap.top/gtjsjbtoaw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.mhx1999.top/gthtifzjaw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yonumen.top/gtppmvafgr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.0kj1m.cn/gtgwcsbmgt.html

[A17] 位运算
来源：http://hz.yvedp.cn/gtyrjgundr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtdhizjewb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gthulkacur.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.daxiang520.top/gtyldhejpw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtfrlqzqlw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtoceqrjzu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gthttfucho.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtmicdkbjm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtagsdcmjh.html

[A18] 字符与 ASCII 码互转
来源：http://hz.hammf.cn/gtdaojiouo.html

Py:   ord("A"); chr(65)
来源：http://hz.fzhhl.top/gtcmdcaotn.html

PHP:  ord("A"); chr(65)
来源：http://hz.chenzaomai.com/gtlkliezys.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hnxiangtu.top/gtlmlkjtoh.html


<!-- 参考信息 -->