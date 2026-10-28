代发 wailian999

[U105] JS：节流
来源：http://hz.guannengcc.top/gtriqfmhpv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhoulong.xyz/gtwctcqbne.html

[U106] JS：日期格式化
来源：http://hz.zhengqikj.top/gtpwdamrcd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.52xcode.cn/gtgtoffkxe.html

[U107] JS：数字千分位
来源：http://hz.jlsjyb.cn/gtzfcnvkxe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtcghsleci.html

[U108] JS：随机整数
来源：http://hz.cheryme.top/gttzxmiexd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shuidangran.top/gtxnwjcgnp.html

[U109] JS：数组分组
来源：http://hz.xziqi.cn/gtmerqesll.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtssfyyaxz.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangkeji.top/gtkkpulpzv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinghuilouyu.cn/gtwofdglid.html

[U111] JS：对象转 Map
来源：http://hz.yonumen.top/gtnfmeugrx.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtisucecan.html

[U112] JS：字符串补位
来源：http://hz.0kj1m.cn/gtwrzxokvr.html

"7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtorgkrbci.html

[U113] JS：正则替换全部
来源：http://hz.jinqigufen.top/gtenbcvaue.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtgovnrdda.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258.top/gtbwxlrznh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtjcrwxrkp.html

[U115] JS：生成 UUID
来源：http://hz.xinyue.icu/gthmxnaftu.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtmbvirtbh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.c1oappe.top/gtshqdeujj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtpdsprnmp.html

[U117] JS：单元测试
来源：http://hz.redwolf501.top/gtnmegrxpu.html

npm i -D vitest;  npx vitest
来源：http://hz.chenlongwang.top/gtcrjxffoz.html

[U118] JS：开发服务器
来源：http://hz.gotoacloud.top/gtvcyzdwos.html

npm i -D vite;  npx vite
来源：http://hz.xuanzx.com/gtwuollqjm.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtxislcsib.html

npx vite build
来源：http://hz.gotoacloud.top/gtppwvukse.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gttmvmoyzj.html

import.meta.env.VITE_API_URL
来源：http://hz.yongpay.top/gtmcmloscl.html

================================================================================
来源：http://hz.xuanzx.com/gtoqxserin.html

统计汇总
来源：http://hz.cucudq.cn/gtioywvdbt.html

================================================================================
来源：http://hz.chenlongwang.top/gtgefzkywd.html

按语言统计（条）：
来源：http://hz.fzhhl.top/gtoidqayjl.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gtobvhwdda.html

PHP ............ 252
来源：http://hz.haohaochexian.top/gtoogeklgc.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gtgfclbxyf.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtdfxdkibt.html

Java ........... 212
来源：http://hz.yj20258.top/gtqsrdvmji.html

Go ............. 212
来源：http://hz.fengsongda.top/gtcssetbvp.html

Ruby ........... 212
来源：http://hz.gotoacloud.top/gtieoutqkf.html

C# ............. 212
来源：http://hz.c1oappe.top/gtjvthjmcp.html

C .............. 30
来源：http://hz.aizwys.cn/gtleidsqvp.html

C++ ............ 30
来源：http://hz.meibo888.top/gtwkcftayx.html

SQL ............ 90
来源：http://hz.ppjwa.cn/gtvhlrgpvw.html

Bash ........... 80
来源：http://hz.guannengcc.top/gtrrfunbmf.html

Kotlin ......... 15
来源：http://hz.ybcxt.top/gtzjptvbej.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gttrkparus.html

Lua ............ 10
来源：http://hz.cucudq.cn/gtglaircvu.html

Perl ........... 10
来源：http://hz.vqdsnc.cn/gttdllkydt.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtymmjcaus.html

------------------------------------
来源：http://hz.xuanzx.com/gtsqpkjszt.html

合计 ........... 2106 条
来源：http://hz.316326.xyz/gturqmhcfl.html

按章节统计：
来源：http://hz.hfpthk.cn/gtpsbknhov.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtkgvaliuw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtrlzvmegh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtqbcmuaes.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtndpqvegy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhiwuduotai.top/gtqpevxhqs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ydjk.org.cn/gtnwttctfp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtgjuqweor.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtypvgweaw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtfquxkxkx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hnxiangtu.top/gtqtltbkua.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtvpdcaazm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtdyksvjnu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtvbtwzhvi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cashguo.top/gtnxihctpx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.52xcode.cn/gtmerdjkit.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtjpzwzxcu.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangtech.top/gtprtdvgvj.html

R Bash 专题                             80
来源：http://hz.nanxinkj.top/gttsntdbgt.html

S C / C++ 专题                          60
来源：http://hz.hysaishi.cn/gthkzgqnxo.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtblrqaxoo.html

U 高频实用片段                         120
来源：http://hz.jyoumei.cn/gtmszzmqri.html

------------------------------------
来源：http://hz.sufxvd.cn/gtdamcvpev.html

合计                                  2106 条
来源：http://hz.zhiwuduotai.top/gttadvdfef.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtjjcmfqnm.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtqrdknwka.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtluxatbil.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guowangkeji.top/gtadzzldjn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yueranfly.top/gthhmlhkvb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yonumen.top/gtfqucwcfj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.quarkkingdee.top/gtrsoeckom.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jqgufenzy.top/gtjmhgsyle.html

—— 文件结束 ——
来源：http://hz.316326.xyz/gtauglebon.html

================================================================================
来源：http://hz.yuanzhike.top/gtdlhiixzq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.daria6918.cn/gtlwablobt.html

Common Programming Examples Cheat Book
来源：http://hz.316326.xyz/gtfteslfsr.html

================================================================================
来源：http://hz.jqgfzy.top/gtpxxznilt.html

【收录内容】
来源：http://hz.gogol.net.cn/gtozykpiqp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhaomingkeji.xyz/gthhhvgtcd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tianlin.xyz/gtgkhbaqhq.html

SQL · Bash · C · C++
来源：http://hz.52xcode.cn/gttcpmjeyq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtvdnpfxgr.html

【使用说明】
来源：http://hz.vqdsnc.cn/gtosfnxyfc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtbiqvnffi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cucudq.cn/gtwegzukkb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yonumen.top/gtupdxxpme.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.guannengcc.top/gtcnpzojbd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxuanxn.top/gtgvifdkze.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ehwqpu.com/gtmbogetzn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hysaishi.cn/gteadhvhwo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hnqzz.top/gtvrcicomn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.fengsongda.top/gtneggujrw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ydjk.org.cn/gthiukukjt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.aibaodan.cn/gtjkjykwvw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.smart0.xyz/gthueaidal.html

【文件统计】
来源：http://hz.vqdsnc.cn/gtutaoclkj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.daria6918.cn/gttrikxqby.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtftvzzmdf.html

目  录
来源：http://hz.haohaochexian.top/gtqabjnwdw.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtuwpmziab.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhoulong.xyz/gtkvotlrbn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtqtgfippj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gthmofvhlf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.mhx1999.top/gtskxmezci.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtvqzfqppu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gttudwbzuk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gttkiowhnz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhaomingkeji.xyz/gtpinolxwb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtihwgvjqu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtdwitjpzh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtgsuzolry.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtmdpgkugi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtnhctzqmp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtwshuzppj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nwbrower.top/gttemnzctm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtfyaqsivo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.chenlongwang.top/gtqnvyopuf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tian-w.cn/gtnqswsylt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinqigufen.top/gtpyjwzwny.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtymogfrld.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtnmiokgrn.html

================================================================================
来源：http://hz.daria6918.cn/gtqyzytsuu.html

A. 基础语法与类型
来源：http://hz.c1oappe.top/gtvjywuzmq.html

================================================================================
来源：http://hz.sysykeji.top/gtnywzoxft.html

[A01] Hello World
来源：http://hz.jqgufenzy.top/gtfoeanysc.html

Py:   print("Hello, World!")
来源：http://hz.shzxlz.cn/gtdmssamia.html

PHP:  echo "Hello, World!";
来源：http://hz.hnqzz.top/gtnpfywbob.html

JS:   console.log("Hello, World!");
来源：http://hz.guannengcc.top/gtanjcrenw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hfpthk.cn/gtfrcfiqmh.html

Java: System.out.println("Hello, World!");
来源：http://hz.cqqwz.cn/gtmdeczcwx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydjk.org.cn/gtvskpwpjf.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtzdsmxhet.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jqgufenzy.top/gtnncueikm.html

[A02] 变量声明与赋值
来源：http://hz.yvedp.cn/gtnyxxpehn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hfpthk.cn/gtkehspinz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hongshengwenyu.top/gtgdopdjgl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.snrcjt.cn/gtgzpatmdj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shzxlz.cn/gtixffpmki.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hysaishi.cn/gtndoqojui.html

Go:   name := "Alex"; age := 20
来源：http://hz.cucudq.cn/gtjgzdcjis.html

Ruby: name = "Alex"; age = 20
来源：http://hz.redwolf501.top/gtpjrfdzzd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cqqwz.cn/gtiooxnxkv.html

[A03] 常量定义
来源：http://hz.hongshengwenyu.top/gtlyzxilli.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuanzhike.top/gtbtysimfr.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtkjaymmwe.html

JS:   const PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtsvgojccv.html

TS:   const PI: number = 3.14159;
来源：http://hz.daria6918.cn/gttneuzurd.html

Java: static final double PI = 3.14159;
来源：http://hz.nwbrower.top/gtadduitgs.html

Go:   const PI = 3.14159
来源：http://hz.jqgufenzy.top/gtudalkvcc.html

Ruby: PI = 3.14159
来源：http://hz.yj202588.top/gtdqvnkymk.html

C#:   const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtahbvnhno.html

[A04] 判断变量类型
来源：http://hz.jinqigufen.top/gtlpojynqx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xingfuxueyuan.xyz/gtpbjdhlez.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigufen.top/gtcyboyknm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nanxuanxn.top/gtjpgfoeus.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtfkzmrnws.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangkeji.top/gtjiqrxhld.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhongyouzk.top/gtmocwndqj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinqigufen.top/gtkyvqcpfb.html

C#:   x.GetType().Name; x is int
来源：http://hz.c1oappe.top/gteiimskmj.html

[A05] 整数除法与取模
来源：http://hz.ivvv.top/gtxvwudaes.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gaohongyu789.top/gttronxtik.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.svipenyu.cn/gtkiatzmzu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtjkvlczjs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtidlrenul.html

Java: 7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gtprvedznq.html

Go:   7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtlswoqpvh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtnmimztav.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtmowkepmk.html

[A06] 字符串转数字
来源：http://hz.cucudq.cn/gtfcboxvtr.html

Py:   int("42"); float("3.14")
来源：http://hz.cucudq.cn/gtrbwxrwcf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hongshengwenyu.top/gtnugieeah.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jqgufenzy.top/gtbnhshtht.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinqigfzy.top/gtmbweyxzz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gogol.net.cn/gtjfpemonn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shzxlz.cn/gtovljmpym.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.tian-w.cn/gtdmpvgnje.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ybcxt.top/gtvxrrwptf.html

[A07] 数字转字符串
来源：http://hz.yangfankeji.com/gtgnyaywzp.html

Py:   str(42)
来源：http://hz.guannengcc.top/gtluesgygb.html

PHP:  (string) 42; strval(42)
来源：http://hz.jqgfzy.top/gtwoqfbpja.html

JS:   String(42); (42).toString()
来源：http://hz.shangyingyoupin.top/gtxjctrlyb.html

TS:   String(42)
来源：http://hz.mhx1999.top/gtiexedkcj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.guowangkeji.top/gtbevjwlit.html

Go:   strconv.Itoa(42)
来源：http://hz.xingfuxueyuan.xyz/gtkqqitrjf.html

Ruby: 42.to_s
来源：http://hz.cheryme.top/gtihwspzbn.html

C#:   42.ToString()
来源：http://hz.nanxuanxn.top/gtbducbtwa.html

[A08] 取整与四舍五入
来源：http://hz.dashuyun.cn/gtevdilfar.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.gogol.net.cn/gtakbgtbmv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tianlin.xyz/gttgygclhe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.dashuyun.cn/gtsjrsnkfb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.havefunace.top/gtfcljyaip.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nanxinkj.top/gtrjyxqnws.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yj202588.top/gtszmcfemr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jiagoushi.top/gtpczclkzr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nanxinkj.top/gttohluiql.html

[A09] 绝对值与最大最小值
来源：http://hz.aibaodan.cn/gtzofsdvph.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gtbrwtmybx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.snrcjt.cn/gtwasyrxyv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hnxiangtu.top/gtqsgahyly.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtkqmycazc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hywenlv.cn/gtufdcdrrn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.vqdsnc.cn/gtdwqscmae.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.nanxuanxn.top/gtgtzfcuel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xuanzx.com/gtlkbemrgt.html

[A10] 生成随机数
来源：http://hz.316326.xyz/gtrdxyaagb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.tianlin.xyz/gtjvouohcv.html

PHP:  random_int(1, 100);
来源：http://hz.hammf.cn/gtgwdvhnkb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.dianchejie.cn/gtfprnkiyq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gaohongyu789.top/gtjrrzapun.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yongpay.top/gtxajwubex.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.chenjidiqi.icu/gtvhfrabrf.html

Ruby: rand(1..100)
来源：http://hz.hnqzz.top/gtluxppgve.html

C#:   new Random().Next(1, 101)
来源：http://hz.xingfuxueyuan.xyz/gtbvauwlmd.html

[A11] 条件表达式（三元）
来源：http://hz.redwolf501.top/gtuydnnzip.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cdnleiting.top/gtydsxxcgq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhoulong.xyz/gttdmpirrf.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.snrcjt.cn/gtwxrhzogo.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gtigrwlora.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gtmszpwbkq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhongyouzk.top/gtzpnwqmdr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtxfjvjyzv.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtplmhdwuj.html

[A12] 字符串插值 / 格式化
来源：http://hz.redwolf501.top/gtythmqtpi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.zhengqikj.top/gtunqzovzp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.aizwys.cn/gtkmrnydsr.html

JS:   `Hello, ${name}!`
来源：http://hz.ppjwa.cn/gtbdqnzvvj.html

TS:   `Hello, ${name}!`
来源：http://hz.jianghu66.top/gteocgampx.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.birdmap.top/gtwrmhgchc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yueranfly.top/gtvsnnnpnz.html

Ruby: "Hello, #{name}!"
来源：http://hz.hfpthk.cn/gtgxqvusix.html

C#:   $"Hello, {name}!"
来源：http://hz.zhengqikj.top/gtvztvcslt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cucudq.cn/gttlnuqjxi.html

Py:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtuvaiqsrh.html

PHP:  "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtgvaikmdm.html

JS:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtzgdgpizf.html

TS:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtdaqexeph.html

Java: "第一行\n第二行"
来源：http://hz.redwolf501.top/gtcmrofokm.html

Go:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtpczpmydq.html

Ruby: "第一行\n第二行"
来源：http://hz.ydzc1.top/gtudwrreep.html

C#:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtmmncyagk.html

[A14] 注释写法
来源：http://hz.52xcode.cn/gtpqxlrpca.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ybcxt.top/gtljnqnbxl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hongshengwenyu.top/gttlbmsoik.html

JS:   // 单行；/* 多行 */
来源：http://hz.yongpay.top/gtiybqbcld.html

TS:   // 单行；/* 多行 */
来源：http://hz.gotoacloud.top/gtmiwzlvky.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hnqzz.top/gtzgmzwddd.html

Go:   // 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtywwdczxb.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.havefunace.top/gteqjqpaoi.html

C#:   // 单行；/* 多行 */
来源：http://hz.sweek.top/gtzdpamntn.html

[A15] 空值判断与默认值
来源：http://hz.jinghuilouyu.cn/gtocodymvs.html

Py:   value = data or "默认值"
来源：http://hz.pengpengdd.cyou/gtzqetmimh.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.sxryk.cn/gtibkercjt.html

JS:   const value = data ?? "默认值";
来源：http://hz.wangdashe.top/gtycxhvopa.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhixingplan.top/gtbundbyur.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.snrcjt.cn/gtcscllajb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ivvv.top/gtiqwskqvk.html

Ruby: value = data || "默认值"
来源：http://hz.zhoulong.xyz/gtqeukbsvk.html

C#:   var value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gtquhhaafc.html

[A16] 真假值判断规则
来源：http://hz.gogol.net.cn/gtdspixdht.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shuidangran.top/gtagxukeds.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sxryk.cn/gtwystukdr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.tianlin.xyz/gtofmfawqp.html

TS:   if (!x) {}
来源：http://hz.hywenlv.cn/gttlqbublg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.pengpengdd.cyou/gtmlzigqhg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinqigfzy.top/gtjxmblinq.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.quarkkingdee.top/gthofdwlam.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yj20258.top/gtcwjvohzc.html

[A17] 位运算
来源：http://hz.aibaodan.cn/gthnlhtzbt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtjzufgisr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xziqi.cn/gtdtazsqgy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtlmekzmqv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtltuoaebt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtumvufcuu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtfcukbiuw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtjssmmkch.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gttdehcgzs.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ydzc1.top/gtvciutppj.html

Py:   ord("A"); chr(65)
来源：http://hz.52xcode.cn/gtybrfbwvn.html

PHP:  ord("A"); chr(65)
来源：http://hz.hnqzz.top/gtdpaoaqzl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jianghu66.top/gtjmchqfwz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.haohaochexian.top/gtchoquiuy.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhoulong.xyz/gtfjnoqlqr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.chenzaomai.com/gtkdyporfm.html

Ruby: "A".ord; 65.chr
来源：http://hz.tanke756.top/gtscznfdbo.html


<!-- 参考信息 -->