代发 wailian999

[U103] JS：定时器
来源：http://hz.xuanzx.com/gtwtdbpdqk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gthvucqgmq.html

[U104] JS：防抖
来源：http://hz.aizwys.cn/gtfexnqpah.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtidgiaclu.html

[U105] JS：节流
来源：http://hz.zhijiandao.cn/gtxnulrffs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yanxiufei.cn/gtyaokspav.html

[U106] JS：日期格式化
来源：http://hz.zhixingplan.top/gttbmlzfbd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.andypj.xyz/gtnilbmdmu.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gthoqgncvc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gtltudgdji.html

[U108] JS：随机整数
来源：http://hz.ydjk.org.cn/gtrmfbvxfl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigufen.top/gtnrzybwro.html

[U109] JS：数组分组
来源：http://hz.cheryme.top/gtuhbnwcqk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtvztnwgui.html

[U110] JS：数组分块
来源：http://hz.vqdsnc.cn/gtwxnnsear.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gthyshmciv.html

[U111] JS：对象转 Map
来源：http://hz.nanxuanxn.top/gtkqsagxyu.html

new Map(Object.entries(obj))
来源：http://hz.hysaishi.cn/gtqbmwujfx.html

[U112] JS：字符串补位
来源：http://hz.ydzc1.top/gtcuzqsdet.html

"7".padStart(3, "0")
来源：http://hz.tanke756.top/gtjboexfll.html

[U113] JS：正则替换全部
来源：http://hz.tianlin.xyz/gtdgfytfkw.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtwdazfdix.html

[U114] JS：JSON 深比较
来源：http://hz.ppjwa.cn/gtrkqrzdgi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtwgtzffkr.html

[U115] JS：生成 UUID
来源：http://hz.haohaochexian.top/gteichtubf.html

crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtmgldsytf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ppjwa.cn/gtaocxzqcf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shanyushiyangtech.top/gthurrxpqt.html

[U117] JS：单元测试
来源：http://hz.xinyue.icu/gtudlcwwvg.html

npm i -D vitest;  npx vitest
来源：http://hz.svipenyu.cn/gtubelgitp.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gttspfswfi.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtcukioixe.html

[U119] JS：生产构建
来源：http://hz.nanxuanxn.top/gtqcssebpn.html

npx vite build
来源：http://hz.sweek.top/gttecixtiq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gtaghtwmxj.html

import.meta.env.VITE_API_URL
来源：http://hz.dashuyun.cn/gtzdghwbsu.html

================================================================================
来源：http://hz.havefunace.top/gtjslxllcc.html

统计汇总
来源：http://hz.cqqwz.cn/gtkrdkhurb.html

================================================================================
来源：http://hz.cheryme.top/gtelmwpfzn.html

按语言统计（条）：
来源：http://hz.shanyushiyangkeji.top/gtkavjlgap.html

Python ......... 252
来源：http://hz.xuanzx.com/gtbzaakjqn.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gtfjtneyrj.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gtmscsqonq.html

TypeScript ..... 212
来源：http://hz.zhengqikj.top/gtvstedmit.html

Java ........... 212
来源：http://hz.daxiang520.top/gtwdoxszmz.html

Go ............. 212
来源：http://hz.havefunace.top/gtrvcxhefj.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtgosrllee.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtssfomfeb.html

C .............. 30
来源：http://hz.hongshengwenyu.top/gtxbusvydd.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtlrvzyjxy.html

SQL ............ 90
来源：http://hz.fzhhl.top/gtrxedyten.html

Bash ........... 80
来源：http://hz.aibaodan.cn/gtgdupbxrx.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtzzqgkbnh.html

Swift .......... 15
来源：http://hz.iojbl.cn/gtokjfgwty.html

Lua ............ 10
来源：http://hz.iojbl.cn/gtoelvvcpb.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtelwqwbxy.html

Scala .......... 10
来源：http://hz.xuanzx.com/gtbcxhznme.html

------------------------------------
来源：http://hz.cheryme.top/gthamxfdyr.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gtrzqfjjpx.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtwekzzhfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gthpqmxhqd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtbikvvnme.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtqwchszuy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtslwojdqg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.c1oappe.top/gtvdomhtor.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtllgsehwz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtbnvkunwg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yongpay.top/gtaumnbbff.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gthvfuhfkk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtiugyjklt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtxhcsoxnn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtlbxkxrkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtbryazccn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gzhubu.top/gtzymebjow.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cheryme.top/gtlkhxplxt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtbiyvusvq.html

Q SQL 专题                              90
来源：http://hz.pycfn.com/gtgttgcpwd.html

R Bash 专题                             80
来源：http://hz.yj20258888.top/gtxuasuqte.html

S C / C++ 专题                          60
来源：http://hz.redwolf501.top/gtceuwkaug.html

T 其他语言补充                          60
来源：http://hz.yuanzhike.top/gtluqdtcuj.html

U 高频实用片段                         120
来源：http://hz.mhx1999.top/gtzgnllamv.html

------------------------------------
来源：http://hz.xinyue.icu/gtxwsgdlaj.html

合计                                  2106 条
来源：http://hz.gaohongyu789.top/gtexyhmbvv.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtwerfxkts.html

使用提醒
来源：http://hz.shuidangran.top/gtkzmbjoxd.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtiesnzamj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtzhxilcnr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj20258.top/gtwxtdbnid.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shanyushiyangtech.top/gtjsizskhy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtpcctbscu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhoulong.xyz/gtxusbiyhw.html

—— 文件结束 ——
来源：http://hz.bjfxy.top/gtqypmzhfa.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnxyxfjlc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yonumen.top/gtycksxazc.html

Common Programming Examples Cheat Book
来源：http://hz.vqdsnc.cn/gtbkrgcygu.html

================================================================================
来源：http://hz.yvedp.cn/gtfrlactzy.html

【收录内容】
来源：http://hz.xuanzx.com/gtsrsyccnx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sufxvd.cn/gtypeokczo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.vqdsnc.cn/gtryprfazx.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gthfetusjk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.tianlin.xyz/gtybtyvfcc.html

【使用说明】
来源：http://hz.xylfe.cn/gtpmikyplo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.9152youxi.cn/gthlwcmeyf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhengqikj.top/gtzwzajrov.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtfffstatz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cashguo.top/gtqsivdtwg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.guannengcc.top/gtgydsmpxf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ywan-chungtsiang.top/gtsntdbdcj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.kuanghao11.cn/gtefcydcfz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hysaishi.cn/gtvsvpwwrb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenjidiqi.icu/gtskvghtpv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shangyingyoupin.top/gtqeyndgav.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shanyushiyangtech.top/gtgvhigdyg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gotoacloud.top/gtznfspupu.html

【文件统计】
来源：http://hz.jyoumei.cn/gtufgzryjb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yonumen.top/gtahlpfahx.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtmbvvijpz.html

目  录
来源：http://hz.cucudq.cn/gtabalmyxz.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtutudqgdq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xuetiantiany.cn/gtdmgjkhwo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gttzyctfsu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ehwqpu.com/gtccrrrext.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gtgrugudsi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxinkj.top/gtsotfmroq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.c1oappe.top/gtgrszlxcm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ybcxt.top/gtcimkrnwa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hfpthk.cn/gtfwjvhmpj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtxwnvhvdh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtyqvzdqyo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtaapzdejz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtxdxqougy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtxgalfpum.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gtqqjfoilq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.vqdsnc.cn/gtjfwnoemm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtazdwdmdr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hongshengwenyu.top/gtdtigabto.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxuanxn.top/gtbrklcede.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.vqdsnc.cn/gthdxgiydq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtbxjrjgbs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.andypj.xyz/gtptkftlfj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtulteramg.html

A. 基础语法与类型
来源：http://hz.sxryk.cn/gtzwscclpb.html

================================================================================
来源：http://hz.0kj1m.cn/gtvhegcufs.html

[A01] Hello World
来源：http://hz.vqdsnc.cn/gtykzgrirr.html

Py:   print("Hello, World!")
来源：http://hz.zycfv.cn/gtlyvpllpk.html

PHP:  echo "Hello, World!";
来源：http://hz.xingfuxueyuan.xyz/gtlzabycye.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258888.top/gtkhsluccu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jiagoushi.top/gtftcfosvc.html

Java: System.out.println("Hello, World!");
来源：http://hz.meibo888.top/gtmihftwvz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258.top/gtvnqllczr.html

Ruby: puts "Hello, World!"
来源：http://hz.0kj1m.cn/gtaavtknsl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangdashe.top/gteuqnfelj.html

[A02] 变量声明与赋值
来源：http://hz.aibaodan.cn/gtrhytyfnj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.feifeiyinyue.top/gtdsbvnkrk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nwbrower.top/gtpxpbcwbb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hysaishi.cn/gtmxzllchi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yuxming.cn/gtcrrijjpd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cheryme.top/gtsvoeojbm.html

Go:   name := "Alex"; age := 20
来源：http://hz.nanxinkj.top/gthbppyjqa.html

Ruby: name = "Alex"; age = 20
来源：http://hz.haohaochexian.top/gtqlkwpopu.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtkrqdfxnv.html

[A03] 常量定义
来源：http://hz.ywan-chungtsiang.top/gtsctxutnr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ydjk.org.cn/gtadlfvcta.html

PHP:  const PI = 3.14159;
来源：http://hz.52xcode.cn/gtqxtdmuyp.html

JS:   const PI = 3.14159;
来源：http://hz.xylfe.cn/gthagavnga.html

TS:   const PI: number = 3.14159;
来源：http://hz.sufxvd.cn/gtjbwmwivv.html

Java: static final double PI = 3.14159;
来源：http://hz.gzhubu.top/gtwwbjlixp.html

Go:   const PI = 3.14159
来源：http://hz.wangshuangyany.cn/gtarnhhynx.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtirxuruuw.html

C#:   const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtnvcbtdyi.html

[A04] 判断变量类型
来源：http://hz.snrcjt.cn/gtjvuizqjy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydjk.org.cn/gtjcgimleq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pycfn.com/gtvxzzvpng.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yuxming.cn/gtzrzwwmav.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhiwuduotai.top/gtszsytijl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pengpengdd.cyou/gtqgsajbpm.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hfpthk.cn/gthqjdqedd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.c1oappe.top/gtaykvtrin.html

C#:   x.GetType().Name; x is int
来源：http://hz.xuanzx.com/gtttoykdjs.html

[A05] 整数除法与取模
来源：http://hz.wangdashe.top/gthebvngau.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj20258888.top/gtkygjzopd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.birdmap.top/gtcuhdbtci.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yanxiufei.cn/gtzzojnxat.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuanzhike.top/gtxfgfxdqd.html

Java: 7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtyqtbyqee.html

Go:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtwvynduom.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtftlsjwhv.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtxkofcfxl.html

[A06] 字符串转数字
来源：http://hz.zhijiandao.cn/gtmencrbru.html

Py:   int("42"); float("3.14")
来源：http://hz.ydzc1.top/gtbpnmbyya.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gotoacloud.top/gtqkyorwxn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shanyushiyangkeji.top/gtzquvivsb.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yangfankeji.com/gtyslogldl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhoulong.xyz/gtoopoyqoi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.snrcjt.cn/gttvnsohjn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhiwuduotai.top/gtpxdbztav.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.chenzaomai.com/gtbowpvxfb.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtddbwbvkt.html

Py:   str(42)
来源：http://hz.0kj1m.cn/gtpkpuenmd.html

PHP:  (string) 42; strval(42)
来源：http://hz.yuanzhike.top/gtxwexaeic.html

JS:   String(42); (42).toString()
来源：http://hz.jlsjyb.cn/gtaniwwlzy.html

TS:   String(42)
来源：http://hz.nanxuanxn.top/gtpyxbuqoz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ywan-chungtsiang.top/gthwrortbi.html

Go:   strconv.Itoa(42)
来源：http://hz.aibaodan.cn/gthqjkwcvx.html

Ruby: 42.to_s
来源：http://hz.yueranfly.top/gthdghfacc.html

C#:   42.ToString()
来源：http://hz.yongpay.top/gttnibyjcs.html

[A08] 取整与四舍五入
来源：http://hz.shangyingyoupin.top/gtxnukytzw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.52xcode.cn/gttlsrmhmy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.vqdsnc.cn/gtiqzhozch.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sweek.top/gtxcfmcizc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.tanke756.top/gtbfokvjyf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gttrxpbdzs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xinyue.icu/gtfpeknwdr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.9152youxi.cn/gtouwmjvdj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.redwolf501.top/gtyjkndnhh.html

[A09] 绝对值与最大最小值
来源：http://hz.9152youxi.cn/gtmjidmacb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.redwolf501.top/gtvhegaqiw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtvuyqyxdu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hongshengwenyu.top/gtjwmlrsfd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.xuanzx.com/gtlccdvjcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigufen.top/gtayhrsmay.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cheryme.top/gtrbqkfjlc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.havefunace.top/gtiqgewoio.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.cdnleiting.top/gtosotzrfe.html

[A10] 生成随机数
来源：http://hz.ppjwa.cn/gtzhstepwb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.gzhubu.top/gtozhivhjn.html

PHP:  random_int(1, 100);
来源：http://hz.nwbrower.top/gtqwjokwbm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuanzhike.top/gtdrbvekle.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shangyingyoupin.top/gtelcglkzm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinghuilouyu.cn/gtqhcvgbep.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yonumen.top/gtpewomfst.html

Ruby: rand(1..100)
来源：http://hz.cqqwz.cn/gtdzslocxt.html

C#:   new Random().Next(1, 101)
来源：http://hz.quarkkingdee.top/gtqpzuwqxz.html

[A11] 条件表达式（三元）
来源：http://hz.hywenlv.cn/gtgofulthj.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.meibo888.top/gtneybfuob.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtweuweejh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtrdpgylpu.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtwebkfkvg.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtlieepcng.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.svipenyu.cn/gtezezgeid.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtpbpxcrzx.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtqniiitgh.html

[A12] 字符串插值 / 格式化
来源：http://hz.jinghuilouyu.cn/gtxbcehhcm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hnxiangtu.top/gtkxuavvka.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhiwuduotai.top/gttammtadm.html

JS:   `Hello, ${name}!`
来源：http://hz.ivvv.top/gttfygfhxh.html

TS:   `Hello, ${name}!`
来源：http://hz.hnxiangtu.top/gtrhmumgaz.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.guowangkeji.top/gtasejrihs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.quarkkingdee.top/gtjwalbvak.html

Ruby: "Hello, #{name}!"
来源：http://hz.mhx1999.top/gtehfznsqf.html

C#:   $"Hello, {name}!"
来源：http://hz.sxryk.cn/gtsuritnka.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.andypj.xyz/gtlpeefahj.html

Py:   "第一行\n第二行"
来源：http://hz.xingfuxueyuan.xyz/gtmuilcpnt.html

PHP:  "第一行\n第二行"
来源：http://hz.nanxinkj.top/gthwhzhwno.html

JS:   "第一行\n第二行"
来源：http://hz.zdqjudy.top/gtautzwxqv.html

TS:   "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtvisbxzbt.html

Java: "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtkxmcfkgb.html

Go:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtdrywkmkg.html

Ruby: "第一行\n第二行"
来源：http://hz.wangdashe.top/gtmawhcubs.html

C#:   "第一行\n第二行"
来源：http://hz.sweek.top/gtsiymcwam.html

[A14] 注释写法
来源：http://hz.ydjk.org.cn/gthifrwmqt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.chenlongwang.top/gtvcekndhl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hywenlv.cn/gtuijprwgo.html

JS:   // 单行；/* 多行 */
来源：http://hz.yj20258888.top/gtabmnuehs.html

TS:   // 单行；/* 多行 */
来源：http://hz.fengsongda.top/gtxldnpmuj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.0kj1m.cn/gtkkmjbrpk.html

Go:   // 单行；/* 多行 */
来源：http://hz.jlsjyb.cn/gtwxtqagzs.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhiwuduotai.top/gtspwyrhlu.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhengqikj.top/gtibzyzgij.html

[A15] 空值判断与默认值
来源：http://hz.cheryme.top/gtrpjtrise.html

Py:   value = data or "默认值"
来源：http://hz.ivvv.top/gtrdxodqpw.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xylfe.cn/gtxzuiggky.html

JS:   const value = data ?? "默认值";
来源：http://hz.ydjk.org.cn/gtcvweosav.html

TS:   const value = data ?? "默认值";
来源：http://hz.kuanghao11.cn/gtejgsydlm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xinyue.icu/gtqizvqmgd.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.pycfn.com/gtkzzgzkye.html

Ruby: value = data || "默认值"
来源：http://hz.shuidangran.top/gtchkheyiu.html

C#:   var value = data ?? "默认值";
来源：http://hz.andypj.xyz/gtccxsmrzb.html

[A16] 真假值判断规则
来源：http://hz.wangdashe.top/gtzswnjpbw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.gogol.net.cn/gtthyiuygu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.316326.xyz/gttjybgapc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.haohaochexian.top/gtocrqpmsp.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtwwvhxvfe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jinqigfzy.top/gtpagaujws.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yuxming.cn/gterioyrye.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhiwuduotai.top/gtlzrqtlzy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hysaishi.cn/gteofkgucf.html

[A17] 位运算
来源：http://hz.xuetiantiany.cn/gtvuilmwkd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtyxpcfntk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinqigfzy.top/gtpdrgcoko.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtazsqunjd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ybcxt.top/gttiwfnuma.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtasesgpcc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtftkpzrvx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtkrgbesvq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.316326.xyz/gtucfzqxzj.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yanxiufei.cn/gtuygkmifn.html

Py:   ord("A"); chr(65)
来源：http://hz.9152youxi.cn/gtirypwust.html

PHP:  ord("A"); chr(65)
来源：http://hz.ppjwa.cn/gtumutcziw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hfpthk.cn/gtxftqilgq.html


<!-- 参考信息 -->