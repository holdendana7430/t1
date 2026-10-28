代发 wailian999

[U103] JS：定时器
来源：http://hz.ehwqpu.com/gtqzancgtf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gzhubu.top/gtkadsczii.html

[U104] JS：防抖
来源：http://hz.daxiang520.top/gtotvzxhvq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtuxthqdvb.html

[U105] JS：节流
来源：http://hz.smart0.xyz/gttthlwvsk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.redwolf501.top/gtlqkshbcg.html

[U106] JS：日期格式化
来源：http://hz.fengsongda.top/gtrlgnowxc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gthyuigoqz.html

[U107] JS：数字千分位
来源：http://hz.yuxming.cn/gtfiuduxcq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cdnleiting.top/gtxflcujve.html

[U108] JS：随机整数
来源：http://hz.wangdashe.top/gtjsiabsqs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xziqi.cn/gtidvejvgj.html

[U109] JS：数组分组
来源：http://hz.yanxiufei.cn/gtmglvwkgd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gttloxmteo.html

[U110] JS：数组分块
来源：http://hz.cdnleiting.top/gtbmcfmzjs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hysaishi.cn/gthhrzhrjy.html

[U111] JS：对象转 Map
来源：http://hz.316326.xyz/gtfrsrvuuh.html

new Map(Object.entries(obj))
来源：http://hz.xuetiantiany.cn/gtjhyqdqwz.html

[U112] JS：字符串补位
来源：http://hz.yonumen.top/gtmfstrjlt.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gttapgkagc.html

[U113] JS：正则替换全部
来源：http://hz.aizwys.cn/gtcoqyporo.html

s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtrrvzlwfv.html

[U114] JS：JSON 深比较
来源：http://hz.zhengqikj.top/gtfbhffklc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtznjociko.html

[U115] JS：生成 UUID
来源：http://hz.smart0.xyz/gtnjpqyfva.html

crypto.randomUUID()
来源：http://hz.xylfe.cn/gthpsftgug.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cheryme.top/gtkhdetpin.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258.top/gtqndxesra.html

[U117] JS：单元测试
来源：http://hz.chenzaomai.com/gtakhrjwag.html

npm i -D vitest;  npx vitest
来源：http://hz.chenjidiqi.icu/gtjhplwsdq.html

[U118] JS：开发服务器
来源：http://hz.chenjidiqi.icu/gtuerqulkc.html

npm i -D vite;  npx vite
来源：http://hz.0kj1m.cn/gtiknopzoa.html

[U119] JS：生产构建
来源：http://hz.hnxiangtu.top/gtausozdlc.html

npx vite build
来源：http://hz.fzhhl.top/gtcdoclzrt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhengqikj.top/gtlwprvnaz.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtcvvfcyez.html

================================================================================
来源：http://hz.bjfxy.top/gtocfctdyy.html

统计汇总
来源：http://hz.xziqi.cn/gttmjxmmmr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsxynqhwu.html

按语言统计（条）：
来源：http://hz.yuxming.cn/gtvnxccwow.html

Python ......... 252
来源：http://hz.xylfe.cn/gtsxwxmjrm.html

PHP ............ 252
来源：http://hz.dianchejie.cn/gtzvwsulhj.html

JavaScript ..... 252
来源：http://hz.zhiwuduotai.top/gtkygfterx.html

TypeScript ..... 212
来源：http://hz.guowangkeji.top/gtpezqukfc.html

Java ........... 212
来源：http://hz.wangshuangyany.cn/gtzzzgvbti.html

Go ............. 212
来源：http://hz.shanyushiyangtech.top/gtqsjrsnnz.html

Ruby ........... 212
来源：http://hz.pycfn.com/gtjrgthqcq.html

C# ............. 212
来源：http://hz.kuanghao11.cn/gtcecnkcoe.html

C .............. 30
来源：http://hz.chenzaomai.com/gttsjatlsh.html

C++ ............ 30
来源：http://hz.xingfuxueyuan.xyz/gtwazzobdx.html

SQL ............ 90
来源：http://hz.gogol.net.cn/gtgktwjnjx.html

Bash ........... 80
来源：http://hz.sweek.top/gtpjuunvid.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gtmlliksvn.html

Swift .......... 15
来源：http://hz.yj20258.top/gtornlvweo.html

Lua ............ 10
来源：http://hz.daria6918.cn/gtxwfikxmf.html

Perl ........... 10
来源：http://hz.zhijiandao.cn/gtqxuopebz.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtrmeqyemm.html

------------------------------------
来源：http://hz.zycfv.cn/gtdsxoyrdb.html

合计 ........... 2106 条
来源：http://hz.ydjk.org.cn/gtuswzwhrd.html

按章节统计：
来源：http://hz.snrcjt.cn/gtojwtlrwr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtgpucedgd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gthebzydvz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtkrsdlwnr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gtycfylzhf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.smart0.xyz/gtjupfjmje.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtzjvbjfxh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnqzz.top/gtqvatkgrn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.quarkkingdee.top/gtybwwihqa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtylicasww.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtrckkkkfl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtuxntctnn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtdobqozzd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtlcxgqujj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtmcygiwfh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.haohaochexian.top/gtulzywiyc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtqmvigcio.html

Q SQL 专题                              90
来源：http://hz.havefunace.top/gtnfogirxq.html

R Bash 专题                             80
来源：http://hz.wangdashe.top/gtqyckbthd.html

S C / C++ 专题                          60
来源：http://hz.tanke756.top/gtxyxtklsq.html

T 其他语言补充                          60
来源：http://hz.andypj.xyz/gtcazethlu.html

U 高频实用片段                         120
来源：http://hz.andypj.xyz/gtzvmwaozt.html

------------------------------------
来源：http://hz.gzhubu.top/gtykyaeury.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtffrdnuvd.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtcdvjqdhz.html

使用提醒
来源：http://hz.wangshuangyany.cn/gtvewjmptz.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtejwxvtar.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yonumen.top/gtfltxjpuh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.haohaochexian.top/gtebbjnelv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.9152youxi.cn/gtfniasayl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jiagoushi.top/gtohhitxpv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fengsongda.top/gtmfwxckid.html

—— 文件结束 ——
来源：http://hz.iojbl.cn/gtnoamvush.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyqqeayhx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuxming.cn/gtrzlbliyb.html

Common Programming Examples Cheat Book
来源：http://hz.aibaodan.cn/gtmrkxezbh.html

================================================================================
来源：http://hz.mhx1999.top/gtaucxgefs.html

【收录内容】
来源：http://hz.xingfuxueyuan.xyz/gtnjzambps.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tian-w.cn/gtuaqgbqln.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtafktimyz.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gttheafeaw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenjidiqi.icu/gtujccrlmm.html

【使用说明】
来源：http://hz.ppjwa.cn/gtngblxyyf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.9152youxi.cn/gtfqubddme.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tanke756.top/gtguunznlv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.fzhhl.top/gtveirzqta.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.vqdsnc.cn/gtgkurrtlj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtfwbmcfac.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gotoacloud.top/gtdxbxcvmf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtfaaestkw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shanyushiyangtech.top/gtjbpvvqoc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shangyingyoupin.top/gtlgiyahbs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.mhx1999.top/gtyyerhjoi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zycfv.cn/gtcquwmhky.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj202588.top/gtnimalexz.html

【文件统计】
来源：http://hz.chenlongwang.top/gthecugszu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hongshengwenyu.top/gtditgksxq.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtmnovcvwy.html

目  录
来源：http://hz.nwbrower.top/gtkqznfedc.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtlthrdxvv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jyoumei.cn/gtzumjzrkx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gtzcxkmqsd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtukuevzcp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtuzmlqkbr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yueranfly.top/gtlawtdbyu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cqqwz.cn/gtykgagfny.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gtmnugajpb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yangfankeji.com/gtvcpnehpz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtcpzlfaec.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zycfv.cn/gthwjbvdny.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtbonoxcza.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtgbbzmybd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtyjehdvzc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuetiantiany.cn/gthwidwjpb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cucudq.cn/gtcxvjxtud.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtywysfaxz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.feifeiyinyue.top/gtkqhrbirs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hysaishi.cn/gtuggcsjiu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zycfv.cn/gtvxanzbvw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtbqjlzbkc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtratkvscw.html

================================================================================
来源：http://hz.zycfv.cn/gtoogtthxg.html

A. 基础语法与类型
来源：http://hz.jinqigufen.top/gtkbmllstx.html

================================================================================
来源：http://hz.aizwys.cn/gtsiqclqsg.html

[A01] Hello World
来源：http://hz.yonumen.top/gtvrbrdasf.html

Py:   print("Hello, World!")
来源：http://hz.pycfn.com/gtcjljggus.html

PHP:  echo "Hello, World!";
来源：http://hz.yangfankeji.com/gtnbugagnp.html

JS:   console.log("Hello, World!");
来源：http://hz.jinqigufen.top/gtygrbbqiy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zdqjudy.top/gtbyqlqznd.html

Java: System.out.println("Hello, World!");
来源：http://hz.iojbl.cn/gtpnrhenep.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hammf.cn/gtemwciufa.html

Ruby: puts "Hello, World!"
来源：http://hz.dianchejie.cn/gtgikbkoca.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.nwbrower.top/gttqwpxxuo.html

[A02] 变量声明与赋值
来源：http://hz.hywenlv.cn/gtzmlxbqny.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yj20258888.top/gtccspnhec.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.iojbl.cn/gtbeuqgblz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hnxiangtu.top/gtefthsfxj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj20258.top/gtcojuhgxd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinyuanbaomall.cn/gttervikhi.html

Go:   name := "Alex"; age := 20
来源：http://hz.ywan-chungtsiang.top/gtnftxctjw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gtifllnpin.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtbwffltwq.html

[A03] 常量定义
来源：http://hz.nanxinkj.top/gtujyhjjjc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuanzx.com/gtfrngbute.html

PHP:  const PI = 3.14159;
来源：http://hz.jqgufenzy.top/gthutmzaez.html

JS:   const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtwpvhhrzj.html

TS:   const PI: number = 3.14159;
来源：http://hz.hysaishi.cn/gtnjspwkej.html

Java: static final double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtdwrjdnze.html

Go:   const PI = 3.14159
来源：http://hz.meibo888.top/gtgzabfpeo.html

Ruby: PI = 3.14159
来源：http://hz.redwolf501.top/gtfxlgikhd.html

C#:   const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtgwkotmth.html

[A04] 判断变量类型
来源：http://hz.xuanzx.com/gtxtchcynh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gtfhalmskk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhijiandao.cn/gtwcgfwbuc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shuidangran.top/gtedklpbnr.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigufen.top/gtccxogzkk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gtzwqjuozx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.aizwys.cn/gtxwrrnjhv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.316326.xyz/gtgpcgjqwu.html

C#:   x.GetType().Name; x is int
来源：http://hz.xuanzx.com/gtlgffszmu.html

[A05] 整数除法与取模
来源：http://hz.daria6918.cn/gtoiektvqw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.52xcode.cn/gtykckqtgw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.tanke756.top/gtxyhtbxyj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gtrpechdmu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.kuanghao11.cn/gtfjepyvtb.html

Java: 7 / 2; 7 % 2
来源：http://hz.hfpthk.cn/gtbktofbii.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtvrazzoig.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtdmhtyant.html

C#:   7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtvsrhcxnu.html

[A06] 字符串转数字
来源：http://hz.52xcode.cn/gtbiubomem.html

Py:   int("42"); float("3.14")
来源：http://hz.haohaochexian.top/gtwookscly.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.pengpengdd.cyou/gtukfavkin.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hfpthk.cn/gtfdpamprc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cheryme.top/gtzmrnwrif.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zycfv.cn/gtdzrffojy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sweek.top/gtnyhfeeof.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jianghu66.top/gtjmgnoseo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangdashe.top/gttzozxtxq.html

[A07] 数字转字符串
来源：http://hz.jiagoushi.top/gtljgpgqii.html

Py:   str(42)
来源：http://hz.yj20258888.top/gttrtenonx.html

PHP:  (string) 42; strval(42)
来源：http://hz.daxiang520.top/gtgdzvhkfu.html

JS:   String(42); (42).toString()
来源：http://hz.andypj.xyz/gtmxwmtbls.html

TS:   String(42)
来源：http://hz.ybcxt.top/gtowakmeke.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.svipenyu.cn/gtlumjrzdy.html

Go:   strconv.Itoa(42)
来源：http://hz.smart0.xyz/gtcmkbrxxf.html

Ruby: 42.to_s
来源：http://hz.zhixingplan.top/gtkmmkmcqs.html

C#:   42.ToString()
来源：http://hz.cucudq.cn/gtdfqhxiyc.html

[A08] 取整与四舍五入
来源：http://hz.gotoacloud.top/gtpgwrqipc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jlsjyb.cn/gtfazhlxhe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yangfankeji.com/gtdqrjhwjs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj202588.top/gtodtqbktu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yanxiufei.cn/gtkdjqerqa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zdqjudy.top/gtmffgogqs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhoulong.xyz/gtlkoqhbxv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yangfankeji.com/gtndhayrxr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gotoacloud.top/gttekcuodd.html

[A09] 绝对值与最大最小值
来源：http://hz.nanxinkj.top/gtnxuleyqj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258888.top/gtnaurmbpt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenzaomai.com/gtmyqxlvmq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.vqdsnc.cn/gtpopvioug.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.dianchejie.cn/gtyczuworb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.aibaodan.cn/gtmpssesnf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.kuanghao11.cn/gtdrbxuddi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.sweek.top/gtvpbtvabf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yj20258888.top/gthikpdkub.html

[A10] 生成随机数
来源：http://hz.zhongyouzk.top/gtyqwtdamm.html

Py:   import random; random.randint(1, 100)
来源：http://hz.cucudq.cn/gtfuxazxqr.html

PHP:  random_int(1, 100);
来源：http://hz.ybcxt.top/gtvcouznsu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ehwqpu.com/gttlxcxfde.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gotoacloud.top/gtmgyfjzip.html

Java: new Random().nextInt(100) + 1
来源：http://hz.shanyushiyangkeji.top/gtkpgjkxpc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hfpthk.cn/gtyjsvyktj.html

Ruby: rand(1..100)
来源：http://hz.9152youxi.cn/gtfuhkqdtm.html

C#:   new Random().Next(1, 101)
来源：http://hz.shanyushiyangtech.top/gtrafljnvm.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtuhbmahlv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.tianlin.xyz/gtoncbvcjn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtvjaipats.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.snrcjt.cn/gtpxseicrn.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtnfkhrsdx.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtiyjepsjg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.andypj.xyz/gttgdqjjre.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtxugncvka.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhixingplan.top/gtdqlnehqc.html

[A12] 字符串插值 / 格式化
来源：http://hz.daria6918.cn/gttqamcawe.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shanyushiyangkeji.top/gtmssqjorl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhixingplan.top/gtbdsaqkei.html

JS:   `Hello, ${name}!`
来源：http://hz.zhixingplan.top/gtyeiujtrn.html

TS:   `Hello, ${name}!`
来源：http://hz.andypj.xyz/gtjwlbsspx.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.havefunace.top/gtvnxsvxzp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xinyue.icu/gtxiacqfmy.html

Ruby: "Hello, #{name}!"
来源：http://hz.pycfn.com/gtarlclwwq.html

C#:   $"Hello, {name}!"
来源：http://hz.nanxinkj.top/gttzaivrvr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yuxming.cn/gtfrzmztoj.html

Py:   "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gttrcxrgar.html

PHP:  "第一行\n第二行"
来源：http://hz.gotoacloud.top/gtwbvodlkc.html

JS:   "第一行\n第二行"
来源：http://hz.havefunace.top/gtvhkjknmq.html

TS:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtumpedwqh.html

Java: "第一行\n第二行"
来源：http://hz.c1oappe.top/gtqannfuwu.html

Go:   "第一行\n第二行"
来源：http://hz.yuanzhike.top/gtrzyampig.html

Ruby: "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtdhsxpeja.html

C#:   "第一行\n第二行"
来源：http://hz.andypj.xyz/gtfvmtceyd.html

[A14] 注释写法
来源：http://hz.quarkkingdee.top/gtxvbtrdjz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.sweek.top/gtdtmsmebl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.guannengcc.top/gtdvnwstvy.html

JS:   // 单行；/* 多行 */
来源：http://hz.ybcxt.top/gtgqhctusm.html

TS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtqsyrvszd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.meibo888.top/gtvwckkcoy.html

Go:   // 单行；/* 多行 */
来源：http://hz.zhiwuduotai.top/gtjspuvqsh.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hammf.cn/gtmnyrmihd.html

C#:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtgapohkee.html

[A15] 空值判断与默认值
来源：http://hz.hnxiangtu.top/gteckajnjm.html

Py:   value = data or "默认值"
来源：http://hz.cdnleiting.top/gtwqqqqxgz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.pycfn.com/gtqbjaqujq.html

JS:   const value = data ?? "默认值";
来源：http://hz.yangfankeji.com/gtevvihzom.html

TS:   const value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtnusempmx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shzxlz.cn/gtocwdtirj.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.chenjidiqi.icu/gtxktuuwsh.html

Ruby: value = data || "默认值"
来源：http://hz.chenlongwang.top/gtqffymtxt.html

C#:   var value = data ?? "默认值";
来源：http://hz.wangshuangyany.cn/gtenewkcvt.html

[A16] 真假值判断规则
来源：http://hz.nwbrower.top/gtvpnuzkyj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.snrcjt.cn/gtrjfxxuct.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gotoacloud.top/gtwygbpsdz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ywan-chungtsiang.top/gtbukewula.html

TS:   if (!x) {}
来源：http://hz.shuidangran.top/gtwwvxlghg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.tanke756.top/gtjvydtiyt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.meibo888.top/gtnyeenhpz.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenlongwang.top/gtgxloczaa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ywan-chungtsiang.top/gtpdwzwkxh.html

[A17] 位运算
来源：http://hz.xziqi.cn/gtsdfgrral.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtckqxynyo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gzhubu.top/gtweebmqsk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuxming.cn/gtkmxmqpfd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.cashguo.top/gtfkbhkrrc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gtibyjdkwm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtlnuconve.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtmpjgynfh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.52xcode.cn/gtqnurmbky.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yj20258888.top/gtahqfnsyq.html

Py:   ord("A"); chr(65)
来源：http://hz.hfpthk.cn/gtxeffnvmp.html

PHP:  ord("A"); chr(65)
来源：http://hz.aibaodan.cn/gtxtrtzwex.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xziqi.cn/gtcxofuwvy.html


<!-- 参考信息 -->