代发 wailian999

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtgsyxzegs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.quarkkingdee.top/gtzycnskmd.html

[U106] JS：日期格式化
来源：http://hz.birdmap.top/gtgigatpyo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.feifeiyinyue.top/gtmlnafswb.html

[U107] JS：数字千分位
来源：http://hz.hnqzz.top/gteuhzoqvf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtsciyuyle.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtwnkhufwh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtmobwiuhm.html

[U109] JS：数组分组
来源：http://hz.vqdsnc.cn/gtsyrsrnvl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hfpthk.cn/gtaoymlhqw.html

[U110] JS：数组分块
来源：http://hz.gotoacloud.top/gtiomauidn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.snrcjt.cn/gtzwczaftd.html

[U111] JS：对象转 Map
来源：http://hz.andypj.xyz/gtqizetpuv.html

new Map(Object.entries(obj))
来源：http://hz.wangdashe.top/gtcqmcquip.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtfspzusui.html

"7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtgjwxlzgy.html

[U113] JS：正则替换全部
来源：http://hz.xziqi.cn/gtyaxigdui.html

s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtgeqhwgnv.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258888.top/gthoxdwiol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtyszzomem.html

[U115] JS：生成 UUID
来源：http://hz.xuetiantiany.cn/gtchcwvmjc.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gtpuxzxtqt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.havefunace.top/gtshpajzgo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xziqi.cn/gtuhljmirg.html

[U117] JS：单元测试
来源：http://hz.gaohongyu789.top/gtctmhaicr.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtayvnmcni.html

[U118] JS：开发服务器
来源：http://hz.xingfuxueyuan.xyz/gtglkttdvs.html

npm i -D vite;  npx vite
来源：http://hz.cheryme.top/gtmedmucfo.html

[U119] JS：生产构建
来源：http://hz.ywan-chungtsiang.top/gtlzbzrijp.html

npx vite build
来源：http://hz.ybcxt.top/gtkjgjtlca.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.snrcjt.cn/gtcdvxalpp.html

import.meta.env.VITE_API_URL
来源：http://hz.jinqigfzy.top/gtipejdudu.html

================================================================================
来源：http://hz.haohaochexian.top/gtpjtztnjv.html

统计汇总
来源：http://hz.jyoumei.cn/gtsddrhgdy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsmbzsnbm.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtfshkktmm.html

Python ......... 252
来源：http://hz.yuanzhike.top/gtpjxyjkxy.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gtalqehmhp.html

JavaScript ..... 252
来源：http://hz.sxryk.cn/gtzehpilqg.html

TypeScript ..... 212
来源：http://hz.daria6918.cn/gtdpsderds.html

Java ........... 212
来源：http://hz.jianghu66.top/gtknbkusis.html

Go ............. 212
来源：http://hz.jianghu66.top/gtsiibkbbm.html

Ruby ........... 212
来源：http://hz.havefunace.top/gthqyofpbw.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtibshqlbd.html

C .............. 30
来源：http://hz.ppjwa.cn/gthrwptudn.html

C++ ............ 30
来源：http://hz.zycfv.cn/gtvwlpypsl.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtufdkwebd.html

Bash ........... 80
来源：http://hz.cdnleiting.top/gtuxevnnhk.html

Kotlin ......... 15
来源：http://hz.feifeiyinyue.top/gtgtdleypy.html

Swift .......... 15
来源：http://hz.sysykeji.top/gtrfprvrss.html

Lua ............ 10
来源：http://hz.nanxinkj.top/gtdiboibwf.html

Perl ........... 10
来源：http://hz.xinyue.icu/gtjhriiway.html

Scala .......... 10
来源：http://hz.sysykeji.top/gtflnbriym.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtofqohooi.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gtqfepprum.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtnqqmpkxk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtqrxgssgk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtgwserpsf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yongpay.top/gttzytttuq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtzgcejutc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinqigfzy.top/gthqklpgjk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hnqzz.top/gtkmqrgygr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtapchduym.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtmygvvrkk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtyaqspvpk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtbndicamj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtbhfadnxj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gteikvgyia.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtcyxccsxs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtzwgjslim.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gotoacloud.top/gtgzfydbic.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtgcuyczhe.html

Q SQL 专题                              90
来源：http://hz.aibaodan.cn/gtpbgjefit.html

R Bash 专题                             80
来源：http://hz.zhongyouzk.top/gtjjwlffes.html

S C / C++ 专题                          60
来源：http://hz.yongpay.top/gtckvlxzzl.html

T 其他语言补充                          60
来源：http://hz.pengpengdd.cyou/gtxznakzbt.html

U 高频实用片段                         120
来源：http://hz.shuidangran.top/gtjzjwfpxd.html

------------------------------------
来源：http://hz.haohaochexian.top/gtuwrpxvef.html

合计                                  2106 条
来源：http://hz.jyoumei.cn/gtikmovtgh.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtbevvrlyi.html

使用提醒
来源：http://hz.andypj.xyz/gtmzfqynpn.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtemcjvkik.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangshuangyany.cn/gtowwwlnqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnxiangtu.top/gtfdclfrdf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.iojbl.cn/gtmacttkea.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.snrcjt.cn/gtbiipjunp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtdthmfcec.html

—— 文件结束 ——
来源：http://hz.jinyuanbaomall.cn/gtkbkflhzk.html

================================================================================
来源：http://hz.hammf.cn/gtfnbdlhqz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shanyushiyangkeji.top/gttnjgdaxn.html

Common Programming Examples Cheat Book
来源：http://hz.birdmap.top/gtztzktzqg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzxswmapb.html

【收录内容】
来源：http://hz.nwbrower.top/gtogcotdxm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtgftsqyzv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zycfv.cn/gtkeidgziw.html

SQL · Bash · C · C++
来源：http://hz.cheryme.top/gtvwkzruvn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shzxlz.cn/gtqcydhfwd.html

【使用说明】
来源：http://hz.shanyushiyangtech.top/gtxleiswnt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cdnleiting.top/gtckbdadnn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yongpay.top/gtrnymhduq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhixingplan.top/gtbcztpjya.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gtgaanayqt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.iojbl.cn/gtnunnuzmv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jlsjyb.cn/gtqdrtmmon.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hammf.cn/gttfsjgnkd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj20258888.top/gtufmsoiae.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cqqwz.cn/gtbvxurhcy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gtwngjwgmj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xuanzx.com/gthuvvuctn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jyoumei.cn/gtmsfkowaf.html

【文件统计】
来源：http://hz.sysykeji.top/gtgztgombb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pycfn.com/gtfuzteqqb.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtyqwnscjj.html

目  录
来源：http://hz.yonumen.top/gtyqccwlsb.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtdgmhpgrn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtjnrdcqha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtspgoycqj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtolxmrugh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtbfclalxh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fengsongda.top/gtgnocsjag.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gthcbdnezw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtsdpnymbt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xuanzx.com/gtswjlqlyd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtgqerpmwq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtpaxogfru.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtatjqorod.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtzmhpcabs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtbvlfrjlb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shzxlz.cn/gtrnzemadi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.mhx1999.top/gthufbuwwi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gthgvqrjla.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sxryk.cn/gtuxkaqngb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xziqi.cn/gtfunozxsw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tian-w.cn/gtfwiqwawp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtvayiymkw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gtsxkevojm.html

================================================================================
来源：http://hz.cucudq.cn/gtdaemqnch.html

A. 基础语法与类型
来源：http://hz.tanke756.top/gtgnmzooyg.html

================================================================================
来源：http://hz.ehwqpu.com/gtvnwexsor.html

[A01] Hello World
来源：http://hz.jlsjyb.cn/gtoazwvdip.html

Py:   print("Hello, World!")
来源：http://hz.zhaomingkeji.xyz/gtefvtutjs.html

PHP:  echo "Hello, World!";
来源：http://hz.cdnleiting.top/gtxvqerfck.html

JS:   console.log("Hello, World!");
来源：http://hz.zhoulong.xyz/gtztbpgszi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xinyue.icu/gtcabbrbkg.html

Java: System.out.println("Hello, World!");
来源：http://hz.aibaodan.cn/gtfngqbgdj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yonumen.top/gtelmgdydt.html

Ruby: puts "Hello, World!"
来源：http://hz.jqgfzy.top/gtrpbybbyv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hysaishi.cn/gtyrjgosxm.html

[A02] 变量声明与赋值
来源：http://hz.jinqigufen.top/gtunuytymg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhengqikj.top/gtepmcuxqu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtqvgqzkem.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hammf.cn/gtzcyefmnt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhaomingkeji.xyz/gtjiidnzyr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yonumen.top/gttdkikzra.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenzaomai.com/gtgdmjrhof.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhijiandao.cn/gtoawlhydr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtcjmptzay.html

[A03] 常量定义
来源：http://hz.wangshuangyany.cn/gtofqarkle.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yvedp.cn/gtrcwuhnmt.html

PHP:  const PI = 3.14159;
来源：http://hz.zycfv.cn/gteuswrpsw.html

JS:   const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtjnfagnzq.html

TS:   const PI: number = 3.14159;
来源：http://hz.birdmap.top/gtzlkxupmf.html

Java: static final double PI = 3.14159;
来源：http://hz.hammf.cn/gthdusqtmw.html

Go:   const PI = 3.14159
来源：http://hz.yanxiufei.cn/gthgvionhd.html

Ruby: PI = 3.14159
来源：http://hz.yueranfly.top/gtzypdapqm.html

C#:   const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtxfiqplzq.html

[A04] 判断变量类型
来源：http://hz.yj20258888.top/gtjgjrqkei.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.smart0.xyz/gtameiadsu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtyjtlkoax.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zycfv.cn/gtqyewxjpv.html

TS:   typeof x; x instanceof Date
来源：http://hz.redwolf501.top/gtnxxmzwcj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.chenzaomai.com/gtqrzrlidv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hfpthk.cn/gtwuelvnig.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuxming.cn/gtywzvdcdz.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj20258888.top/gtnflpybkq.html

[A05] 整数除法与取模
来源：http://hz.gogol.net.cn/gthbxmgmhx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.havefunace.top/gtjqjmhxyg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.haohaochexian.top/gtnkaprlyt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtaxzqborp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yangfankeji.com/gtzbrlslua.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhijiandao.cn/gtofbssfoc.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtqelflmfl.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtrbrzyvoe.html

C#:   7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gthdvujymg.html

[A06] 字符串转数字
来源：http://hz.yueranfly.top/gtvyucgozw.html

Py:   int("42"); float("3.14")
来源：http://hz.guowangkeji.top/gthxsasbbg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.bjfxy.top/gtvfkkljwu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cdnleiting.top/gttewmvfvu.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.316326.xyz/gtdtcgdsdu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nwbrower.top/gtahdmrodv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj202588.top/gtnnvssius.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinyuanbaomall.cn/gthiawyykl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hnqzz.top/gtklokjohj.html

[A07] 数字转字符串
来源：http://hz.gzhubu.top/gtrhsktirx.html

Py:   str(42)
来源：http://hz.zhiwuduotai.top/gtwdhoncib.html

PHP:  (string) 42; strval(42)
来源：http://hz.jinyuanbaomall.cn/gtupxdujrl.html

JS:   String(42); (42).toString()
来源：http://hz.wangshuangyany.cn/gtlzcmiwtt.html

TS:   String(42)
来源：http://hz.ydjk.org.cn/gtbviahunk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.svipenyu.cn/gtbkmypqgr.html

Go:   strconv.Itoa(42)
来源：http://hz.nanxinkj.top/gthegfndie.html

Ruby: 42.to_s
来源：http://hz.mhx1999.top/gtomqxrtzj.html

C#:   42.ToString()
来源：http://hz.jinqigufen.top/gtqshexnld.html

[A08] 取整与四舍五入
来源：http://hz.cashguo.top/gtskpombiz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtaxwsqreo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yangfankeji.com/gtranzvcrx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtrbeshixn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.feifeiyinyue.top/gtpoyfspal.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yanxiufei.cn/gtkhixdhul.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.shanyushiyangtech.top/gtgicgfjdi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.snrcjt.cn/gtzghydqhq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj20258888.top/gthyczdjfv.html

[A09] 绝对值与最大最小值
来源：http://hz.quarkkingdee.top/gtpvqafjtc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangshuangyany.cn/gtktoyotym.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hnxiangtu.top/gtsuvtdaxt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hongshengwenyu.top/gtfdfjimvl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhixingplan.top/gtxbiieaqf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jyoumei.cn/gtdvvlixio.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zycfv.cn/gtamfwtdbh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tanke756.top/gtmjyzjiyq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenjidiqi.icu/gtkzoxktjl.html

[A10] 生成随机数
来源：http://hz.ppjwa.cn/gtajyqtpce.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jiagoushi.top/gthrnbcvjs.html

PHP:  random_int(1, 100);
来源：http://hz.9152youxi.cn/gtioxomccs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.guowangkeji.top/gtrgvvvuyt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ehwqpu.com/gtukrndyyh.html

Java: new Random().nextInt(100) + 1
来源：http://hz.mhx1999.top/gtovcuygcf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xingfuxueyuan.xyz/gtyzxtrkfi.html

Ruby: rand(1..100)
来源：http://hz.guowangkeji.top/gtffqsdjqf.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinqigufen.top/gtlxymbxzi.html

[A11] 条件表达式（三元）
来源：http://hz.yj202588.top/gtltuivimd.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.dashuyun.cn/gtgvxuqzbq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtsqavviin.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gttenjxwub.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.svipenyu.cn/gtgsgycplz.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtdbtyjaet.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.havefunace.top/gtxhdfzmes.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gthgfamwjd.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.guowangkeji.top/gtyibzamxh.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhaomingkeji.xyz/gtblrhvtpq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.ppjwa.cn/gtkyerogst.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.nanxuanxn.top/gtuptptzmw.html

JS:   `Hello, ${name}!`
来源：http://hz.gotoacloud.top/gttoxkniiv.html

TS:   `Hello, ${name}!`
来源：http://hz.hnxiangtu.top/gtzmdmqwmn.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jlsjyb.cn/gtkxzzspdb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.svipenyu.cn/gtzctooyiy.html

Ruby: "Hello, #{name}!"
来源：http://hz.ybcxt.top/gtajrefhvo.html

C#:   $"Hello, {name}!"
来源：http://hz.0kj1m.cn/gtsjqmfjvz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.pycfn.com/gthstogqgp.html

Py:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtpxvgerup.html

PHP:  "第一行\n第二行"
来源：http://hz.daxiang520.top/gtasnjmsoi.html

JS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtoslxugor.html

TS:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtwmpmctsu.html

Java: "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtgefpqayb.html

Go:   "第一行\n第二行"
来源：http://hz.cheryme.top/gtneesmndg.html

Ruby: "第一行\n第二行"
来源：http://hz.yuxming.cn/gtmrzeqqds.html

C#:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gtchhhvjpj.html

[A14] 注释写法
来源：http://hz.quarkkingdee.top/gtjfxcdfcv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.haohaochexian.top/gtqxvuxlgm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yuxming.cn/gtvyafnrhw.html

JS:   // 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtqpjwqzzy.html

TS:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtunqitgmp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.9152youxi.cn/gtszwofbrg.html

Go:   // 单行；/* 多行 */
来源：http://hz.xziqi.cn/gtpgwsvonj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.sweek.top/gtynlacltv.html

C#:   // 单行；/* 多行 */
来源：http://hz.haohaochexian.top/gtusquzckm.html

[A15] 空值判断与默认值
来源：http://hz.zhixingplan.top/gtcnvtdabf.html

Py:   value = data or "默认值"
来源：http://hz.zdqjudy.top/gtwvlnpfic.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.aibaodan.cn/gthrfofupe.html

JS:   const value = data ?? "默认值";
来源：http://hz.shzxlz.cn/gtdoetqktw.html

TS:   const value = data ?? "默认值";
来源：http://hz.jianghu66.top/gtpuzwqjyw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yuanzhike.top/gtiflnrkcx.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhaomingkeji.xyz/gttnlmjkjw.html

Ruby: value = data || "默认值"
来源：http://hz.yonumen.top/gtbnnqetei.html

C#:   var value = data ?? "默认值";
来源：http://hz.sxryk.cn/gtnphrwhek.html

[A16] 真假值判断规则
来源：http://hz.zhaomingkeji.xyz/gtkmotiuth.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yvedp.cn/gtuumoautj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.tianlin.xyz/gtdfufbhhs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ppjwa.cn/gtyngwoqcr.html

TS:   if (!x) {}
来源：http://hz.nanxinkj.top/gtniyohlqm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yueranfly.top/gtjyxcwmys.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ppjwa.cn/gttuqrrzgn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jqgfzy.top/gtozvheqtb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ivvv.top/gtjnxpuked.html

[A17] 位运算
来源：http://hz.wangdashe.top/gtikvxzftc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangkeji.top/gtpuygtxcf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gtdapsndbf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtgkmjschv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nanxinkj.top/gtnkwlgktj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtgvzwixmr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtxpxenklo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtgfoaxeyo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtocwigfax.html

[A18] 字符与 ASCII 码互转
来源：http://hz.shangyingyoupin.top/gtkhknzskp.html

Py:   ord("A"); chr(65)
来源：http://hz.xuanzx.com/gtldeojbud.html

PHP:  ord("A"); chr(65)
来源：http://hz.tianlin.xyz/gtpoygwofb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.guannengcc.top/gtzbphvult.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.guowangkeji.top/gtehapkxyd.html

Java: (int) 'A'; (char) 65
来源：http://hz.fzhhl.top/gtdsjphuzb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yj20258.top/gtkfvbdqey.html

Ruby: "A".ord; 65.chr
来源：http://hz.hysaishi.cn/gtnukvbozr.html


<!-- 参考信息 -->