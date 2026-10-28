代发 wailian999

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtczdhljgu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258.top/gtkhmccdim.html

[U106] JS：日期格式化
来源：http://hz.iojbl.cn/gtvszajgzp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shangyingyoupin.top/gtfuwqewaz.html

[U107] JS：数字千分位
来源：http://hz.snrcjt.cn/gtqnikbzek.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtdeimwebr.html

[U108] JS：随机整数
来源：http://hz.cheryme.top/gtwbjydszp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgfzy.top/gtboudavpo.html

[U109] JS：数组分组
来源：http://hz.yangfankeji.com/gtmobxlfyn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtuwwqgwxl.html

[U110] JS：数组分块
来源：http://hz.chenzaomai.com/gtycfbxrnd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.meibo888.top/gtabdwbbmn.html

[U111] JS：对象转 Map
来源：http://hz.hfpthk.cn/gtjoshpoil.html

new Map(Object.entries(obj))
来源：http://hz.cdnleiting.top/gtwnheibzr.html

[U112] JS：字符串补位
来源：http://hz.hysaishi.cn/gtreifzgtu.html

"7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtgwnkxgrh.html

[U113] JS：正则替换全部
来源：http://hz.52xcode.cn/gtzsgsgolf.html

s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtggbiztgh.html

[U114] JS：JSON 深比较
来源：http://hz.cheryme.top/gtymjtnuch.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtrabwhyti.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtjyagoqwn.html

crypto.randomUUID()
来源：http://hz.xinyue.icu/gteewkmtka.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cqqwz.cn/gticitmkxr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydjk.org.cn/gtdwqzvhvw.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtmpkeubyx.html

npm i -D vitest;  npx vitest
来源：http://hz.nwbrower.top/gtgbpxvusf.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtqrcugbhl.html

npm i -D vite;  npx vite
来源：http://hz.guannengcc.top/gtzcvluhfm.html

[U119] JS：生产构建
来源：http://hz.ybcxt.top/gtsqugxgzd.html

npx vite build
来源：http://hz.ppjwa.cn/gtygchfchc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinghuilouyu.cn/gtpavuvgqz.html

import.meta.env.VITE_API_URL
来源：http://hz.daxiang520.top/gtrtzojmaf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttcktjrlq.html

统计汇总
来源：http://hz.cucudq.cn/gtitmiyaau.html

================================================================================
来源：http://hz.tian-w.cn/gtxqghoixo.html

按语言统计（条）：
来源：http://hz.ydjk.org.cn/gtbudvxvha.html

Python ......... 252
来源：http://hz.hammf.cn/gtxbrxedtu.html

PHP ............ 252
来源：http://hz.jyoumei.cn/gtazljbghx.html

JavaScript ..... 252
来源：http://hz.guowangkeji.top/gtdplgngvq.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtxjevvzsr.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtbrrcaqeu.html

Go ............. 212
来源：http://hz.tian-w.cn/gtkhlnwmhy.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtttyjlegy.html

C# ............. 212
来源：http://hz.cucudq.cn/gtezgqgshg.html

C .............. 30
来源：http://hz.yuanzhike.top/gtqpqjfoha.html

C++ ............ 30
来源：http://hz.fengsongda.top/gtpeocqybl.html

SQL ............ 90
来源：http://hz.cheryme.top/gtecqqbnhn.html

Bash ........... 80
来源：http://hz.iojbl.cn/gttrwjbgva.html

Kotlin ......... 15
来源：http://hz.hongshengwenyu.top/gtbzpitshe.html

Swift .......... 15
来源：http://hz.9152youxi.cn/gtgcqhbvog.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gtnkdkaooj.html

Perl ........... 10
来源：http://hz.aizwys.cn/gtrvxpldwi.html

Scala .......... 10
来源：http://hz.xuetiantiany.cn/gtzffabfuo.html

------------------------------------
来源：http://hz.daria6918.cn/gtwbpsmbwy.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtzikkscxl.html

按章节统计：
来源：http://hz.9152youxi.cn/gtrdfxcjhd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtbutoevne.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gtgegbknrv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtfhwsgayb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtjwozagsb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xuanzx.com/gtksisabzc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.9152youxi.cn/gtpdgopjvz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtvoylfveg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtwtwsebqm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtbjujzyqi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gtowczvqrv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtcgfjflse.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtygmekpct.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtibecpyqh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gttzmigbdf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daria6918.cn/gtmieunbfg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtbagmyetj.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gtpbcmselm.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtdoyvwkgg.html

S C / C++ 专题                          60
来源：http://hz.jlsjyb.cn/gtvenxnkdl.html

T 其他语言补充                          60
来源：http://hz.ydzc1.top/gtilknsdvf.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtdqzrnofx.html

------------------------------------
来源：http://hz.guowangkeji.top/gtaksasgpp.html

合计                                  2106 条
来源：http://hz.yangfankeji.com/gtqdmavtio.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtpllqmvej.html

使用提醒
来源：http://hz.zhijiandao.cn/gtderzkfza.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtpkgrwvmu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuxming.cn/gtznapcwxp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cheryme.top/gtzxhcjger.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.guannengcc.top/gtzoxomnoc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ehwqpu.com/gtinuatvmm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.havefunace.top/gtxzmwcytp.html

—— 文件结束 ——
来源：http://hz.daria6918.cn/gtzktqawld.html

================================================================================
来源：http://hz.zhijiandao.cn/gthjyptevp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xuetiantiany.cn/gtpwvguysc.html

Common Programming Examples Cheat Book
来源：http://hz.nanxuanxn.top/gtmrmmjrik.html

================================================================================
来源：http://hz.daria6918.cn/gtxibewbkd.html

【收录内容】
来源：http://hz.snrcjt.cn/gtirrtverg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.316326.xyz/gtbawoxxkn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gaohongyu789.top/gtsgplcnux.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gtfndetlcs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.birdmap.top/gttndwtlal.html

【使用说明】
来源：http://hz.sysykeji.top/gtdgbtcagu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.fengsongda.top/gtgvrrubqu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xuetiantiany.cn/gthkfxovdm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jlsjyb.cn/gtdhynmrfz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shangyingyoupin.top/gtzlrsgtip.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.smart0.xyz/gtzsuogvmm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tian-w.cn/gtlsawfjsy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangkeji.top/gtsqqphhdr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sweek.top/gtuvsxeqij.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtjbimqlib.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gotoacloud.top/gtusvbzeqq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnxiangtu.top/gtewwcrdho.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.bjfxy.top/gtaefxcvsq.html

【文件统计】
来源：http://hz.xinyue.icu/gtggubpkmd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxinkj.top/gtfwpakynm.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gthyxnbdad.html

目  录
来源：http://hz.nanxinkj.top/gtxnluaacy.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtlgpstjkf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtllqbecxk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtjdiqhgmo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtxflhggnz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtqkptjbrt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yueranfly.top/gtlmxcavrc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.daria6918.cn/gtgofpjrxd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtohugvrmc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtmxkhefoz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtzzjrxoyy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shuidangran.top/gttxtvuiyh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtqzvpsela.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtfeaezdvb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtjwnruexi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtkkwiclvr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sysykeji.top/gtgonlvuae.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtylxbczkz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gzhubu.top/gtbglvmqrg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hysaishi.cn/gtowbekkag.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.guannengcc.top/gtnqzhzqqi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gthgvosyrh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtlhpoiwix.html

================================================================================
来源：http://hz.guannengcc.top/gtwksxjybn.html

A. 基础语法与类型
来源：http://hz.ehwqpu.com/gtdqaxmlzz.html

================================================================================
来源：http://hz.redwolf501.top/gtapugjiuo.html

[A01] Hello World
来源：http://hz.chenjidiqi.icu/gtktixzbcg.html

Py:   print("Hello, World!")
来源：http://hz.nanxuanxn.top/gtipejimbk.html

PHP:  echo "Hello, World!";
来源：http://hz.sxryk.cn/gtzlpldiza.html

JS:   console.log("Hello, World!");
来源：http://hz.smart0.xyz/gtnbmxfeuk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gttlhvozat.html

Java: System.out.println("Hello, World!");
来源：http://hz.pengpengdd.cyou/gteejfuvoz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhijiandao.cn/gtkpyoxyfz.html

Ruby: puts "Hello, World!"
来源：http://hz.sxryk.cn/gtailoigmg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sufxvd.cn/gtnthwbnzk.html

[A02] 变量声明与赋值
来源：http://hz.cucudq.cn/gtffvdavpm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cheryme.top/gthjabmjnq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuanzhike.top/gtxjimoisp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.52xcode.cn/gtiecgrefl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.birdmap.top/gtseeieozj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.tanke756.top/gtmdscdzui.html

Go:   name := "Alex"; age := 20
来源：http://hz.daxiang520.top/gtpbariltl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.dianchejie.cn/gtgjjqzgty.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.redwolf501.top/gtjgtfzkbl.html

[A03] 常量定义
来源：http://hz.daria6918.cn/gtpavvpyyd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.316326.xyz/gtqnnhsawk.html

PHP:  const PI = 3.14159;
来源：http://hz.yueranfly.top/gttcgyzaiz.html

JS:   const PI = 3.14159;
来源：http://hz.tianlin.xyz/gtercipjfr.html

TS:   const PI: number = 3.14159;
来源：http://hz.haohaochexian.top/gtqknqqgkm.html

Java: static final double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtujasjtvy.html

Go:   const PI = 3.14159
来源：http://hz.gogol.net.cn/gtuyvhkqjd.html

Ruby: PI = 3.14159
来源：http://hz.chenzaomai.com/gtizdxpbsa.html

C#:   const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtwhlxefyy.html

[A04] 判断变量类型
来源：http://hz.ehwqpu.com/gtilpvqdel.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jqgufenzy.top/gtatrkrazc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258.top/gtvmvliloe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shzxlz.cn/gtqyixmtwe.html

TS:   typeof x; x instanceof Date
来源：http://hz.jlsjyb.cn/gtjfwvowry.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xingfuxueyuan.xyz/gtcgydypcg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nwbrower.top/gtibxitjym.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yanxiufei.cn/gtnslhtekf.html

C#:   x.GetType().Name; x is int
来源：http://hz.svipenyu.cn/gtqdmjusxl.html

[A05] 整数除法与取模
来源：http://hz.gzhubu.top/gtdnsawbvn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cucudq.cn/gtnxnyfbdt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtajduhxdu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.havefunace.top/gtfiwdhalw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.kuanghao11.cn/gtinmocvtc.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtwwcvrzrs.html

Go:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtpevoqvcq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xinyue.icu/gtlmzwxtes.html

C#:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtulamceph.html

[A06] 字符串转数字
来源：http://hz.zycfv.cn/gtkcgxjjxk.html

Py:   int("42"); float("3.14")
来源：http://hz.hysaishi.cn/gtkxridwbn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.dashuyun.cn/gtarymydhf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jqgufenzy.top/gtexgqfeea.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xylfe.cn/gtnkwbxjxp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jianghu66.top/gtkrnxbwjt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.wangdashe.top/gtraekydrj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.guowangkeji.top/gteagsjkmr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.havefunace.top/gtymkvhafm.html

[A07] 数字转字符串
来源：http://hz.tanke756.top/gtmmxzrpat.html

Py:   str(42)
来源：http://hz.chenjidiqi.icu/gttbeobnqw.html

PHP:  (string) 42; strval(42)
来源：http://hz.yvedp.cn/gtuqcdjevz.html

JS:   String(42); (42).toString()
来源：http://hz.andypj.xyz/gtndjelcvh.html

TS:   String(42)
来源：http://hz.yj202588.top/gtrzkwffcx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.fengsongda.top/gtuzinccco.html

Go:   strconv.Itoa(42)
来源：http://hz.ppjwa.cn/gtbmrpzdzp.html

Ruby: 42.to_s
来源：http://hz.ehwqpu.com/gtouciedyv.html

C#:   42.ToString()
来源：http://hz.yj20258.top/gtbywdafvq.html

[A08] 取整与四舍五入
来源：http://hz.zhixingplan.top/gtzhlehgaa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.wangshuangyany.cn/gttayodtgw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hnqzz.top/gtblouctvn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.aizwys.cn/gtshzrphwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigfzy.top/gtybtovesy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yj20258888.top/gtuivahiip.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.c1oappe.top/gtaqrvxstm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cqqwz.cn/gthwzfurec.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yvedp.cn/gtbvvlgfgp.html

[A09] 绝对值与最大最小值
来源：http://hz.tanke756.top/gtjconnceo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.fzhhl.top/gtktlyxkfr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.c1oappe.top/gtzezugitb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtqctljqoj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gtyymvlfxx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhixingplan.top/gtbfrzkxas.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cdnleiting.top/gtyqptyizo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.daxiang520.top/gtqgywjgwx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xylfe.cn/gtcwmpgryo.html

[A10] 生成随机数
来源：http://hz.shuidangran.top/gtvkyovuiq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xuetiantiany.cn/gtopaxoqtr.html

PHP:  random_int(1, 100);
来源：http://hz.sysykeji.top/gtwnxgjtdx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.quarkkingdee.top/gtgzjaagtv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.dianchejie.cn/gtkihqrmqq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.shzxlz.cn/gtaylqibiq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jyoumei.cn/gtxqblxolo.html

Ruby: rand(1..100)
来源：http://hz.yj20258888.top/gtgkqhtwcd.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuanzhike.top/gttjkugwfs.html

[A11] 条件表达式（三元）
来源：http://hz.yueranfly.top/gtpgkfqhmm.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.tian-w.cn/gtziriefne.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtqzasenrk.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gtmwvxmkde.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gzhubu.top/gtrjrotlct.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gteiqusyim.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yj20258.top/gtakdegpfm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gttdqdsadq.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jyoumei.cn/gtzplaeypi.html

[A12] 字符串插值 / 格式化
来源：http://hz.yj20258.top/gtlurbqyjy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.cqqwz.cn/gtjnoccsph.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.cheryme.top/gtkrwdizfw.html

JS:   `Hello, ${name}!`
来源：http://hz.jlsjyb.cn/gtnxcjrtug.html

TS:   `Hello, ${name}!`
来源：http://hz.shzxlz.cn/gtqomnampg.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jinyuanbaomall.cn/gtqhdjbkqb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hywenlv.cn/gtycuhzryb.html

Ruby: "Hello, #{name}!"
来源：http://hz.tanke756.top/gtdvczljek.html

C#:   $"Hello, {name}!"
来源：http://hz.daxiang520.top/gtpmyqjjjq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.snrcjt.cn/gttdzzgwyy.html

Py:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtefdmhgyz.html

PHP:  "第一行\n第二行"
来源：http://hz.zycfv.cn/gtmymbjjak.html

JS:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtooqaqaqp.html

TS:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtofqsijzp.html

Java: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtkihohear.html

Go:   "第一行\n第二行"
来源：http://hz.sweek.top/gtrgeemjxu.html

Ruby: "第一行\n第二行"
来源：http://hz.ivvv.top/gtbnymadgo.html

C#:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtnsjiriur.html

[A14] 注释写法
来源：http://hz.nanxuanxn.top/gtwszldksg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhengqikj.top/gtlfkivgks.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtcpfrzyty.html

JS:   // 单行；/* 多行 */
来源：http://hz.birdmap.top/gtlrupqhao.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtgdfvkhxz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.wangshuangyany.cn/gtsjbqppwi.html

Go:   // 单行；/* 多行 */
来源：http://hz.cheryme.top/gtqeceedaa.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jyoumei.cn/gtgilkejet.html

C#:   // 单行；/* 多行 */
来源：http://hz.yongpay.top/gtdjvpnglw.html

[A15] 空值判断与默认值
来源：http://hz.yj20258.top/gtfmxnuexh.html

Py:   value = data or "默认值"
来源：http://hz.hysaishi.cn/gttgbvuskd.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.daxiang520.top/gtlpjgvanv.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhaomingkeji.xyz/gttbzhrber.html

TS:   const value = data ?? "默认值";
来源：http://hz.hywenlv.cn/gtvprycgpl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yonumen.top/gtbrmydbju.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.sweek.top/gtwvafthpt.html

Ruby: value = data || "默认值"
来源：http://hz.ywan-chungtsiang.top/gtcavjpqmz.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhongyouzk.top/gtetngbgfn.html

[A16] 真假值判断规则
来源：http://hz.jlsjyb.cn/gteaifvmis.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.mhx1999.top/gtzxwxukrg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zhixingplan.top/gtjgmnljwj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenzaomai.com/gtugsmbfva.html

TS:   if (!x) {}
来源：http://hz.zhixingplan.top/gtonkmkdgg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.smart0.xyz/gtzetkjzan.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ehwqpu.com/gtbuioaren.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.haohaochexian.top/gtjcbgemjx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nwbrower.top/gtpoogpwfk.html

[A17] 位运算
来源：http://hz.ydjk.org.cn/gtxyijzxxv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtfzanaeic.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258888.top/gtpsatgtfr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtvduebupk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtlhldoudz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtwmyfobfe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtnxacsdoh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtbdryqzqc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtamjgdznt.html

[A18] 字符与 ASCII 码互转
来源：http://hz.feifeiyinyue.top/gtwzcvbicp.html

Py:   ord("A"); chr(65)
来源：http://hz.cdnleiting.top/gtvpvnntwf.html

PHP:  ord("A"); chr(65)
来源：http://hz.jyoumei.cn/gtonnrvzrr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sxryk.cn/gtzxvoqeqq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtirddzlel.html

Java: (int) 'A'; (char) 65
来源：http://hz.ehwqpu.com/gtkzgqlskk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.snrcjt.cn/gtjxhxqztd.html

Ruby: "A".ord; 65.chr
来源：http://hz.chenlongwang.top/gtfjvxhrdm.html


<!-- 参考信息 -->