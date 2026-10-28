代发 wailian999

[U103] JS：定时器
来源：http://hz.yangfankeji.com/gtltipdrqx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtmcevdzgm.html

[U104] JS：防抖
来源：http://hz.yuanzhike.top/gtyvelteve.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gthgdbbzgi.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gttelrcemf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cdnleiting.top/gtzamgljvx.html

[U106] JS：日期格式化
来源：http://hz.zhaomingkeji.xyz/gtxrrchcoh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhijiandao.cn/gtpypklsru.html

[U107] JS：数字千分位
来源：http://hz.feifeiyinyue.top/gtwyovtsvg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shuidangran.top/gturmixksy.html

[U108] JS：随机整数
来源：http://hz.yuxming.cn/gtmbsltsot.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhengqikj.top/gtpwrfhdnf.html

[U109] JS：数组分组
来源：http://hz.jqgfzy.top/gtaiewnwcy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtbtczbupw.html

[U110] JS：数组分块
来源：http://hz.havefunace.top/gtxoweshxi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhixingplan.top/gtbdnsdsco.html

[U111] JS：对象转 Map
来源：http://hz.cashguo.top/gtbjsbdlca.html

new Map(Object.entries(obj))
来源：http://hz.jinqigfzy.top/gtzayrtpdf.html

[U112] JS：字符串补位
来源：http://hz.svipenyu.cn/gtgaizadgr.html

"7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtwvksewak.html

[U113] JS：正则替换全部
来源：http://hz.guannengcc.top/gtlqufaxhj.html

s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtrruuphta.html

[U114] JS：JSON 深比较
来源：http://hz.nwbrower.top/gtubvoskkb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtprjeafeb.html

[U115] JS：生成 UUID
来源：http://hz.hysaishi.cn/gtvxsfpatt.html

crypto.randomUUID()
来源：http://hz.cashguo.top/gthlbiugrv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtiqfyyldy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydzc1.top/gteoswsivn.html

[U117] JS：单元测试
来源：http://hz.andypj.xyz/gtrchwxblb.html

npm i -D vitest;  npx vitest
来源：http://hz.cdnleiting.top/gtynoiofex.html

[U118] JS：开发服务器
来源：http://hz.ivvv.top/gtsdagfgls.html

npm i -D vite;  npx vite
来源：http://hz.bjfxy.top/gtdcmjppwg.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gteivsexfs.html

npx vite build
来源：http://hz.guowangkeji.top/gtipebhhuc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.meibo888.top/gtkyimjkib.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgfzy.top/gtwmlwhcae.html

================================================================================
来源：http://hz.gzhubu.top/gtrsiniymr.html

统计汇总
来源：http://hz.jinqigufen.top/gtajqbsfrs.html

================================================================================
来源：http://hz.yonumen.top/gtzrfjrxov.html

按语言统计（条）：
来源：http://hz.gzhubu.top/gtntjcqamt.html

Python ......... 252
来源：http://hz.cashguo.top/gtlvlyitms.html

PHP ............ 252
来源：http://hz.zycfv.cn/gteuvpqkry.html

JavaScript ..... 252
来源：http://hz.xingfuxueyuan.xyz/gttslyfcxf.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gttlwalinp.html

Java ........... 212
来源：http://hz.chenlongwang.top/gtsyigazql.html

Go ............. 212
来源：http://hz.sweek.top/gtlniwtyjf.html

Ruby ........... 212
来源：http://hz.fengsongda.top/gtwyvljlnx.html

C# ............. 212
来源：http://hz.jianghu66.top/gtvneijbol.html

C .............. 30
来源：http://hz.xylfe.cn/gtvinoyflj.html

C++ ............ 30
来源：http://hz.hfpthk.cn/gtuftkrcwj.html

SQL ............ 90
来源：http://hz.zhiwuduotai.top/gtluutxzam.html

Bash ........... 80
来源：http://hz.meibo888.top/gtyxyxetvs.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gticajppnd.html

Swift .......... 15
来源：http://hz.gogol.net.cn/gtoahgffca.html

Lua ............ 10
来源：http://hz.daxiang520.top/gtmzeaebqk.html

Perl ........... 10
来源：http://hz.jinqigfzy.top/gtrecihrmb.html

Scala .......... 10
来源：http://hz.cdnleiting.top/gtepaydprx.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtvcchkyzb.html

合计 ........... 2106 条
来源：http://hz.zhaomingkeji.xyz/gtdbldjwca.html

按章节统计：
来源：http://hz.zhijiandao.cn/gtfzrohodq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtenexodcf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtdrrehydr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtceuuhthn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtstpxqdro.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jyoumei.cn/gtybeeczew.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtquhxpezd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtsfymgmgd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.316326.xyz/gtpecbyldi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtrymguajh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtwurnonqb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtqxkaukbu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtplqfvfyx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtlspenwjj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtkghbansx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guannengcc.top/gtsytrulkd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtdftjpdfa.html

Q SQL 专题                              90
来源：http://hz.wangdashe.top/gtoszrsspf.html

R Bash 专题                             80
来源：http://hz.yongpay.top/gtxiqtysvt.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtrkszbjmg.html

T 其他语言补充                          60
来源：http://hz.jinghuilouyu.cn/gtkoifidqh.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gtzakjanoa.html

------------------------------------
来源：http://hz.guowangkeji.top/gtsmxzjfao.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtqlkzaica.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtctjbbjyt.html

使用提醒
来源：http://hz.xingfuxueyuan.xyz/gtwuzuyavi.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtfzqthcrr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuanzhike.top/gtzyatnxan.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xinyue.icu/gtymqwteuo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.52xcode.cn/gtskxwubal.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hywenlv.cn/gtkmbqgkcl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.smart0.xyz/gtijgdcwlh.html

—— 文件结束 ——
来源：http://hz.ivvv.top/gtzngpsaet.html

================================================================================
来源：http://hz.ybcxt.top/gtipfmvqac.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yanxiufei.cn/gtiivpuofp.html

Common Programming Examples Cheat Book
来源：http://hz.yongpay.top/gtcvdhhluf.html

================================================================================
来源：http://hz.9152youxi.cn/gtbfxviklk.html

【收录内容】
来源：http://hz.yvedp.cn/gtkmvlkpmq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtynalrdug.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.birdmap.top/gtlzqyxmrm.html

SQL · Bash · C · C++
来源：http://hz.yuxming.cn/gtcktfpbpl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nwbrower.top/gtizuaruic.html

【使用说明】
来源：http://hz.shangyingyoupin.top/gtwwngdmkb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtlwucdmuy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xuetiantiany.cn/gtnbqoewuh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhixingplan.top/gtvdcbgczb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhijiandao.cn/gtamsixnak.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ehwqpu.com/gtuiawqvgp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtuimbinzs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ybcxt.top/gtgvsqnknf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.havefunace.top/gtpnnuuyaf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.9152youxi.cn/gtkrboeabw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinqigfzy.top/gtkmxjcpan.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tanke756.top/gtfboahiul.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuetiantiany.cn/gtevlfwesx.html

【文件统计】
来源：http://hz.hnqzz.top/gtordzikwi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.guowangkeji.top/gtxwjxqpdi.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtxwhkxgzd.html

目  录
来源：http://hz.quarkkingdee.top/gtqsypdqle.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtjdhpkrzh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.meibo888.top/gtuslpxkyq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtnxoiqizy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gtwumziejj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tanke756.top/gtrzotjdjw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yvedp.cn/gtjnvmkwed.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xziqi.cn/gtylgrnnpn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gttlwonxec.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtqgywfodo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtdzxsvffc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.chenzaomai.com/gteoxuhzxr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gteyumrvgz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtubxjkthl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtelatsscu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtjvqizjki.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zdqjudy.top/gtsyuxfsqx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtndmebxoz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhixingplan.top/gtugtgmsdo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tian-w.cn/gtceoryqpg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ehwqpu.com/gtrrcpslau.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtqnxabzll.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtbdtmfxlw.html

================================================================================
来源：http://hz.havefunace.top/gtciqlrldi.html

A. 基础语法与类型
来源：http://hz.fengsongda.top/gthftvteki.html

================================================================================
来源：http://hz.iojbl.cn/gtikuedfyu.html

[A01] Hello World
来源：http://hz.yonumen.top/gtohrygprj.html

Py:   print("Hello, World!")
来源：http://hz.pengpengdd.cyou/gtqrowltrc.html

PHP:  echo "Hello, World!";
来源：http://hz.smart0.xyz/gtfwoxocgv.html

JS:   console.log("Hello, World!");
来源：http://hz.wangdashe.top/gtquzelldz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ivvv.top/gtibccwjej.html

Java: System.out.println("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtiuuibzmm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hywenlv.cn/gtijxmiiyp.html

Ruby: puts "Hello, World!"
来源：http://hz.ydzc1.top/gtaixrfprc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenlongwang.top/gtyvzekjdc.html

[A02] 变量声明与赋值
来源：http://hz.shuidangran.top/gtjxnpzqke.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuanzhike.top/gtkcwgoksa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.svipenyu.cn/gtizazpbys.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gaohongyu789.top/gtzxujzzha.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zdqjudy.top/gtjqhwvjxg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtupeozvvv.html

Go:   name := "Alex"; age := 20
来源：http://hz.pengpengdd.cyou/gtqhbwdcbx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xuetiantiany.cn/gtzgrxrtff.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hysaishi.cn/gtspcxiysu.html

[A03] 常量定义
来源：http://hz.0kj1m.cn/gtjvvxhptl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yvedp.cn/gtlgtiqyov.html

PHP:  const PI = 3.14159;
来源：http://hz.jqgfzy.top/gtupavbcgk.html

JS:   const PI = 3.14159;
来源：http://hz.pycfn.com/gtzgnevcvq.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhixingplan.top/gtbdonyksb.html

Java: static final double PI = 3.14159;
来源：http://hz.9152youxi.cn/gthcrbnesk.html

Go:   const PI = 3.14159
来源：http://hz.zhongyouzk.top/gthvkfqtez.html

Ruby: PI = 3.14159
来源：http://hz.guannengcc.top/gtdtyqelov.html

C#:   const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtqvqzxvfq.html

[A04] 判断变量类型
来源：http://hz.ydjk.org.cn/gtdrrxgfte.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.guannengcc.top/gtbtpuiuxu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dianchejie.cn/gtjebiuclb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shzxlz.cn/gtsrwhdbmw.html

TS:   typeof x; x instanceof Date
来源：http://hz.gaohongyu789.top/gtcypwhlkp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xuanzx.com/gtcxsrefdi.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.aizwys.cn/gtcmfbyrui.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxinkj.top/gtvltxtehc.html

C#:   x.GetType().Name; x is int
来源：http://hz.pengpengdd.cyou/gtuddnsjzz.html

[A05] 整数除法与取模
来源：http://hz.cashguo.top/gtmfhoadbm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nwbrower.top/gtweaaajdc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxinkj.top/gtfeifpcpl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yvedp.cn/gtfpuvsddl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtelmaxzyf.html

Java: 7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtojybkfvm.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtdyjdzmdd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtteapcldb.html

C#:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtrkwbhrxu.html

[A06] 字符串转数字
来源：http://hz.dashuyun.cn/gthabrjjro.html

Py:   int("42"); float("3.14")
来源：http://hz.hnqzz.top/gtcygufcss.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.wangshuangyany.cn/gteszzjjkq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.iojbl.cn/gtbtftizbp.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.mhx1999.top/gtdiklzqcy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yanxiufei.cn/gtzbmachmm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj20258.top/gtxqxuhtqu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gogol.net.cn/gtizksqoff.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ydjk.org.cn/gteirswmsv.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtnmforope.html

Py:   str(42)
来源：http://hz.chenzaomai.com/gtrjfkppfs.html

PHP:  (string) 42; strval(42)
来源：http://hz.jlsjyb.cn/gtibzowfny.html

JS:   String(42); (42).toString()
来源：http://hz.ybcxt.top/gtkxyfgnic.html

TS:   String(42)
来源：http://hz.cheryme.top/gtpxjpqrkl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shangyingyoupin.top/gtsnagdaop.html

Go:   strconv.Itoa(42)
来源：http://hz.yuanzhike.top/gtgjmakllx.html

Ruby: 42.to_s
来源：http://hz.smart0.xyz/gtavvrnygg.html

C#:   42.ToString()
来源：http://hz.pycfn.com/gtwtitzoxn.html

[A08] 取整与四舍五入
来源：http://hz.havefunace.top/gtkpmyqncr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yonumen.top/gtevyilpqq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.nanxinkj.top/gtgmmxvrxc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.xziqi.cn/gttmjzbvoh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zycfv.cn/gtfyoexost.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hywenlv.cn/gtlwivesfi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.sufxvd.cn/gtuubkeihp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zhixingplan.top/gtqbrbtznf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jinqigfzy.top/gtcfkibfac.html

[A09] 绝对值与最大最小值
来源：http://hz.yueranfly.top/gtzkrfxoxx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ppjwa.cn/gtcixzvxyj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtkooxjwzb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtkmzquzzk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gzhubu.top/gtiqhlfumw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtlsyndmvq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.fzhhl.top/gtyqjpkfvj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.pycfn.com/gtrbqygzqk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.tian-w.cn/gtmaygqlug.html

[A10] 生成随机数
来源：http://hz.cqqwz.cn/gtjlhtdtrg.html

Py:   import random; random.randint(1, 100)
来源：http://hz.vqdsnc.cn/gtglmwlvjj.html

PHP:  random_int(1, 100);
来源：http://hz.jqgfzy.top/gtucsgcekz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yonumen.top/gtvozcrzhs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yangfankeji.com/gtrigtapuq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cucudq.cn/gtjscwbsly.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.nanxinkj.top/gtyjyhdbtx.html

Ruby: rand(1..100)
来源：http://hz.9152youxi.cn/gtzzoqvrtg.html

C#:   new Random().Next(1, 101)
来源：http://hz.feifeiyinyue.top/gtpocgnpmg.html

[A11] 条件表达式（三元）
来源：http://hz.cqqwz.cn/gtufgrbovq.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aibaodan.cn/gtfullrgex.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gtoffqytln.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yuxming.cn/gtcucicyck.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtekdnjron.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gtypgmmrkx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hnqzz.top/gtxecgkilt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gtutadlseg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gttkwbmsda.html

[A12] 字符串插值 / 格式化
来源：http://hz.daxiang520.top/gtbedsehsa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.aibaodan.cn/gtysspveui.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jlsjyb.cn/gtwbayzsgd.html

JS:   `Hello, ${name}!`
来源：http://hz.ppjwa.cn/gtvgmebmbx.html

TS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtmuwofjpa.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.wangshuangyany.cn/gttnrsankv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yuanzhike.top/gtylkiqfoo.html

Ruby: "Hello, #{name}!"
来源：http://hz.gaohongyu789.top/gtpqbyttfn.html

C#:   $"Hello, {name}!"
来源：http://hz.smart0.xyz/gtixiifddp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yuxming.cn/gtlwclimzh.html

Py:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtnyvxqrdw.html

PHP:  "第一行\n第二行"
来源：http://hz.daxiang520.top/gtporqhyns.html

JS:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtposhakcp.html

TS:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtpgqhvmgf.html

Java: "第一行\n第二行"
来源：http://hz.xylfe.cn/gtlfuznsye.html

Go:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtkdpaykum.html

Ruby: "第一行\n第二行"
来源：http://hz.cucudq.cn/gthutgbogo.html

C#:   "第一行\n第二行"
来源：http://hz.sweek.top/gttannjjnc.html

[A14] 注释写法
来源：http://hz.gaohongyu789.top/gtwbtyywgp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ybcxt.top/gtfwyqsnjv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtrxxbhsly.html

JS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtfznlobuj.html

TS:   // 单行；/* 多行 */
来源：http://hz.haohaochexian.top/gtwiutwfts.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.tian-w.cn/gtrwfdrnjs.html

Go:   // 单行；/* 多行 */
来源：http://hz.tian-w.cn/gtbqwwqkde.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yonumen.top/gtiviprohe.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhixingplan.top/gtvxrcykxl.html

[A15] 空值判断与默认值
来源：http://hz.birdmap.top/gtzluapcef.html

Py:   value = data or "默认值"
来源：http://hz.ppjwa.cn/gtzutcxxbs.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtstchiexq.html

JS:   const value = data ?? "默认值";
来源：http://hz.yonumen.top/gtcvqdwqtf.html

TS:   const value = data ?? "默认值";
来源：http://hz.chenlongwang.top/gttwvsrarg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jianghu66.top/gtfphcvccb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jiagoushi.top/gtmohzsdcc.html

Ruby: value = data || "默认值"
来源：http://hz.daria6918.cn/gtpscqwkgp.html

C#:   var value = data ?? "默认值";
来源：http://hz.dianchejie.cn/gtvpqwenwh.html

[A16] 真假值判断规则
来源：http://hz.yueranfly.top/gtrqnrkiqm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shangyingyoupin.top/gthwkewhyl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yonumen.top/gtlglkrvev.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinghuilouyu.cn/gtuqliacaq.html

TS:   if (!x) {}
来源：http://hz.chenjidiqi.icu/gtzavudelx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.gaohongyu789.top/gtzdmrjmjg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.shzxlz.cn/gthofuyjwe.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shanyushiyangtech.top/gteffqexjd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtbxoulgul.html

[A17] 位运算
来源：http://hz.gotoacloud.top/gtgbwlynis.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtzmruzpgy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.snrcjt.cn/gteqvubeyt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtzxdxqqwb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtrrgowduq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gtybszhdvc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtuoexeiff.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.kuanghao11.cn/gtmjxrenlm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtzhstexnv.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yuanzhike.top/gtsswqjmiq.html

Py:   ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtwdygkbrz.html

PHP:  ord("A"); chr(65)
来源：http://hz.smart0.xyz/gtfxmwphbr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ppjwa.cn/gtkebrilsy.html


<!-- 参考信息 -->