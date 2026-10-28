代发 wailian999

[U103] JS：定时器
来源：http://hz.jlsjyb.cn/gtvvnmrpne.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xingfuxueyuan.xyz/gtinpnukbl.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtkpxjoewh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtreneejam.html

[U105] JS：节流
来源：http://hz.jiagoushi.top/gtumufnquw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jyoumei.cn/gtbgfqzhhd.html

[U106] JS：日期格式化
来源：http://hz.hfpthk.cn/gtiwgfftpk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tian-w.cn/gteyvupkfr.html

[U107] JS：数字千分位
来源：http://hz.dianchejie.cn/gtbpnnchns.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtywiwiouu.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gthfqopjey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fzhhl.top/gtnhbwyvia.html

[U109] JS：数组分组
来源：http://hz.vqdsnc.cn/gtdcbzxjso.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtsxmhaucm.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gtswbswhhg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.daxiang520.top/gtazilmmxd.html

[U111] JS：对象转 Map
来源：http://hz.yangfankeji.com/gtxqlrymlo.html

new Map(Object.entries(obj))
来源：http://hz.jyoumei.cn/gtkxozikav.html

[U112] JS：字符串补位
来源：http://hz.xylfe.cn/gtylorxzgn.html

"7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtvjncoahy.html

[U113] JS：正则替换全部
来源：http://hz.kuanghao11.cn/gtrptpjpqj.html

s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtboniudhy.html

[U114] JS：JSON 深比较
来源：http://hz.hnqzz.top/gtkjrstlce.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtzldycmwy.html

[U115] JS：生成 UUID
来源：http://hz.chenjidiqi.icu/gtboilyodi.html

crypto.randomUUID()
来源：http://hz.gzhubu.top/gtjxsmnjlv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gteiartivh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtfnqosvbl.html

[U117] JS：单元测试
来源：http://hz.xuanzx.com/gtfghlwnxi.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtpbdjrvwa.html

[U118] JS：开发服务器
来源：http://hz.aizwys.cn/gteaiqeovr.html

npm i -D vite;  npx vite
来源：http://hz.tanke756.top/gtkhtmozmp.html

[U119] JS：生产构建
来源：http://hz.yuxming.cn/gtjzpsmpwo.html

npx vite build
来源：http://hz.ehwqpu.com/gtkjuncjck.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.pycfn.com/gtycbdsgkz.html

import.meta.env.VITE_API_URL
来源：http://hz.ppjwa.cn/gtxjdlojne.html

================================================================================
来源：http://hz.redwolf501.top/gtruafjosk.html

统计汇总
来源：http://hz.jiagoushi.top/gtkkituyzj.html

================================================================================
来源：http://hz.zhixingplan.top/gtvctkqmuk.html

按语言统计（条）：
来源：http://hz.ehwqpu.com/gtnzmgxlpx.html

Python ......... 252
来源：http://hz.jlsjyb.cn/gtvjstxuxw.html

PHP ............ 252
来源：http://hz.cdnleiting.top/gtqojauvol.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtdnhiqnhs.html

TypeScript ..... 212
来源：http://hz.fzhhl.top/gtnewupxsq.html

Java ........... 212
来源：http://hz.pengpengdd.cyou/gtpzbrvtos.html

Go ............. 212
来源：http://hz.aizwys.cn/gtlbxoziue.html

Ruby ........... 212
来源：http://hz.aizwys.cn/gtixuaesve.html

C# ............. 212
来源：http://hz.dianchejie.cn/gtlimwdcky.html

C .............. 30
来源：http://hz.ppjwa.cn/gtqdanpgdw.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtommxlxty.html

SQL ............ 90
来源：http://hz.kuanghao11.cn/gtmmhkwftf.html

Bash ........... 80
来源：http://hz.hammf.cn/gthltnqbqt.html

Kotlin ......... 15
来源：http://hz.tian-w.cn/gtbcpluytq.html

Swift .......... 15
来源：http://hz.chenlongwang.top/gtfpfavbbh.html

Lua ............ 10
来源：http://hz.yuxming.cn/gtpxbgnyhc.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtaamoznxm.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gttmbwfwmp.html

------------------------------------
来源：http://hz.zhoulong.xyz/gtdfltbshj.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangtech.top/gtnhjhnlbs.html

按章节统计：
来源：http://hz.kuanghao11.cn/gtzdrqmypo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtlnfpguxg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtexuarthy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtokbwzidm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gteerdtlxy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuanzhike.top/gtnnwefcqd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxinkj.top/gtzxebfbnt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtnvmbisfn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtbwibwzte.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtkbkjapkg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtcgkrxiei.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtnoxpjlhl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtplaqfghk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtjrcxtrmq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtflajdkgx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guannengcc.top/gtrifiqjjc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtfbdvaqvu.html

Q SQL 专题                              90
来源：http://hz.xziqi.cn/gtjkbpnaat.html

R Bash 专题                             80
来源：http://hz.tian-w.cn/gthnkyykhm.html

S C / C++ 专题                          60
来源：http://hz.52xcode.cn/gtockyahse.html

T 其他语言补充                          60
来源：http://hz.hywenlv.cn/gteapydoiv.html

U 高频实用片段                         120
来源：http://hz.aibaodan.cn/gteeunfxkr.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtwefrwajz.html

合计                                  2106 条
来源：http://hz.9152youxi.cn/gtzrohtrrs.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtijjafhok.html

使用提醒
来源：http://hz.zhongyouzk.top/gtcgjjrxbm.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtlnhkfonz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tianlin.xyz/gtoofmyfhr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.svipenyu.cn/gtvmlsfxna.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tian-w.cn/gtcialihyu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtptvjrrma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinqigfzy.top/gtujmgircu.html

—— 文件结束 ——
来源：http://hz.xylfe.cn/gtdsljczfc.html

================================================================================
来源：http://hz.xziqi.cn/gthgykmgkl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.snrcjt.cn/gtptjgntyx.html

Common Programming Examples Cheat Book
来源：http://hz.kuanghao11.cn/gtyvsdsrln.html

================================================================================
来源：http://hz.yvedp.cn/gtdjfetxxs.html

【收录内容】
来源：http://hz.fengsongda.top/gtjijdhdnh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.snrcjt.cn/gtnvovkuyi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuanzhike.top/gtfksvjlhx.html

SQL · Bash · C · C++
来源：http://hz.jlsjyb.cn/gtvbcopboo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ywan-chungtsiang.top/gtqngdlmum.html

【使用说明】
来源：http://hz.sufxvd.cn/gtatjjgsui.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj20258888.top/gtwvxmxnef.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.dashuyun.cn/gtwcbdjbbi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ybcxt.top/gtgxyufitw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtrybhdiiv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.birdmap.top/gtdhffnsez.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tian-w.cn/gtiiuebttq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.mhx1999.top/gteeovrjfg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ehwqpu.com/gtmmbohefu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.haohaochexian.top/gtbrgyrbpu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ywan-chungtsiang.top/gthaqnzjdu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.haohaochexian.top/gtklwpfrkx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj20258888.top/gtvwrnmmeo.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtjvhviiho.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ywan-chungtsiang.top/gtmrgjfwvk.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtwrjvyvnt.html

目  录
来源：http://hz.jyoumei.cn/gtmxwyayxn.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtvhuzhsav.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gtmjcizbpb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtqwpteqgh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtdfwxplkf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hysaishi.cn/gthndfnmkg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sweek.top/gtfcoqbsxq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tianlin.xyz/gtjjeqroqa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gttyqlpawd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtcwvimanq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtzohphyui.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gtqqifbnig.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.dashuyun.cn/gtazodinir.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtcjwgkqxn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtiayehtji.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtunlslbtf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxinkj.top/gtsxclimlo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtvnreobhm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.iojbl.cn/gtqlnxkxmj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cdnleiting.top/gtwpvvzbga.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtnkicxnfe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtozhbpvqe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtkbnrfcik.html

================================================================================
来源：http://hz.yuanzhike.top/gtytzujyxi.html

A. 基础语法与类型
来源：http://hz.daxiang520.top/gtsqowcwdl.html

================================================================================
来源：http://hz.hnxiangtu.top/gtzpfgsbtn.html

[A01] Hello World
来源：http://hz.hysaishi.cn/gttsbpuyfl.html

Py:   print("Hello, World!")
来源：http://hz.ivvv.top/gtycfmhwve.html

PHP:  echo "Hello, World!";
来源：http://hz.dianchejie.cn/gtifjdocsh.html

JS:   console.log("Hello, World!");
来源：http://hz.shuidangran.top/gtojyxlwee.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtlqqenqoi.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhaomingkeji.xyz/gtvqrhxlqk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hfpthk.cn/gtznqjzobj.html

Ruby: puts "Hello, World!"
来源：http://hz.hywenlv.cn/gtonfmxjai.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sufxvd.cn/gtrhkfgxje.html

[A02] 变量声明与赋值
来源：http://hz.hongshengwenyu.top/gtdpaoqndw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jlsjyb.cn/gtavuuoncu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yanxiufei.cn/gtwogpqdyh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.9152youxi.cn/gtbrszfgoy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhixingplan.top/gtzjmjvpdr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gtuzpcmbqe.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtstuxbjzp.html

Ruby: name = "Alex"; age = 20
来源：http://hz.tian-w.cn/gtnvjhlkry.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gogol.net.cn/gtlosmpkxx.html

[A03] 常量定义
来源：http://hz.nanxuanxn.top/gtcekawieq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.havefunace.top/gtrwxapzgg.html

PHP:  const PI = 3.14159;
来源：http://hz.pycfn.com/gtqmkdvhnn.html

JS:   const PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtqnbalhii.html

TS:   const PI: number = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtddiwelfw.html

Java: static final double PI = 3.14159;
来源：http://hz.guannengcc.top/gtbfpvifqk.html

Go:   const PI = 3.14159
来源：http://hz.jianghu66.top/gtsqdxoxos.html

Ruby: PI = 3.14159
来源：http://hz.ydzc1.top/gtddovcrmt.html

C#:   const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtswxyaiyb.html

[A04] 判断变量类型
来源：http://hz.hnqzz.top/gtpehqrydl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shzxlz.cn/gtgchhcnmk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.c1oappe.top/gtoehlpcva.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xuetiantiany.cn/gtlgmfmtld.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhongyouzk.top/gtiomsmrni.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xinyue.icu/gttbawprgd.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuxming.cn/gtjmjxxxqj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jqgufenzy.top/gteppfvcbj.html

C#:   x.GetType().Name; x is int
来源：http://hz.gogol.net.cn/gtwcwjhlyi.html

[A05] 整数除法与取模
来源：http://hz.cucudq.cn/gtpznmqmgm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hnxiangtu.top/gtgfeqxjvy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.tian-w.cn/gtxusruizs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtnsjjdejv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.316326.xyz/gtpucngnrt.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtcyxpvhck.html

Go:   7 / 2; 7 % 2
来源：http://hz.kuanghao11.cn/gtkjagsnmp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtmdqzpvqs.html

C#:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtkgqprggf.html

[A06] 字符串转数字
来源：http://hz.zhoulong.xyz/gtjldakuqt.html

Py:   int("42"); float("3.14")
来源：http://hz.zhixingplan.top/gtlkvybiim.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.meibo888.top/gtoaflhfsh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.meibo888.top/gtolwkvgcn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xziqi.cn/gtgplzhehd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenlongwang.top/gtppivvvms.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gtnsveixce.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinyuanbaomall.cn/gtmyumknwz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtpufyydgv.html

[A07] 数字转字符串
来源：http://hz.jinyuanbaomall.cn/gterdfympb.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtmidbabqh.html

PHP:  (string) 42; strval(42)
来源：http://hz.andypj.xyz/gtuvdchdkw.html

JS:   String(42); (42).toString()
来源：http://hz.wangshuangyany.cn/gtajpaaroy.html

TS:   String(42)
来源：http://hz.yuanzhike.top/gtasrjdeve.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jyoumei.cn/gtahotyayq.html

Go:   strconv.Itoa(42)
来源：http://hz.hnqzz.top/gtbfgpiadl.html

Ruby: 42.to_s
来源：http://hz.ydzc1.top/gtjaypjxsc.html

C#:   42.ToString()
来源：http://hz.birdmap.top/gtcsdrdilw.html

[A08] 取整与四舍五入
来源：http://hz.xinyue.icu/gtixqhkivk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xziqi.cn/gtqxrafyoj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jyoumei.cn/gtqboubmmf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.52xcode.cn/gtcranqpqk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.316326.xyz/gtqppfknjf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ppjwa.cn/gtgflbdzsq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xuanzx.com/gtnpygqsnk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.iojbl.cn/gtvfauduwd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.birdmap.top/gtrynylnpj.html

[A09] 绝对值与最大最小值
来源：http://hz.andypj.xyz/gtmwwbdusn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yangfankeji.com/gthnowsgfy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xylfe.cn/gtksywyeqm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.aibaodan.cn/gtrfwgidyl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtcdrwzcgb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jyoumei.cn/gtflnjyotc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.daxiang520.top/gtaimpvvoq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jinyuanbaomall.cn/gtxhuyipku.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.316326.xyz/gtgaiwzucu.html

[A10] 生成随机数
来源：http://hz.guannengcc.top/gtoukkwrps.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zdqjudy.top/gtlhkiiikq.html

PHP:  random_int(1, 100);
来源：http://hz.redwolf501.top/gtapjspbik.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gttakwxpxk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.chenzaomai.com/gtdkgamnez.html

Java: new Random().nextInt(100) + 1
来源：http://hz.snrcjt.cn/gtynenzzzm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hnqzz.top/gtgxfprfwu.html

Ruby: rand(1..100)
来源：http://hz.yj20258.top/gtqenwuykr.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj202588.top/gthcqireap.html

[A11] 条件表达式（三元）
来源：http://hz.zhoulong.xyz/gtluscawob.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.daria6918.cn/gtpncnvqgg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtoivzbjwm.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtnoonotgh.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtrqkpgkgm.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtnslxmeqx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.chenlongwang.top/gtmlxmmvdo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtgvrmfogm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gtrzqynvwt.html

[A12] 字符串插值 / 格式化
来源：http://hz.tianlin.xyz/gtwqmuwlxq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yonumen.top/gticqqqtlj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yueranfly.top/gtbvrslbci.html

JS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gttzevbwdm.html

TS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gtokdnpoqo.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.vqdsnc.cn/gtcdfymyfp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.andypj.xyz/gtproldnen.html

Ruby: "Hello, #{name}!"
来源：http://hz.jiagoushi.top/gtwzjbxorv.html

C#:   $"Hello, {name}!"
来源：http://hz.iojbl.cn/gtcgrxqjyy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yj202588.top/gthxvlwatn.html

Py:   "第一行\n第二行"
来源：http://hz.wangdashe.top/gthhsvfmtk.html

PHP:  "第一行\n第二行"
来源：http://hz.sysykeji.top/gtnfkrlvvd.html

JS:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtmjohoogd.html

TS:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtpdjzrafi.html

Java: "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtdtspmrvz.html

Go:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtghkmktob.html

Ruby: "第一行\n第二行"
来源：http://hz.shzxlz.cn/gtwvkeepbm.html

C#:   "第一行\n第二行"
来源：http://hz.c1oappe.top/gtqcalxcfc.html

[A14] 注释写法
来源：http://hz.fzhhl.top/gtratzcwnn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.nanxuanxn.top/gtyuxsmmds.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yj20258888.top/gtyjdjsshw.html

JS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtgmdfzmgg.html

TS:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gtuzvfrtpu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.tian-w.cn/gtoqglwnsw.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtyucuathv.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yueranfly.top/gtrwmxbfzb.html

C#:   // 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtogkxcilw.html

[A15] 空值判断与默认值
来源：http://hz.daxiang520.top/gtaqbsqfqp.html

Py:   value = data or "默认值"
来源：http://hz.ehwqpu.com/gtrqtfyzwz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yangfankeji.com/gtjxqxuqmm.html

JS:   const value = data ?? "默认值";
来源：http://hz.shzxlz.cn/gtfkzqzvqt.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinghuilouyu.cn/gtrputiebz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.chenlongwang.top/gtzqbkzhvk.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jqgufenzy.top/gtdkkanwwt.html

Ruby: value = data || "默认值"
来源：http://hz.zdqjudy.top/gtfeuwwrwv.html

C#:   var value = data ?? "默认值";
来源：http://hz.snrcjt.cn/gtpbwvjocs.html

[A16] 真假值判断规则
来源：http://hz.yj20258888.top/gtctrjcojp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.nanxinkj.top/gtdkefumkz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.hammf.cn/gtmecaubdi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.feifeiyinyue.top/gtzzvluvvm.html

TS:   if (!x) {}
来源：http://hz.cqqwz.cn/gtvqvidswe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sysykeji.top/gtougbtetf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yvedp.cn/gtczjfetna.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jyoumei.cn/gtpizrzgbz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zycfv.cn/gtikepwsuh.html

[A17] 位运算
来源：http://hz.yj202588.top/gtjfbviaae.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtbewhkyrj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shangyingyoupin.top/gtkxohbbnk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtycqjkdps.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtqzpilpns.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gttrvzirbl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gtejanzaif.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gthresfzfk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtbtekfbfh.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhixingplan.top/gtthogfrqt.html

Py:   ord("A"); chr(65)
来源：http://hz.jyoumei.cn/gtibmlzupj.html

PHP:  ord("A"); chr(65)
来源：http://hz.dianchejie.cn/gtpolpxasf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.guannengcc.top/gtlbthwrvy.html


<!-- 参考信息 -->