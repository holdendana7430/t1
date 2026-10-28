代发 wailian999

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtqarnqcni.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gtdkkcnitz.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gtuvmaxboo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtwdpxfdsp.html

[U105] JS：节流
来源：http://hz.zhengqikj.top/gtrjmlwlvy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cheryme.top/gtwqrdektr.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtiajpaowr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinyuanbaomall.cn/gtxtyoqrzl.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtvrjhimtt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nwbrower.top/gtpiewrlah.html

[U108] JS：随机整数
来源：http://hz.hywenlv.cn/gttpagzllq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jianghu66.top/gtxtcczaea.html

[U109] JS：数组分组
来源：http://hz.guannengcc.top/gtsvqpuzer.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gthspqmjia.html

[U110] JS：数组分块
来源：http://hz.chenzaomai.com/gtfhsletll.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtcacrzkah.html

[U111] JS：对象转 Map
来源：http://hz.xinyue.icu/gthujvnguq.html

new Map(Object.entries(obj))
来源：http://hz.ppjwa.cn/gtjglrndqw.html

[U112] JS：字符串补位
来源：http://hz.wangshuangyany.cn/gtqaqjfbzr.html

"7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtxvxgjhsy.html

[U113] JS：正则替换全部
来源：http://hz.svipenyu.cn/gtwkgnddlc.html

s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtmsbltdtt.html

[U114] JS：JSON 深比较
来源：http://hz.redwolf501.top/gtzzjdsovb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gthybmsizz.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtkmbcxsvi.html

crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtoiqyajqe.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gtrbhqvhcw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.52xcode.cn/gtzrnqtiuq.html

[U117] JS：单元测试
来源：http://hz.meibo888.top/gtvertyhbr.html

npm i -D vitest;  npx vitest
来源：http://hz.shzxlz.cn/gtblyupzkd.html

[U118] JS：开发服务器
来源：http://hz.316326.xyz/gtiriyqemc.html

npm i -D vite;  npx vite
来源：http://hz.nanxuanxn.top/gtunzqeyri.html

[U119] JS：生产构建
来源：http://hz.52xcode.cn/gtkkpnhjae.html

npx vite build
来源：http://hz.pycfn.com/gtwhkjcjhd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtxjwwlfik.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangkeji.top/gtavwitszf.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjftllneb.html

统计汇总
来源：http://hz.zhoulong.xyz/gtwjpinnaw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtejrnlbbz.html

按语言统计（条）：
来源：http://hz.chenjidiqi.icu/gtoxgxcyht.html

Python ......... 252
来源：http://hz.haohaochexian.top/gtnmpxrpgt.html

PHP ............ 252
来源：http://hz.zhengqikj.top/gtbyqlyvwh.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtalwedbsl.html

TypeScript ..... 212
来源：http://hz.jiagoushi.top/gtidkurdxt.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtyfsjshdt.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtbmkvpslz.html

Ruby ........... 212
来源：http://hz.zhijiandao.cn/gtrdcdoujh.html

C# ............. 212
来源：http://hz.jlsjyb.cn/gtszdizemw.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gtqjibmncd.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtfjbxhdeh.html

SQL ............ 90
来源：http://hz.daria6918.cn/gtdeupynjp.html

Bash ........... 80
来源：http://hz.hnqzz.top/gtyzsdxfpn.html

Kotlin ......... 15
来源：http://hz.tianlin.xyz/gtnislptyn.html

Swift .......... 15
来源：http://hz.guowangkeji.top/gtzfplbsfy.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtsoinzckq.html

Perl ........... 10
来源：http://hz.chenlongwang.top/gtlezxmplz.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtykxaecae.html

------------------------------------
来源：http://hz.xylfe.cn/gtkxqsvniw.html

合计 ........... 2106 条
来源：http://hz.yvedp.cn/gtfaqknmfb.html

按章节统计：
来源：http://hz.ppjwa.cn/gtebyzukdp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yanxiufei.cn/gtgnaxloyz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtljushseh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtfcyzsoit.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cqqwz.cn/gtqokgxocf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xylfe.cn/gtisjqjpct.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tian-w.cn/gtuwrcjdpj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtxvhmzgnt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtgabnzmnx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtmtjatiym.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinqigufen.top/gtjefffsvu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtgiiyortx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtlfuuuphh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtcdazhtpp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ydzc1.top/gtbjgbwlff.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.vqdsnc.cn/gtxlwcyemo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtypeuthtm.html

Q SQL 专题                              90
来源：http://hz.jyoumei.cn/gtruhwtwzs.html

R Bash 专题                             80
来源：http://hz.meibo888.top/gtvsesslpa.html

S C / C++ 专题                          60
来源：http://hz.snrcjt.cn/gtoblerary.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gtssakwpjf.html

U 高频实用片段                         120
来源：http://hz.feifeiyinyue.top/gtkeaafrhl.html

------------------------------------
来源：http://hz.sufxvd.cn/gtaknlkppg.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtjpgzzfbc.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtilpppzok.html

使用提醒
来源：http://hz.cheryme.top/gtxfflgjjx.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtjhrsxszr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhijiandao.cn/gtynjniowe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hfpthk.cn/gttoorxvxh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.kuanghao11.cn/gtrvvipyqo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gzhubu.top/gtvotkazel.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.andypj.xyz/gtsaalzanh.html

—— 文件结束 ——
来源：http://hz.yuanzhike.top/gttarlllzn.html

================================================================================
来源：http://hz.chenlongwang.top/gtcrgcxcad.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtkgztmjrb.html

Common Programming Examples Cheat Book
来源：http://hz.yuxming.cn/gtidnjdqlz.html

================================================================================
来源：http://hz.haohaochexian.top/gtuybbblig.html

【收录内容】
来源：http://hz.mhx1999.top/gtltpsibdd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.redwolf501.top/gtxkmhmfqj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.9152youxi.cn/gtbvnnxacg.html

SQL · Bash · C · C++
来源：http://hz.hysaishi.cn/gtlacwaagq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ybcxt.top/gtjrtfgkuo.html

【使用说明】
来源：http://hz.gaohongyu789.top/gtnhxciizu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gtfhyfzsto.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.smart0.xyz/gtkrhozlyk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sweek.top/gtcqrbsqhr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yvedp.cn/gtsoigehok.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shuidangran.top/gtxhptzbel.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dashuyun.cn/gtrrakxnbs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sufxvd.cn/gtrksbxcih.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtfrbvdzum.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xinyue.icu/gtszbhlprh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jianghu66.top/gtddjcmrhi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xingfuxueyuan.xyz/gtzfyagewq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tanke756.top/gtqwmjfloi.html

【文件统计】
来源：http://hz.chenzaomai.com/gtenzupkzm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhiwuduotai.top/gtdficeifo.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gttylmuedy.html

目  录
来源：http://hz.pycfn.com/gtfselbfom.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtprvccrmk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nwbrower.top/gtqezhomlg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.fengsongda.top/gtotzpqueh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtgrtzgyoz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yonumen.top/gtdembbicx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yvedp.cn/gttomwwzaj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shangyingyoupin.top/gtelzyspya.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtaqbwvoxa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zycfv.cn/gttjvfjisy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtllmoxlwk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.nanxinkj.top/gtwxahzkiy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtiyuungsr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtrfktmopn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jqgfzy.top/gtydtmvofi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtckuqshcy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hnqzz.top/gtnfryqbiq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtrlcugqoy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.meibo888.top/gtejzqqaxb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.feifeiyinyue.top/gtbemyctjx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gzhubu.top/gtlwozplhc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtxgzyrtib.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtqfneqqid.html

================================================================================
来源：http://hz.wangdashe.top/gtojeumosu.html

A. 基础语法与类型
来源：http://hz.zhoulong.xyz/gtfaakimip.html

================================================================================
来源：http://hz.ivvv.top/gttwehcizz.html

[A01] Hello World
来源：http://hz.zhoulong.xyz/gtbtmpfeid.html

Py:   print("Hello, World!")
来源：http://hz.cqqwz.cn/gtrynpgeia.html

PHP:  echo "Hello, World!";
来源：http://hz.chenzaomai.com/gtlwiuktkc.html

JS:   console.log("Hello, World!");
来源：http://hz.sweek.top/gtnkmjrmkp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shangyingyoupin.top/gtgmipogui.html

Java: System.out.println("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtjvtfeyaf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xuetiantiany.cn/gtotyvpnfp.html

Ruby: puts "Hello, World!"
来源：http://hz.bjfxy.top/gtonaufrmq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.bjfxy.top/gtxduoqkpd.html

[A02] 变量声明与赋值
来源：http://hz.feifeiyinyue.top/gtwdwhwile.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhoulong.xyz/gtuwjatgae.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinqigfzy.top/gtxyuentan.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.wangshuangyany.cn/gtxnadkmqa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.aibaodan.cn/gtlsgkcuik.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnqzz.top/gtbrpavstw.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtoijbxaii.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jianghu66.top/gtsowrrxyz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sweek.top/gtotuomkau.html

[A03] 常量定义
来源：http://hz.ehwqpu.com/gtatmpqdnb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenzaomai.com/gteqpirxsp.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258.top/gtpdctkmdx.html

JS:   const PI = 3.14159;
来源：http://hz.aizwys.cn/gtcinwmvjs.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnqzz.top/gtipinsfhh.html

Java: static final double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtggjpnrlh.html

Go:   const PI = 3.14159
来源：http://hz.daria6918.cn/gteeavoaoh.html

Ruby: PI = 3.14159
来源：http://hz.tanke756.top/gtrwikzmng.html

C#:   const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtrpxdjpda.html

[A04] 判断变量类型
来源：http://hz.hnxiangtu.top/gtdjdqzffk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jqgfzy.top/gtxujapflo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sxryk.cn/gtfyxgmzgz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ivvv.top/gtuohmllah.html

TS:   typeof x; x instanceof Date
来源：http://hz.aizwys.cn/gtneowlapv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.iojbl.cn/gtuydzrxjv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ywan-chungtsiang.top/gtlhqyacpc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.smart0.xyz/gtcmqqqxuw.html

C#:   x.GetType().Name; x is int
来源：http://hz.cheryme.top/gtyqgovnvu.html

[A05] 整数除法与取模
来源：http://hz.ehwqpu.com/gtspulvadi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj20258888.top/gtsydlxoft.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtfqpiumqc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258888.top/gtxalpkmss.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtdihkobuf.html

Java: 7 / 2; 7 % 2
来源：http://hz.meibo888.top/gtxdtewnei.html

Go:   7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gtvldejkud.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gttaisiqol.html

C#:   7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtcbituvmy.html

[A06] 字符串转数字
来源：http://hz.smart0.xyz/gtdlzvizpl.html

Py:   int("42"); float("3.14")
来源：http://hz.52xcode.cn/gtpwgjixfe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.quarkkingdee.top/gtblpjwdji.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ehwqpu.com/gtfggahfac.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhongyouzk.top/gtuupwcqjw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shanyushiyangkeji.top/gtewmydvdx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.fengsongda.top/gtgmntwwhd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.snrcjt.cn/gtotatunpe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gaohongyu789.top/gtitygxmtl.html

[A07] 数字转字符串
来源：http://hz.0kj1m.cn/gtvgaavsch.html

Py:   str(42)
来源：http://hz.ehwqpu.com/gttyboiazf.html

PHP:  (string) 42; strval(42)
来源：http://hz.mhx1999.top/gtabbhcamy.html

JS:   String(42); (42).toString()
来源：http://hz.hnqzz.top/gtpnnxmdtj.html

TS:   String(42)
来源：http://hz.gzhubu.top/gtgstnggtl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.chenzaomai.com/gtagsnufks.html

Go:   strconv.Itoa(42)
来源：http://hz.xylfe.cn/gtzjznxgyq.html

Ruby: 42.to_s
来源：http://hz.smart0.xyz/gtzoneasuc.html

C#:   42.ToString()
来源：http://hz.hysaishi.cn/gtftiwajpg.html

[A08] 取整与四舍五入
来源：http://hz.tanke756.top/gtkustqjtf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yongpay.top/gtimocaeqy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cheryme.top/gtcxhzyzql.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sxryk.cn/gtqeuxixae.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.feifeiyinyue.top/gtzbtbagci.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yueranfly.top/gtgfxbtomn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.52xcode.cn/gtxrbsbimu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.wangdashe.top/gtfitepwll.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.redwolf501.top/gtxbgdrnlp.html

[A09] 绝对值与最大最小值
来源：http://hz.gaohongyu789.top/gtvzieevsi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.kuanghao11.cn/gtyatghoxa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hammf.cn/gtagibqvnv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.316326.xyz/gtrfzvgnls.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.haohaochexian.top/gthnvczwcz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hysaishi.cn/gtglhggrsx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cheryme.top/gtifabfvrx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xingfuxueyuan.xyz/gtwomrfyqb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtjvapdgfj.html

[A10] 生成随机数
来源：http://hz.52xcode.cn/gtzwzrhjeg.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sysykeji.top/gtxnsivwnr.html

PHP:  random_int(1, 100);
来源：http://hz.yuanzhike.top/gtchenhrmi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.quarkkingdee.top/gtodxckxjl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.guannengcc.top/gtrdlrxuhl.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinghuilouyu.cn/gtluvdcgos.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xingfuxueyuan.xyz/gtjysrenkc.html

Ruby: rand(1..100)
来源：http://hz.xuanzx.com/gtksdceara.html

C#:   new Random().Next(1, 101)
来源：http://hz.shanyushiyangkeji.top/gtliddmtln.html

[A11] 条件表达式（三元）
来源：http://hz.bjfxy.top/gtdflpxqso.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtvrkgokcy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.quarkkingdee.top/gtrupmtoeo.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gtvarrweyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jianghu66.top/gtzpnkyktu.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gttshzgmnq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gzhubu.top/gtgnnqzlzr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtdmkkzqzp.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtwbfnbhqt.html

[A12] 字符串插值 / 格式化
来源：http://hz.hysaishi.cn/gtvwfazeyc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.ydzc1.top/gtakilyekd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.smart0.xyz/gtbsiocpca.html

JS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gtifldamvp.html

TS:   `Hello, ${name}!`
来源：http://hz.xuetiantiany.cn/gtgpvanlzk.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.gogol.net.cn/gttemqehgt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.dianchejie.cn/gtzxtyviqz.html

Ruby: "Hello, #{name}!"
来源：http://hz.jyoumei.cn/gtcomwrbwd.html

C#:   $"Hello, {name}!"
来源：http://hz.zycfv.cn/gthcznqoga.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jianghu66.top/gtiqhqjccd.html

Py:   "第一行\n第二行"
来源：http://hz.nanxuanxn.top/gttyrojdvq.html

PHP:  "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtpgjjlcav.html

JS:   "第一行\n第二行"
来源：http://hz.redwolf501.top/gtbnzihquk.html

TS:   "第一行\n第二行"
来源：http://hz.xuanzx.com/gtzegqmgmm.html

Java: "第一行\n第二行"
来源：http://hz.daria6918.cn/gttgsadhjm.html

Go:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtlvgonzqu.html

Ruby: "第一行\n第二行"
来源：http://hz.gotoacloud.top/gtqpydmliv.html

C#:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtwfqgbmlm.html

[A14] 注释写法
来源：http://hz.cashguo.top/gtzauccsch.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.nwbrower.top/gtgbkwoucy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtmfbmrlvr.html

JS:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtwdrbzwdg.html

TS:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gtmfrsrtqz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.feifeiyinyue.top/gtzarheluv.html

Go:   // 单行；/* 多行 */
来源：http://hz.yuxming.cn/gtlzrlofko.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hnqzz.top/gtrnfvurlb.html

C#:   // 单行；/* 多行 */
来源：http://hz.iojbl.cn/gtpongummb.html

[A15] 空值判断与默认值
来源：http://hz.shanyushiyangtech.top/gtaarwsqzh.html

Py:   value = data or "默认值"
来源：http://hz.sweek.top/gtjcparswt.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.quarkkingdee.top/gtdjxdkoha.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhixingplan.top/gtofdhjsyd.html

TS:   const value = data ?? "默认值";
来源：http://hz.yj20258.top/gtjonstart.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hnqzz.top/gtivphmxnl.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhixingplan.top/gtehxoancm.html

Ruby: value = data || "默认值"
来源：http://hz.yonumen.top/gtmmcvrqld.html

C#:   var value = data ?? "默认值";
来源：http://hz.tanke756.top/gtlyrcgxcu.html

[A16] 真假值判断规则
来源：http://hz.gzhubu.top/gtpkxaybkg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zhiwuduotai.top/gtepkmfqza.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.svipenyu.cn/gtslvnqbgl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ybcxt.top/gtbfvhfsal.html

TS:   if (!x) {}
来源：http://hz.hywenlv.cn/gtenzjtqti.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hnqzz.top/gtnbahlcuc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.feifeiyinyue.top/gtgtlgvbmx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.tianlin.xyz/gttwhblvwh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.redwolf501.top/gtgvkogkzb.html

[A17] 位运算
来源：http://hz.hywenlv.cn/gtqcgvgolw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtnedscpfx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.chenzaomai.com/gteopngudv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtlgdgrmrs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtjwkrhyan.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yongpay.top/gtoncxnnmk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtoeyjcdrc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtodgouwhf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtfdqgplbf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fzhhl.top/gtpagailts.html

Py:   ord("A"); chr(65)
来源：http://hz.kuanghao11.cn/gtztnhxaui.html

PHP:  ord("A"); chr(65)
来源：http://hz.tian-w.cn/gtpjjxgvym.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gogol.net.cn/gtzgyxudnw.html


<!-- 参考信息 -->