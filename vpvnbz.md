代发 wailian999

[U105] JS：节流
来源：http://hz.guannengcc.top/gtyzriumxi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtgqwznpfl.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtvhpgfffs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nwbrower.top/gtedealznt.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gtzcuposaz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhiwuduotai.top/gtmicbzabc.html

[U108] JS：随机整数
来源：http://hz.hongshengwenyu.top/gtcnzcwlfg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.chenzaomai.com/gtgacuynff.html

[U109] JS：数组分组
来源：http://hz.aizwys.cn/gttxscewpg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gthqfbyawx.html

[U110] JS：数组分块
来源：http://hz.zdqjudy.top/gtwfflnkel.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jiagoushi.top/gtfzfrpgbq.html

[U111] JS：对象转 Map
来源：http://hz.havefunace.top/gtqpsnbbfd.html

new Map(Object.entries(obj))
来源：http://hz.hammf.cn/gtbqocjeil.html

[U112] JS：字符串补位
来源：http://hz.nanxinkj.top/gtclkwlotg.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtyecomilw.html

[U113] JS：正则替换全部
来源：http://hz.xingfuxueyuan.xyz/gthebbwove.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtxahqlloe.html

[U114] JS：JSON 深比较
来源：http://hz.gzhubu.top/gtyhkcjlyq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtyotqqfcu.html

[U115] JS：生成 UUID
来源：http://hz.tian-w.cn/gtpfrsqoaf.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gthuaymmim.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtsjjxtmzj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ppjwa.cn/gtmarbaypz.html

[U117] JS：单元测试
来源：http://hz.9152youxi.cn/gtydruynua.html

npm i -D vitest;  npx vitest
来源：http://hz.chenzaomai.com/gthohoxfuy.html

[U118] JS：开发服务器
来源：http://hz.9152youxi.cn/gtbvlniazq.html

npm i -D vite;  npx vite
来源：http://hz.tian-w.cn/gtgvkbklqw.html

[U119] JS：生产构建
来源：http://hz.ppjwa.cn/gtopxnuzwg.html

npx vite build
来源：http://hz.aibaodan.cn/gtgaapbvls.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtwylmttly.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtkbbyddmq.html

================================================================================
来源：http://hz.xziqi.cn/gtgwebaruo.html

统计汇总
来源：http://hz.tianlin.xyz/gtvdebiwvl.html

================================================================================
来源：http://hz.smart0.xyz/gtwetwlobc.html

按语言统计（条）：
来源：http://hz.yj20258.top/gtsoimldij.html

Python ......... 252
来源：http://hz.hfpthk.cn/gtiitccinv.html

PHP ............ 252
来源：http://hz.zycfv.cn/gthlzgeuwh.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gthmlwrcxp.html

TypeScript ..... 212
来源：http://hz.chenlongwang.top/gtnryuhztr.html

Java ........... 212
来源：http://hz.nanxuanxn.top/gtiwdidwvk.html

Go ............. 212
来源：http://hz.svipenyu.cn/gtlkhramfm.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtyzdhkxmr.html

C# ............. 212
来源：http://hz.aibaodan.cn/gtfkotlpnp.html

C .............. 30
来源：http://hz.redwolf501.top/gtnxzcfbik.html

C++ ............ 30
来源：http://hz.gzhubu.top/gthrwmrodb.html

SQL ............ 90
来源：http://hz.xinyue.icu/gtnnjuuhxo.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtwqkbmtrq.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtjewsuekr.html

Swift .......... 15
来源：http://hz.pycfn.com/gthllnxirp.html

Lua ............ 10
来源：http://hz.nanxinkj.top/gtxgybcdma.html

Perl ........... 10
来源：http://hz.chenlongwang.top/gteyjowjgd.html

Scala .......... 10
来源：http://hz.yj202588.top/gtvlxvukze.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtyqtqoapt.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtcxnhzpgu.html

按章节统计：
来源：http://hz.svipenyu.cn/gtwrbudnjt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinyuanbaomall.cn/gtrzgabgvt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtrftdizqe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtglqqbeut.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtuguxfrqz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yangfankeji.com/gtyyrvnunm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtxnfihopc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtymnwlfqe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtxdpxgxor.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtbrjodqwq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtfhjqczhn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtloucxppa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gttyhmksfs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gthtjviita.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtxqmpohhw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gtiluoyvvv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtygscjfdm.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gtnnufryug.html

R Bash 专题                             80
来源：http://hz.andypj.xyz/gtajcfrjlb.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtqqordcfp.html

T 其他语言补充                          60
来源：http://hz.svipenyu.cn/gtubnpwkps.html

U 高频实用片段                         120
来源：http://hz.snrcjt.cn/gtugvoetig.html

------------------------------------
来源：http://hz.vqdsnc.cn/gtklvgowwj.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtzzlwigfc.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtyrxywhdf.html

使用提醒
来源：http://hz.vqdsnc.cn/gtamrxjmkb.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gthmcbbnio.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zycfv.cn/gtxjlnfkjc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.vqdsnc.cn/gtybmukzkz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cucudq.cn/gtypajivkk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenzaomai.com/gtafstgtmh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shangyingyoupin.top/gtmeinbunz.html

—— 文件结束 ——
来源：http://hz.gzhubu.top/gtgcngbcqx.html

================================================================================
来源：http://hz.tianlin.xyz/gtiijtjcdq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tanke756.top/gtqztnxkzb.html

Common Programming Examples Cheat Book
来源：http://hz.jyoumei.cn/gtqmycwrpc.html

================================================================================
来源：http://hz.0kj1m.cn/gtohvdoyyn.html

【收录内容】
来源：http://hz.9152youxi.cn/gtsmrywbuo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hammf.cn/gtdhzlaqfs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yangfankeji.com/gtimmjizwh.html

SQL · Bash · C · C++
来源：http://hz.wangdashe.top/gtfsozbzed.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.havefunace.top/gtciesgxgb.html

【使用说明】
来源：http://hz.9152youxi.cn/gtbneohely.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xziqi.cn/gtjsuypiey.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.havefunace.top/gtlcsbxzwy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.vqdsnc.cn/gtoouzezrl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cashguo.top/gtpcysmcbc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yanxiufei.cn/gtedzfjzqx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jqgufenzy.top/gtrvpgiszg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ybcxt.top/gtsjqqmhhi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hnqzz.top/gtumfienlt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xuetiantiany.cn/gtotqhxmnt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cheryme.top/gtutgurnud.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtkrekypeb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.kuanghao11.cn/gtjczifbsv.html

【文件统计】
来源：http://hz.0kj1m.cn/gtftsykpxy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hywenlv.cn/gtvrpwfnab.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtltbgcjvt.html

目  录
来源：http://hz.wangshuangyany.cn/gtqzqwlgot.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtxwyejmaw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtpfoxovwx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtsbhwoycr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtpnpahosn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtrzncruda.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.meibo888.top/gtzpnmcarw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ywan-chungtsiang.top/gtimaukgnl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtdqrqrbgk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtcfkhxiyd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtjqiqkvqq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gtmwoufxir.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtwmfmxddp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtcrnfhqyj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtizsclavz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtodagqvcd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xingfuxueyuan.xyz/gtpjezuoid.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtquqdszcx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtbsjejpiw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangtech.top/gtkadxjhzk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.daria6918.cn/gtrcrjobsv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtabhdmwnb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zycfv.cn/gtakumolpb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmylksdyk.html

A. 基础语法与类型
来源：http://hz.tanke756.top/gtngotaxly.html

================================================================================
来源：http://hz.shuidangran.top/gtdhvmeotx.html

[A01] Hello World
来源：http://hz.wangshuangyany.cn/gtbxooqxoc.html

Py:   print("Hello, World!")
来源：http://hz.birdmap.top/gtriicrgip.html

PHP:  echo "Hello, World!";
来源：http://hz.ivvv.top/gtzkwudnjm.html

JS:   console.log("Hello, World!");
来源：http://hz.gogol.net.cn/gtyzqvtyaa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jlsjyb.cn/gtfbcaexco.html

Java: System.out.println("Hello, World!");
来源：http://hz.ppjwa.cn/gtfsnjtmji.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtmjenwwdf.html

Ruby: puts "Hello, World!"
来源：http://hz.chenjidiqi.icu/gthzemvyga.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhoulong.xyz/gtkrjfxinm.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtnggtvbmb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zdqjudy.top/gtrddynbnv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.guowangkeji.top/gtdhonwqyz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.fzhhl.top/gtwwnnulsc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yangfankeji.com/gtvivkdoag.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.9152youxi.cn/gtwofzneyt.html

Go:   name := "Alex"; age := 20
来源：http://hz.aibaodan.cn/gtokeiajby.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cheryme.top/gtyuhanvlm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtriwttizx.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtupmrtswe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.kuanghao11.cn/gtipehuckd.html

PHP:  const PI = 3.14159;
来源：http://hz.sysykeji.top/gtwfujkpwv.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gtsevqkfxu.html

TS:   const PI: number = 3.14159;
来源：http://hz.mhx1999.top/gtetdyfbku.html

Java: static final double PI = 3.14159;
来源：http://hz.xziqi.cn/gtwapbxcbw.html

Go:   const PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtsnojhmmx.html

Ruby: PI = 3.14159
来源：http://hz.xuanzx.com/gtpunucmet.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtjcqielzj.html

[A04] 判断变量类型
来源：http://hz.bjfxy.top/gtlwoygjyy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yj20258.top/gtrixrupyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xuetiantiany.cn/gttctclvld.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangshuangyany.cn/gtkstdbnkq.html

TS:   typeof x; x instanceof Date
来源：http://hz.sufxvd.cn/gtwmnapvxz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daxiang520.top/gtoggkjsmh.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnxiangtu.top/gtsejwyswf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhiwuduotai.top/gthpdeeuqb.html

C#:   x.GetType().Name; x is int
来源：http://hz.yuxming.cn/gtrdfgvsve.html

[A05] 整数除法与取模
来源：http://hz.9152youxi.cn/gtgbnbtjdk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.guowangkeji.top/gtcxclxpvs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aizwys.cn/gtewwpwwmv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yonumen.top/gtcnibnbvl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtupjpjkpx.html

Java: 7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtcbvgybsj.html

Go:   7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gthhlltieu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtngxczaue.html

C#:   7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtvbnuiylz.html

[A06] 字符串转数字
来源：http://hz.ybcxt.top/gtjhmeruru.html

Py:   int("42"); float("3.14")
来源：http://hz.nanxuanxn.top/gtvqqmfmvd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.guowangkeji.top/gtwumrtzgx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shzxlz.cn/gtvfximtiz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.chenzaomai.com/gthddcmwit.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jyoumei.cn/gtqiuoymhu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.aibaodan.cn/gtclwprxig.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.wangshuangyany.cn/gtkrnnbyll.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtiznsteiq.html

[A07] 数字转字符串
来源：http://hz.shangyingyoupin.top/gtvpudghoa.html

Py:   str(42)
来源：http://hz.birdmap.top/gtihcmovpy.html

PHP:  (string) 42; strval(42)
来源：http://hz.jqgfzy.top/gtadnfzvaq.html

JS:   String(42); (42).toString()
来源：http://hz.sweek.top/gtfdrqfwni.html

TS:   String(42)
来源：http://hz.svipenyu.cn/gtrtoogbgs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.aibaodan.cn/gtabumvfhn.html

Go:   strconv.Itoa(42)
来源：http://hz.jyoumei.cn/gtimwopqjp.html

Ruby: 42.to_s
来源：http://hz.0kj1m.cn/gtdcjmuloq.html

C#:   42.ToString()
来源：http://hz.tian-w.cn/gteeoaahrz.html

[A08] 取整与四舍五入
来源：http://hz.jinghuilouyu.cn/gtiqxilfwu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nanxinkj.top/gtinhrwoty.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.nanxinkj.top/gtjokdilim.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhaomingkeji.xyz/gtsrojnsad.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigufen.top/gtnzleyfao.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gtpjyckjhd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.andypj.xyz/gtcsqyellh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ivvv.top/gtzfevxvvm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj20258888.top/gtxrwanzll.html

[A09] 绝对值与最大最小值
来源：http://hz.gzhubu.top/gtvzkptjqq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtnryyoulu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guowangkeji.top/gteectavyz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.aibaodan.cn/gtswxkrnks.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.smart0.xyz/gtyhnuglmq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.0kj1m.cn/gtjjmdhznd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.0kj1m.cn/gtmspxgxvp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhiwuduotai.top/gtgqmmbdqm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.redwolf501.top/gtdiocnosc.html

[A10] 生成随机数
来源：http://hz.chenlongwang.top/gtgtylyvjh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.pengpengdd.cyou/gtefjamitk.html

PHP:  random_int(1, 100);
来源：http://hz.tanke756.top/gtspfvctcg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.feifeiyinyue.top/gtqptvwjie.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ydzc1.top/gtzyjrvilw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.tian-w.cn/gtvjlqdkam.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jianghu66.top/gtsifkaior.html

Ruby: rand(1..100)
来源：http://hz.hammf.cn/gtxzcdftyn.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj202588.top/gtbjnugmec.html

[A11] 条件表达式（三元）
来源：http://hz.ydjk.org.cn/gtfxdjwqwg.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtworkndzi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtnpzrnqng.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgfzy.top/gtuaopmkqq.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtruzxmxav.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtjyuttiuq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yonumen.top/gthjuyyvmi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtydyvgmhz.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.dashuyun.cn/gtpasqkdnz.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuanzhike.top/gtifbajvat.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.pengpengdd.cyou/gtcwkkospi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tian-w.cn/gtrbkhrocm.html

JS:   `Hello, ${name}!`
来源：http://hz.zhixingplan.top/gtryilaysc.html

TS:   `Hello, ${name}!`
来源：http://hz.ydjk.org.cn/gtkneadmnf.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhoulong.xyz/gtvuiccoks.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.shuidangran.top/gthvfhnbkt.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenjidiqi.icu/gtajhiqwln.html

C#:   $"Hello, {name}!"
来源：http://hz.fengsongda.top/gthxdadmjm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yj202588.top/gtynpgtwqz.html

Py:   "第一行\n第二行"
来源：http://hz.svipenyu.cn/gtczmstoja.html

PHP:  "第一行\n第二行"
来源：http://hz.zhiwuduotai.top/gtqpgnqwyd.html

JS:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtadcmejez.html

TS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtfimcnlon.html

Java: "第一行\n第二行"
来源：http://hz.mhx1999.top/gtgzeyxsnf.html

Go:   "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtpqrpxkga.html

Ruby: "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtxfmfddcf.html

C#:   "第一行\n第二行"
来源：http://hz.sweek.top/gtpixaasgu.html

[A14] 注释写法
来源：http://hz.chenlongwang.top/gtwtqbaekr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.meibo888.top/gtnfopashh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.iojbl.cn/gtdvczizlp.html

JS:   // 单行；/* 多行 */
来源：http://hz.wangdashe.top/gtknrnyeki.html

TS:   // 单行；/* 多行 */
来源：http://hz.yonumen.top/gtibrjoftm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.birdmap.top/gtupskaepo.html

Go:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtimfspnca.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.birdmap.top/gtmtdxomsf.html

C#:   // 单行；/* 多行 */
来源：http://hz.vqdsnc.cn/gtlgrrmdkq.html

[A15] 空值判断与默认值
来源：http://hz.gaohongyu789.top/gtcrihznsy.html

Py:   value = data or "默认值"
来源：http://hz.jinqigufen.top/gtmrbcdtpd.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ybcxt.top/gtqbcpjzdl.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtbtizqtwd.html

TS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtahhvyzzf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.daxiang520.top/gtxopcoiqi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cdnleiting.top/gtgjcvtchy.html

Ruby: value = data || "默认值"
来源：http://hz.ivvv.top/gtjqltugto.html

C#:   var value = data ?? "默认值";
来源：http://hz.chenjidiqi.icu/gtiraffbhj.html

[A16] 真假值判断规则
来源：http://hz.sysykeji.top/gtnybkihhg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.tianlin.xyz/gtvwgeitwm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.vqdsnc.cn/gttzemcobi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.svipenyu.cn/gtyiicgbsx.html

TS:   if (!x) {}
来源：http://hz.kuanghao11.cn/gthjyyrumv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yuanzhike.top/gtauccwkwt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.wangdashe.top/gtklxkivxv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.aibaodan.cn/gtqimoxyov.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhijiandao.cn/gtjajgvdxr.html

[A17] 位运算
来源：http://hz.zhijiandao.cn/gtckzejbfi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtfsdkzqsw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.quarkkingdee.top/gtmmdhqdyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sxryk.cn/gtcstykjbz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtajehmqqk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtcavgzisc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtkottkopp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtzbqkgcuq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtujavzrph.html

[A18] 字符与 ASCII 码互转
来源：http://hz.cheryme.top/gtycaptpkg.html

Py:   ord("A"); chr(65)
来源：http://hz.fzhhl.top/gttxlzbgtm.html

PHP:  ord("A"); chr(65)
来源：http://hz.sufxvd.cn/gtfgjymqyd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gogol.net.cn/gtcwrunome.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fzhhl.top/gtepicyewy.html

Java: (int) 'A'; (char) 65
来源：http://hz.cheryme.top/gtyhmisbri.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xingfuxueyuan.xyz/gtoglqqyzr.html

Ruby: "A".ord; 65.chr
来源：http://hz.0kj1m.cn/gtazoswfgq.html


<!-- 参考信息 -->