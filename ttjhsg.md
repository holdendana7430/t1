代发 wailian999

[U105] JS：节流
来源：http://hz.ydjk.org.cn/gtaqihgjse.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xinyue.icu/gtpiuxtzjl.html

[U106] JS：日期格式化
来源：http://hz.guowangkeji.top/gtmzkbhqwy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhaomingkeji.xyz/gtlpraclth.html

[U107] JS：数字千分位
来源：http://hz.daria6918.cn/gtqpcciibm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fzhhl.top/gthznwozdu.html

[U108] JS：随机整数
来源：http://hz.aizwys.cn/gtaofbsyjb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yueranfly.top/gtxzqtbrus.html

[U109] JS：数组分组
来源：http://hz.haohaochexian.top/gtfqnwagoz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtyjwcfzxt.html

[U110] JS：数组分块
来源：http://hz.zhongyouzk.top/gtvruhnnek.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xinyue.icu/gtjulqpijp.html

[U111] JS：对象转 Map
来源：http://hz.hywenlv.cn/gtfqjmntvs.html

new Map(Object.entries(obj))
来源：http://hz.pycfn.com/gtqyuahvgf.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtqyxzbovx.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtqwzevwnp.html

[U113] JS：正则替换全部
来源：http://hz.jqgfzy.top/gtqofkizmb.html

s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtedlbpnos.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gthgydhlzl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtkxvfchcs.html

[U115] JS：生成 UUID
来源：http://hz.jyoumei.cn/gtamymybjg.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtcjbqnmro.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xingfuxueyuan.xyz/gtwbqqcewe.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gthywsoyoe.html

[U117] JS：单元测试
来源：http://hz.52xcode.cn/gtjzyieoqm.html

npm i -D vitest;  npx vitest
来源：http://hz.fzhhl.top/gtrhrzunll.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtfcvotqvn.html

npm i -D vite;  npx vite
来源：http://hz.shuidangran.top/gtsfddfzch.html

[U119] JS：生产构建
来源：http://hz.tanke756.top/gtbridgepg.html

npx vite build
来源：http://hz.chenlongwang.top/gttsxeeizk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dashuyun.cn/gtxjnsdqih.html

import.meta.env.VITE_API_URL
来源：http://hz.jinghuilouyu.cn/gtfzvtarjc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfjxzqdrq.html

统计汇总
来源：http://hz.aibaodan.cn/gtiyebylkw.html

================================================================================
来源：http://hz.sweek.top/gtdjfpzdmq.html

按语言统计（条）：
来源：http://hz.hfpthk.cn/gtasxpotms.html

Python ......... 252
来源：http://hz.pengpengdd.cyou/gtfohjkzca.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtwxdregis.html

JavaScript ..... 252
来源：http://hz.sysykeji.top/gthilodmgd.html

TypeScript ..... 212
来源：http://hz.daria6918.cn/gtovlkmrbm.html

Java ........... 212
来源：http://hz.hywenlv.cn/gtejrahveg.html

Go ............. 212
来源：http://hz.xziqi.cn/gtohvkptru.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtcjkhzyfq.html

C# ............. 212
来源：http://hz.jinyuanbaomall.cn/gtijdlbiaz.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtojsqvbbc.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtmnxnwjle.html

SQL ............ 90
来源：http://hz.jiagoushi.top/gtzqyiyhft.html

Bash ........... 80
来源：http://hz.jlsjyb.cn/gtpsphxpkn.html

Kotlin ......... 15
来源：http://hz.gzhubu.top/gtyulqnjcs.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtuodjlhyl.html

Lua ............ 10
来源：http://hz.aibaodan.cn/gtwywinmuh.html

Perl ........... 10
来源：http://hz.zhijiandao.cn/gtuyxitvig.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtoqlbbhlg.html

------------------------------------
来源：http://hz.ppjwa.cn/gtpyxhbouf.html

合计 ........... 2106 条
来源：http://hz.guowangkeji.top/gtnntboxga.html

按章节统计：
来源：http://hz.fzhhl.top/gtbxwhyvpa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtmjwzjnlc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yongpay.top/gttkrfkuwy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtbgnkpekn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtbwhftngz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtmzmyxlmp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtgnsjbjin.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtpctlpxqk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gthapqymyx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtaavuzrna.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtomfdapnd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gttloxpdiq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtqwqjcnut.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtnvfofpxi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtgkcznubn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sufxvd.cn/gtgbtoeqrr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtlbhpohte.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtuptohzht.html

R Bash 专题                             80
来源：http://hz.ydzc1.top/gtwzawnrbn.html

S C / C++ 专题                          60
来源：http://hz.yuxming.cn/gtsuuvsclj.html

T 其他语言补充                          60
来源：http://hz.gzhubu.top/gtjjiosjvu.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangtech.top/gtdojekfqz.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtqhperrxq.html

合计                                  2106 条
来源：http://hz.shuidangran.top/gtsktzaaoq.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtklkhcacq.html

使用提醒
来源：http://hz.daria6918.cn/gtgytgxtas.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtyglgcxsv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtgqgrnmce.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtkxptcowu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.0kj1m.cn/gtiezxrrhl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jiagoushi.top/gtzsxhznlv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yuanzhike.top/gtxuzaqbfw.html

—— 文件结束 ——
来源：http://hz.hnxiangtu.top/gtlmyhdysy.html

================================================================================
来源：http://hz.yuxming.cn/gtwdegrphy.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuxming.cn/gtltaxqvjx.html

Common Programming Examples Cheat Book
来源：http://hz.yonumen.top/gtzmavehzh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcoyriieu.html

【收录内容】
来源：http://hz.jqgfzy.top/gtalllqwqr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtqfvbgjog.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenlongwang.top/gtwlqulwtc.html

SQL · Bash · C · C++
来源：http://hz.chenlongwang.top/gtxekeybaa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtcvwtoaqv.html

【使用说明】
来源：http://hz.shangyingyoupin.top/gtcskfwqas.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhoulong.xyz/gtzeqezvid.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenzaomai.com/gtcafglojf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhijiandao.cn/gtmzdepdca.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yuxming.cn/gtxdrtvyke.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinyuanbaomall.cn/gtykmedsgw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xuetiantiany.cn/gtgsevtmjg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj202588.top/gtlibvlrik.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hnqzz.top/gtmqgmzson.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinyuanbaomall.cn/gttbxnrijn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hongshengwenyu.top/gtfuynvldi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hysaishi.cn/gtqfdqqezy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.mhx1999.top/gtwwyokmfz.html

【文件统计】
来源：http://hz.shanyushiyangtech.top/gturembxwb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhijiandao.cn/gtxowxtelx.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtetzfpdue.html

目  录
来源：http://hz.jqgfzy.top/gtnbrgqvah.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtarxdeknc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.mhx1999.top/gtgkdqoful.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtdyldlvge.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtfcytqjne.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gthnvqyarj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pengpengdd.cyou/gtoznuzpma.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gtklowhyvc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtqbugdgnq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.wangdashe.top/gtdacacpmn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtnskmdctj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gtyycxvzmq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtlpjkhize.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtitlqueyh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gttpibdphk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tanke756.top/gtaxswnnlo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtebwxjpqy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtuvycdfyx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gotoacloud.top/gtfcszxsvx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.mhx1999.top/gtggfyskdm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhengqikj.top/gtgzoptyln.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtssmfmcel.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.guannengcc.top/gtmbjhnqzd.html

================================================================================
来源：http://hz.shuidangran.top/gtgvagalou.html

A. 基础语法与类型
来源：http://hz.cucudq.cn/gtaxgpglkz.html

================================================================================
来源：http://hz.ybcxt.top/gtmvzlsowo.html

[A01] Hello World
来源：http://hz.shangyingyoupin.top/gtjdcczkic.html

Py:   print("Hello, World!")
来源：http://hz.yanxiufei.cn/gtjuvbzirx.html

PHP:  echo "Hello, World!";
来源：http://hz.sufxvd.cn/gtooapciev.html

JS:   console.log("Hello, World!");
来源：http://hz.gzhubu.top/gtmomiaztf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.c1oappe.top/gtehxzistm.html

Java: System.out.println("Hello, World!");
来源：http://hz.birdmap.top/gtvnlvbqhn.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhijiandao.cn/gtxhuajkgx.html

Ruby: puts "Hello, World!"
来源：http://hz.ydzc1.top/gtfmoxeyle.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cdnleiting.top/gtljalhqyd.html

[A02] 变量声明与赋值
来源：http://hz.zhixingplan.top/gtkquzzqwz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtdostdkwj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtrxvwslrt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gtirjheitd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sufxvd.cn/gtajgoxzed.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtnigcwrpr.html

Go:   name := "Alex"; age := 20
来源：http://hz.redwolf501.top/gtujtfxxwx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnqzz.top/gtwjxyigvk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yuxming.cn/gtvdqewugz.html

[A03] 常量定义
来源：http://hz.hongshengwenyu.top/gtrrzaluvi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hongshengwenyu.top/gtwtklmjau.html

PHP:  const PI = 3.14159;
来源：http://hz.tanke756.top/gtstjivpsd.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gthsorzqmq.html

TS:   const PI: number = 3.14159;
来源：http://hz.9152youxi.cn/gtxpdssypx.html

Java: static final double PI = 3.14159;
来源：http://hz.0kj1m.cn/gtfgryjqlk.html

Go:   const PI = 3.14159
来源：http://hz.yonumen.top/gtysonsfoz.html

Ruby: PI = 3.14159
来源：http://hz.c1oappe.top/gtlzguxvtf.html

C#:   const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtegjtgqaw.html

[A04] 判断变量类型
来源：http://hz.shuidangran.top/gtadzdrycg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.cashguo.top/gtlpvjxgrv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhiwuduotai.top/gtuclzuwms.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhixingplan.top/gtythvbjbr.html

TS:   typeof x; x instanceof Date
来源：http://hz.xziqi.cn/gtxnvtnavj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhiwuduotai.top/gtjdrsgzpp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.c1oappe.top/gtbbwtceme.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nwbrower.top/gtbjvpvjvt.html

C#:   x.GetType().Name; x is int
来源：http://hz.yonumen.top/gtsphzhhra.html

[A05] 整数除法与取模
来源：http://hz.ydjk.org.cn/gtoijacreb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhiwuduotai.top/gtdkiablmo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cdnleiting.top/gtdcigwubl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtemwwhxnt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gogol.net.cn/gtxjrqbltb.html

Java: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtothfmzzi.html

Go:   7 / 2; 7 % 2
来源：http://hz.gzhubu.top/gtfsrbcnnj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtetjbhwfy.html

C#:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtgramritg.html

[A06] 字符串转数字
来源：http://hz.yj20258888.top/gtrmogeaya.html

Py:   int("42"); float("3.14")
来源：http://hz.hnqzz.top/gtainexdux.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gzhubu.top/gthkllhund.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.dashuyun.cn/gtilufwtfl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.kuanghao11.cn/gtvalqaegx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yongpay.top/gtbzjnfhaw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.quarkkingdee.top/gtnoblsjsv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hammf.cn/gtalwncfcu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hywenlv.cn/gtztlworck.html

[A07] 数字转字符串
来源：http://hz.snrcjt.cn/gtlrujqsjj.html

Py:   str(42)
来源：http://hz.jlsjyb.cn/gtibjnxfyz.html

PHP:  (string) 42; strval(42)
来源：http://hz.cashguo.top/gtxzklyqrm.html

JS:   String(42); (42).toString()
来源：http://hz.ydjk.org.cn/gtgionfctz.html

TS:   String(42)
来源：http://hz.daria6918.cn/gtpjiuegnh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhongyouzk.top/gtmnaxvygp.html

Go:   strconv.Itoa(42)
来源：http://hz.yj20258.top/gtflupvtwy.html

Ruby: 42.to_s
来源：http://hz.quarkkingdee.top/gtveqpkglj.html

C#:   42.ToString()
来源：http://hz.sysykeji.top/gtnizqsvbv.html

[A08] 取整与四舍五入
来源：http://hz.yangfankeji.com/gtrtaofwvb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.pengpengdd.cyou/gtnthlswhk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhiwuduotai.top/gtbxrqifyw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yangfankeji.com/gtilwgsuya.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigfzy.top/gtnjamxsoq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.52xcode.cn/gttzzstdbf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hammf.cn/gtvthrgqen.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jiagoushi.top/gtzunqkmmt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.wangdashe.top/gtvfpogufk.html

[A09] 绝对值与最大最小值
来源：http://hz.daria6918.cn/gtzcpzraid.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuxming.cn/gtlihimjeq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sysykeji.top/gtztkqeoqu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hammf.cn/gtaetmxjdh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxuanxn.top/gtriclhtdi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shuidangran.top/gtgsvxkouo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.daria6918.cn/gtyoomezxv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shanyushiyangkeji.top/gtdcjgwrlw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yvedp.cn/gtgbgfxrhu.html

[A10] 生成随机数
来源：http://hz.cqqwz.cn/gtbkckrwwj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sysykeji.top/gtnrufohts.html

PHP:  random_int(1, 100);
来源：http://hz.birdmap.top/gtqigxayyw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zdqjudy.top/gtdgirenix.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhengqikj.top/gtxzglqrmi.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cheryme.top/gtpcvxxrqu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhoulong.xyz/gtwdxyroxo.html

Ruby: rand(1..100)
来源：http://hz.aibaodan.cn/gtwqwiwwal.html

C#:   new Random().Next(1, 101)
来源：http://hz.gzhubu.top/gtrnvgkzhg.html

[A11] 条件表达式（三元）
来源：http://hz.zhijiandao.cn/gtgjichurp.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.feifeiyinyue.top/gtgvqxekyz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtdsyaespr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.cdnleiting.top/gtulotvnaj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtrzldomop.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtjevmuwym.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jinqigufen.top/gthmtlowcd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.wangshuangyany.cn/gttfkzoyny.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtmbyxzkyl.html

[A12] 字符串插值 / 格式化
来源：http://hz.jqgfzy.top/gtprkfwggs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.aibaodan.cn/gtkrcdklmh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhoulong.xyz/gtyeicutiu.html

JS:   `Hello, ${name}!`
来源：http://hz.dashuyun.cn/gtnlmmblrj.html

TS:   `Hello, ${name}!`
来源：http://hz.tanke756.top/gtnfgzifln.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhiwuduotai.top/gtoaeitxry.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinqigfzy.top/gtjjqjszkj.html

Ruby: "Hello, #{name}!"
来源：http://hz.xylfe.cn/gtwqwxonol.html

C#:   $"Hello, {name}!"
来源：http://hz.hfpthk.cn/gtknumexjx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.daxiang520.top/gtmpftmcgw.html

Py:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtkbbztibr.html

PHP:  "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtkvyyuyeu.html

JS:   "第一行\n第二行"
来源：http://hz.jqgufenzy.top/gtssghuntt.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtdktvcwnb.html

Java: "第一行\n第二行"
来源：http://hz.jyoumei.cn/gtdhoiimsz.html

Go:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtiavazsen.html

Ruby: "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtppyqigem.html

C#:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtrpjmuola.html

[A14] 注释写法
来源：http://hz.sweek.top/gtkfggkijr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.tanke756.top/gtesmzbfqg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtzwupbebd.html

JS:   // 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtbpxeqjqy.html

TS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtfmzakgip.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.iojbl.cn/gtxafpbkhi.html

Go:   // 单行；/* 多行 */
来源：http://hz.gogol.net.cn/gtfpigjgpb.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.tanke756.top/gtuayytsbg.html

C#:   // 单行；/* 多行 */
来源：http://hz.iojbl.cn/gtbwknuntz.html

[A15] 空值判断与默认值
来源：http://hz.jyoumei.cn/gtnrzcwrrn.html

Py:   value = data or "默认值"
来源：http://hz.yangfankeji.com/gtqvtrwlln.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtwkirjtud.html

JS:   const value = data ?? "默认值";
来源：http://hz.yueranfly.top/gtlzhhinlq.html

TS:   const value = data ?? "默认值";
来源：http://hz.yuanzhike.top/gtngkxsgzk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ybcxt.top/gtuvxbaadw.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.tanke756.top/gtldrmdtkj.html

Ruby: value = data || "默认值"
来源：http://hz.daxiang520.top/gtqcosnsem.html

C#:   var value = data ?? "默认值";
来源：http://hz.nanxinkj.top/gtgrwgwsfw.html

[A16] 真假值判断规则
来源：http://hz.andypj.xyz/gtvoldrhud.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.sxryk.cn/gtuboonecu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ehwqpu.com/gtmzkarlaj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yueranfly.top/gtwvmznggv.html

TS:   if (!x) {}
来源：http://hz.aibaodan.cn/gtgoohzptf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cdnleiting.top/gtintaoyid.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yongpay.top/gtjcgtzshi.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shuidangran.top/gtyhhjnkeb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nwbrower.top/gteebyiwae.html

[A17] 位运算
来源：http://hz.sysykeji.top/gtdnsaxbhq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtpudvdvvp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.cheryme.top/gtxlpipxct.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuxming.cn/gtmssdcjgc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yvedp.cn/gttfyfpfju.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtpzqtxxfq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtyvsilmkx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtawrzxmni.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtaiomcpkm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinghuilouyu.cn/gtnyjlvvlf.html

Py:   ord("A"); chr(65)
来源：http://hz.shanyushiyangkeji.top/gtfdnwbpsx.html

PHP:  ord("A"); chr(65)
来源：http://hz.feifeiyinyue.top/gtukhhjwgg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtusxejych.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenlongwang.top/gtfkiambqi.html

Java: (int) 'A'; (char) 65
来源：http://hz.tian-w.cn/gteltrkato.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.9152youxi.cn/gtkszauknm.html

Ruby: "A".ord; 65.chr
来源：http://hz.yuanzhike.top/gtgtuzhnoa.html


<!-- 参考信息 -->