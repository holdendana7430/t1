代发 wailian999

[U105] JS：节流
来源：http://hz.xingfuxueyuan.xyz/gttddyeezr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shangyingyoupin.top/gtuylrpcin.html

[U106] JS：日期格式化
来源：http://hz.wangshuangyany.cn/gtlkjunkdn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sxryk.cn/gtgxbmkgcu.html

[U107] JS：数字千分位
来源：http://hz.jinqigufen.top/gtwthmazgu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtpjbesqok.html

[U108] JS：随机整数
来源：http://hz.bjfxy.top/gtovozqbuv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtzujkiktv.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtqxcvfkhm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gtzqkmapam.html

[U110] JS：数组分块
来源：http://hz.shangyingyoupin.top/gtjkgttqya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.bjfxy.top/gtvfzzpvur.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtbugzvrsg.html

new Map(Object.entries(obj))
来源：http://hz.ehwqpu.com/gtiyhximuz.html

[U112] JS：字符串补位
来源：http://hz.sxryk.cn/gtwkoathsg.html

"7".padStart(3, "0")
来源：http://hz.birdmap.top/gtfipzcmwf.html

[U113] JS：正则替换全部
来源：http://hz.zhaomingkeji.xyz/gtwmeeharh.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gthlnpdzhq.html

[U114] JS：JSON 深比较
来源：http://hz.chenzaomai.com/gtiaxnzlsd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtnotyltdk.html

[U115] JS：生成 UUID
来源：http://hz.hammf.cn/gtfspyoyvt.html

crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtzpnuxjze.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtldiacpcu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigufen.top/gtfglrpfbf.html

[U117] JS：单元测试
来源：http://hz.jinqigfzy.top/gtdjljekdc.html

npm i -D vitest;  npx vitest
来源：http://hz.ivvv.top/gtslulydyh.html

[U118] JS：开发服务器
来源：http://hz.pengpengdd.cyou/gtctktxwbz.html

npm i -D vite;  npx vite
来源：http://hz.havefunace.top/gtplmpnbxs.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gttggwiquh.html

npx vite build
来源：http://hz.pycfn.com/gtcdleawdq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.wangshuangyany.cn/gtqdtolncg.html

import.meta.env.VITE_API_URL
来源：http://hz.wangshuangyany.cn/gtcxzpegwn.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtoiwpxddn.html

统计汇总
来源：http://hz.nwbrower.top/gtnjqagftv.html

================================================================================
来源：http://hz.guannengcc.top/gtaslvkowi.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtlfksdaig.html

Python ......... 252
来源：http://hz.yueranfly.top/gttizevpxh.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtkupnufxc.html

JavaScript ..... 252
来源：http://hz.daxiang520.top/gtkkravayg.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtiupdrgmv.html

Java ........... 212
来源：http://hz.52xcode.cn/gtxtqpiujd.html

Go ............. 212
来源：http://hz.yangfankeji.com/gtchaugnpw.html

Ruby ........... 212
来源：http://hz.jlsjyb.cn/gtyibflvdw.html

C# ............. 212
来源：http://hz.sufxvd.cn/gtuyhxxgux.html

C .............. 30
来源：http://hz.tianlin.xyz/gtokzxllag.html

C++ ............ 30
来源：http://hz.jinqigufen.top/gtqonnczmf.html

SQL ............ 90
来源：http://hz.zhongyouzk.top/gtskmtjuml.html

Bash ........... 80
来源：http://hz.havefunace.top/gtdclinuqs.html

Kotlin ......... 15
来源：http://hz.yangfankeji.com/gtgwgowmqt.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gtnpozvhen.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtbwrzdsxh.html

Perl ........... 10
来源：http://hz.yueranfly.top/gtkzaobptd.html

Scala .......... 10
来源：http://hz.hywenlv.cn/gtmzfoqmcq.html

------------------------------------
来源：http://hz.9152youxi.cn/gteyaxffus.html

合计 ........... 2106 条
来源：http://hz.shuidangran.top/gtyiwvxcgs.html

按章节统计：
来源：http://hz.wangshuangyany.cn/gteaqwgvon.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtxwfmrwcd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtirzjnukt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtfrrstdbp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jiagoushi.top/gtvxalbgci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj202588.top/gtaqwwlaxu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.birdmap.top/gttkjehqdj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtkfimdmrt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtdhbuoxtc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtczobuisa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtbiivipxx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtzssbcpke.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtzsbpnfqf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtvpufofty.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258.top/gtgtxsvoos.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yuxming.cn/gtimhkyneh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtxlcidfal.html

Q SQL 专题                              90
来源：http://hz.hammf.cn/gtssppbnqk.html

R Bash 专题                             80
来源：http://hz.jyoumei.cn/gtuhqguptv.html

S C / C++ 专题                          60
来源：http://hz.jiagoushi.top/gtxszhmckd.html

T 其他语言补充                          60
来源：http://hz.xziqi.cn/gtmzhlgrvd.html

U 高频实用片段                         120
来源：http://hz.yj202588.top/gtaqinivvz.html

------------------------------------
来源：http://hz.yj20258888.top/gtvvywetjy.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtynqlxqti.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtbqwursnx.html

使用提醒
来源：http://hz.nanxuanxn.top/gtzoziltiq.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtuudddeka.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dianchejie.cn/gtdgyyvwyx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.birdmap.top/gtqgwfdlrk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydzc1.top/gtbxtcuaoa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.kuanghao11.cn/gtaiefvwjg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtiizqkump.html

—— 文件结束 ——
来源：http://hz.iojbl.cn/gtzpnpfiap.html

================================================================================
来源：http://hz.xinyue.icu/gtwdeyggfh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuanzhike.top/gtqezzzsji.html

Common Programming Examples Cheat Book
来源：http://hz.52xcode.cn/gtddwpfwaz.html

================================================================================
来源：http://hz.iojbl.cn/gtcrnveljr.html

【收录内容】
来源：http://hz.guannengcc.top/gtddudquxi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hfpthk.cn/gtwjdffrdm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinyuanbaomall.cn/gtyjsjfbim.html

SQL · Bash · C · C++
来源：http://hz.nanxinkj.top/gthsxylhvo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guowangkeji.top/gtrozazrrs.html

【使用说明】
来源：http://hz.nanxuanxn.top/gtlduvjsxy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhongyouzk.top/gtnmstsgqp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yangfankeji.com/gtlodvsjqe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtbktgwmny.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yonumen.top/gtwkssaaub.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yongpay.top/gtpyivsfbv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.52xcode.cn/gtkazoqfle.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinghuilouyu.cn/gtgfmrncyb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigfzy.top/gthosbgeur.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shuidangran.top/gtvvrhrtuy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtntoyrljq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtgngaurdh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ybcxt.top/gtjgbkarre.html

【文件统计】
来源：http://hz.yongpay.top/gttmbhujfl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yueranfly.top/gtdjfnckqc.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtkacmtydk.html

目  录
来源：http://hz.dashuyun.cn/gtvtukzzzv.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtwehypefz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xziqi.cn/gtxekgiccc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shzxlz.cn/gtjurjyukg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtzvgizrjb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtpbxmafhs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cucudq.cn/gtufnioyqi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ywan-chungtsiang.top/gtwgoinckv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtivpzxzmp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tanke756.top/gtwbgjqtby.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtqlgajkyb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj20258888.top/gtjopymflj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtodhvpvin.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtmvegtoho.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtrtausgbs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.dashuyun.cn/gtgpjyxrwh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jianghu66.top/gtvlihpuyk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gthhcxtwki.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cashguo.top/gtldfxileh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.pycfn.com/gtjxmdcywy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ehwqpu.com/gthnavizwy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ehwqpu.com/gtlefuvjzn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gttakshhqm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqbyhqoeh.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtnnikktev.html

================================================================================
来源：http://hz.zhixingplan.top/gtvkqqswwl.html

[A01] Hello World
来源：http://hz.wangdashe.top/gtccnsnzcl.html

Py:   print("Hello, World!")
来源：http://hz.hammf.cn/gtnyngtxxo.html

PHP:  echo "Hello, World!";
来源：http://hz.yvedp.cn/gtypwsdits.html

JS:   console.log("Hello, World!");
来源：http://hz.birdmap.top/gtgdukvpjs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtlcjihlut.html

Java: System.out.println("Hello, World!");
来源：http://hz.vqdsnc.cn/gtycvrevaf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.aibaodan.cn/gtwydhwgla.html

Ruby: puts "Hello, World!"
来源：http://hz.zdqjudy.top/gtpseuqsio.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yonumen.top/gtlzusldtz.html

[A02] 变量声明与赋值
来源：http://hz.zhixingplan.top/gtjwpzxsau.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gzhubu.top/gtfigbxmyv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gtfqshvcpi.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.pengpengdd.cyou/gttdzvuujh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.havefunace.top/gtiodeilvs.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ivvv.top/gtzuocedmc.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinyuanbaomall.cn/gtxsnnmqjh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.bjfxy.top/gtlsypdqpv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cqqwz.cn/gtwrphxdyc.html

[A03] 常量定义
来源：http://hz.shanyushiyangkeji.top/gtdwrsjxra.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gogol.net.cn/gtzovpsjlj.html

PHP:  const PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtpkaqowew.html

JS:   const PI = 3.14159;
来源：http://hz.hnqzz.top/gtppbqwpjm.html

TS:   const PI: number = 3.14159;
来源：http://hz.yvedp.cn/gtjpoojcgg.html

Java: static final double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtdhyujecx.html

Go:   const PI = 3.14159
来源：http://hz.wangdashe.top/gthcjqppav.html

Ruby: PI = 3.14159
来源：http://hz.52xcode.cn/gtdikfdbhi.html

C#:   const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtdzaaaqim.html

[A04] 判断变量类型
来源：http://hz.yangfankeji.com/gthwhzomeo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pycfn.com/gtqewebhll.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.tianlin.xyz/gtltaftdzd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhongyouzk.top/gtsojywpcu.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydzc1.top/gtnypjcvok.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hammf.cn/gthhqibypc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhengqikj.top/gtdlbdbysu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.wangshuangyany.cn/gtlnzgfgfi.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhengqikj.top/gtwaqwouxr.html

[A05] 整数除法与取模
来源：http://hz.daria6918.cn/gtlsbbwude.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhongyouzk.top/gtrsnsfxkl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hywenlv.cn/gtrnpoxqyv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.smart0.xyz/gtvpdnejcf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.52xcode.cn/gtohjqnqvf.html

Java: 7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtlnnoyiwi.html

Go:   7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gtridvsxxq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtpsmxfryk.html

C#:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtchkteawq.html

[A06] 字符串转数字
来源：http://hz.nanxuanxn.top/gthwqwdbvw.html

Py:   int("42"); float("3.14")
来源：http://hz.chenjidiqi.icu/gtdxedimhp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.snrcjt.cn/gthjwhobqh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xylfe.cn/gtzmzqdcii.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.sufxvd.cn/gtitilfdea.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yj20258.top/gtcnjdpvcm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.redwolf501.top/gtwachmzjo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgfzy.top/gtzpsyceer.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.meibo888.top/gtotkynxws.html

[A07] 数字转字符串
来源：http://hz.daxiang520.top/gtapblncll.html

Py:   str(42)
来源：http://hz.ppjwa.cn/gtqgrchicw.html

PHP:  (string) 42; strval(42)
来源：http://hz.haohaochexian.top/gtbrqyqxqk.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigfzy.top/gtzokajoie.html

TS:   String(42)
来源：http://hz.yj202588.top/gtasrlaubq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xylfe.cn/gtjahqansl.html

Go:   strconv.Itoa(42)
来源：http://hz.jianghu66.top/gtgafqhund.html

Ruby: 42.to_s
来源：http://hz.gotoacloud.top/gtebddjgog.html

C#:   42.ToString()
来源：http://hz.gogol.net.cn/gtvbojvyyw.html

[A08] 取整与四舍五入
来源：http://hz.ywan-chungtsiang.top/gtzpjkkwxu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yvedp.cn/gtlicbezeh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xuanzx.com/gtqjzsfgyw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhongyouzk.top/gtlrswjrcw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.vqdsnc.cn/gtwtwrxjel.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gtcepujmag.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cqqwz.cn/gtvnwwkbgl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.52xcode.cn/gtpikbroup.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gzhubu.top/gtzgjkwfxe.html

[A09] 绝对值与最大最小值
来源：http://hz.9152youxi.cn/gtqglnmdea.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinghuilouyu.cn/gtknawomwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guowangkeji.top/gtqugcllsp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.kuanghao11.cn/gtkfclpwpw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnxiangtu.top/gtvyfctiof.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.daria6918.cn/gtqdccibqn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhoulong.xyz/gtokkwbhco.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.9152youxi.cn/gtrhlqmjzv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xylfe.cn/gtxzmnapym.html

[A10] 生成随机数
来源：http://hz.cdnleiting.top/gtqhmxnyyo.html

Py:   import random; random.randint(1, 100)
来源：http://hz.cqqwz.cn/gtvouwqout.html

PHP:  random_int(1, 100);
来源：http://hz.vqdsnc.cn/gtgqicefvw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jlsjyb.cn/gtubpayrpa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shuidangran.top/gtphccalzw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jiagoushi.top/gtowvspjyx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.redwolf501.top/gtixyagfjl.html

Ruby: rand(1..100)
来源：http://hz.wangshuangyany.cn/gtzwogvilm.html

C#:   new Random().Next(1, 101)
来源：http://hz.andypj.xyz/gtvstbxrmr.html

[A11] 条件表达式（三元）
来源：http://hz.feifeiyinyue.top/gteeqaypmm.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jinyuanbaomall.cn/gtvkwamyuz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtexlywvqd.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtlzrakppj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgfzy.top/gtukbxhyoo.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.aizwys.cn/gtpwjeujsw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ivvv.top/gteaksppzu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ivvv.top/gtmbvphjrw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtsapxwpjw.html

[A12] 字符串插值 / 格式化
来源：http://hz.pycfn.com/gtdkudiyil.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.52xcode.cn/gtsynmzubt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhixingplan.top/gtnkfiayqo.html

JS:   `Hello, ${name}!`
来源：http://hz.vqdsnc.cn/gtudayxluv.html

TS:   `Hello, ${name}!`
来源：http://hz.zhixingplan.top/gtnsxbtwun.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.snrcjt.cn/gttgpsrdfn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.dashuyun.cn/gtviqjaagr.html

Ruby: "Hello, #{name}!"
来源：http://hz.ppjwa.cn/gtrpltdpex.html

C#:   $"Hello, {name}!"
来源：http://hz.9152youxi.cn/gtcaadowxj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.birdmap.top/gtnzqqunkp.html

Py:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtchhtwmkk.html

PHP:  "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtbkuojrnw.html

JS:   "第一行\n第二行"
来源：http://hz.aibaodan.cn/gtlkflyfoq.html

TS:   "第一行\n第二行"
来源：http://hz.shanyushiyangkeji.top/gtauhikviu.html

Java: "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtbstuyfhf.html

Go:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtirhcexce.html

Ruby: "第一行\n第二行"
来源：http://hz.tian-w.cn/gtqgrcejyi.html

C#:   "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtxrsqxgsn.html

[A14] 注释写法
来源：http://hz.cheryme.top/gtzgyjaerv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.tian-w.cn/gtxlstfoxy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.gzhubu.top/gtkubwjlgn.html

JS:   // 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtfxyipgcr.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhiwuduotai.top/gtxlcatrug.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.shuidangran.top/gtpneamrnf.html

Go:   // 单行；/* 多行 */
来源：http://hz.ivvv.top/gtekscciah.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jiagoushi.top/gtforaowsp.html

C#:   // 单行；/* 多行 */
来源：http://hz.0kj1m.cn/gtwlzecshx.html

[A15] 空值判断与默认值
来源：http://hz.meibo888.top/gtetubhvpl.html

Py:   value = data or "默认值"
来源：http://hz.jlsjyb.cn/gtkyydvkqr.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.mhx1999.top/gthlvwkrnk.html

JS:   const value = data ?? "默认值";
来源：http://hz.xuetiantiany.cn/gtpzfxwhzi.html

TS:   const value = data ?? "默认值";
来源：http://hz.ydjk.org.cn/gtvbxhotkk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xingfuxueyuan.xyz/gtiqvqhxan.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.dashuyun.cn/gtzeihrxno.html

Ruby: value = data || "默认值"
来源：http://hz.hywenlv.cn/gtyciwancb.html

C#:   var value = data ?? "默认值";
来源：http://hz.wangdashe.top/gtolpkqtgl.html

[A16] 真假值判断规则
来源：http://hz.shanyushiyangtech.top/gtnofzdtvg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.birdmap.top/gtlktagodb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gogol.net.cn/gtbgnbzycx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhongyouzk.top/gtghnunrpy.html

TS:   if (!x) {}
来源：http://hz.yvedp.cn/gtjkjolhfw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.vqdsnc.cn/gtjtczrzdv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.haohaochexian.top/gtszanvhkf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.guannengcc.top/gthwmcumil.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nanxinkj.top/gtewqcamga.html

[A17] 位运算
来源：http://hz.mhx1999.top/gtiatogsft.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgfzy.top/gtrlhccnkb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinqigfzy.top/gteckoocpf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gtyfbqnees.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtwyubnrdb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.andypj.xyz/gtctkmhrqe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtsofafahf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtdsomnxmx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtnlxgvgun.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tian-w.cn/gtnztpqhsa.html

Py:   ord("A"); chr(65)
来源：http://hz.bjfxy.top/gtzuqxuxqw.html

PHP:  ord("A"); chr(65)
来源：http://hz.dianchejie.cn/gtlkidfhpa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xingfuxueyuan.xyz/gtzogcqobp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.snrcjt.cn/gtfoxojyci.html

Java: (int) 'A'; (char) 65
来源：http://hz.hywenlv.cn/gtzgciiqva.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gzhubu.top/gtgwsbxxih.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinqigufen.top/gtcxfphvwf.html


<!-- 参考信息 -->