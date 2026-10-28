代发 wailian999

[U95] JS：Promise 包装
来源：http://hz.daxiang520.top/gthnjxynph.html

new Promise((resolve, reject) => {})
来源：http://hz.yj20258888.top/gtoybuywli.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gtdjtjmejm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtunhhkpjo.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gttjbzgnre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtloepzhdl.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtwlwcnncv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.kuanghao11.cn/gtgxceiblc.html

[U99] JS：事件监听
来源：http://hz.9152youxi.cn/gtjwpebwnx.html

el.addEventListener("click", e => {})
来源：http://hz.cashguo.top/gtvhjteigp.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtqrmrqgxo.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtktsrlodg.html

[U101] JS：classList 操作
来源：http://hz.yj20258888.top/gtemrgtlat.html

el.classList.toggle("active")
来源：http://hz.316326.xyz/gtlqakkqcf.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtlvljnsbx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtoujrvoyl.html

[U103] JS：定时器
来源：http://hz.yonumen.top/gtsfjbuvaj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cheryme.top/gtrurgubtc.html

[U104] JS：防抖
来源：http://hz.aibaodan.cn/gtybjbndyj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtisjfmvil.html

[U105] JS：节流
来源：http://hz.aizwys.cn/gtdrehoyun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tanke756.top/gthffxfqxm.html

[U106] JS：日期格式化
来源：http://hz.kuanghao11.cn/gtbinyvrya.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.aizwys.cn/gtkbkoppwu.html

[U107] JS：数字千分位
来源：http://hz.meibo888.top/gtjdwrqtwy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhoulong.xyz/gtmuvvaazv.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtgwmezahf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fzhhl.top/gtuxqtjrcc.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtadvhtgvq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtjoposbgo.html

[U110] JS：数组分块
来源：http://hz.yj20258888.top/gtgsuhtnjq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ppjwa.cn/gtkgusynxw.html

[U111] JS：对象转 Map
来源：http://hz.cqqwz.cn/gtpkxnhlsz.html

new Map(Object.entries(obj))
来源：http://hz.0kj1m.cn/gtyctclpiy.html

[U112] JS：字符串补位
来源：http://hz.jianghu66.top/gtuzcszcbr.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtstbrwqjf.html

[U113] JS：正则替换全部
来源：http://hz.chenjidiqi.icu/gtouucaqiw.html

s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtjxnwgyuu.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtpbwjvbsa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtowyrofmr.html

[U115] JS：生成 UUID
来源：http://hz.fengsongda.top/gtebcygamy.html

crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtzqalvzmz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gzhubu.top/gtupdrjomx.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258888.top/gtnflgsfqu.html

[U117] JS：单元测试
来源：http://hz.mhx1999.top/gtmcsanbik.html

npm i -D vitest;  npx vitest
来源：http://hz.xziqi.cn/gtcezmdylv.html

[U118] JS：开发服务器
来源：http://hz.xuanzx.com/gtgcholfxv.html

npm i -D vite;  npx vite
来源：http://hz.dashuyun.cn/gtvnjfmxlf.html

[U119] JS：生产构建
来源：http://hz.gogol.net.cn/gtsuekgkmd.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtdukcdezg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnqzz.top/gtstbzclfj.html

import.meta.env.VITE_API_URL
来源：http://hz.zhijiandao.cn/gtclhcpyjb.html

================================================================================
来源：http://hz.wangdashe.top/gtyabnsquq.html

统计汇总
来源：http://hz.pycfn.com/gtxnptjois.html

================================================================================
来源：http://hz.c1oappe.top/gtbekuuktw.html

按语言统计（条）：
来源：http://hz.guannengcc.top/gtaamxgisp.html

Python ......... 252
来源：http://hz.yj202588.top/gtdqcroivw.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtigutofdk.html

JavaScript ..... 252
来源：http://hz.zhiwuduotai.top/gtctgvssff.html

TypeScript ..... 212
来源：http://hz.chenlongwang.top/gtsekfomge.html

Java ........... 212
来源：http://hz.kuanghao11.cn/gttgrsmxns.html

Go ............. 212
来源：http://hz.cheryme.top/gtbrddtgrm.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtzscogngs.html

C# ............. 212
来源：http://hz.jlsjyb.cn/gtzzllkdly.html

C .............. 30
来源：http://hz.ydjk.org.cn/gtfhikuuvs.html

C++ ............ 30
来源：http://hz.yonumen.top/gtkglatuzg.html

SQL ............ 90
来源：http://hz.jinghuilouyu.cn/gtvgmvynpv.html

Bash ........... 80
来源：http://hz.cqqwz.cn/gtarkbygir.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gtoodcqyiu.html

Swift .......... 15
来源：http://hz.yongpay.top/gtvpjwnrzv.html

Lua ............ 10
来源：http://hz.xingfuxueyuan.xyz/gtzfofyxza.html

Perl ........... 10
来源：http://hz.xuetiantiany.cn/gtrkuzquhw.html

Scala .......... 10
来源：http://hz.hywenlv.cn/gtsqsyahip.html

------------------------------------
来源：http://hz.yangfankeji.com/gthnfvovua.html

合计 ........... 2106 条
来源：http://hz.fzhhl.top/gtvmzcnaxy.html

按章节统计：
来源：http://hz.gogol.net.cn/gtbskuklvr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258888.top/gtcgdvpwuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtxotizxlu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtushclayi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.vqdsnc.cn/gtqmianmrj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cashguo.top/gtqycboers.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtaxcgnzbe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtrbpfngje.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnxiangtu.top/gtrvielmsc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtnmhguxwb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hongshengwenyu.top/gtfjtlspbm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtxukhqoxq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtyrsgyhtu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtznqfeske.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daria6918.cn/gtjseslhmi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtlbbbyjda.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtgtpyrkcf.html

Q SQL 专题                              90
来源：http://hz.xuetiantiany.cn/gttkefzzik.html

R Bash 专题                             80
来源：http://hz.yanxiufei.cn/gthmndsscl.html

S C / C++ 专题                          60
来源：http://hz.316326.xyz/gtqrcdoxli.html

T 其他语言补充                          60
来源：http://hz.bjfxy.top/gtwlhwmecp.html

U 高频实用片段                         120
来源：http://hz.52xcode.cn/gtbyoginop.html

------------------------------------
来源：http://hz.daria6918.cn/gtmjcjcbyv.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtfjkfkpkr.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtlxapyekg.html

使用提醒
来源：http://hz.andypj.xyz/gtnmnjonil.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtjvrdkckk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gtdowgrdba.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tianlin.xyz/gtarziapcf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fzhhl.top/gtbzjlydyv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.bjfxy.top/gtssztowiu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.0kj1m.cn/gtnowtzump.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gtsemhjygg.html

================================================================================
来源：http://hz.chenlongwang.top/gtzhncyohl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.vqdsnc.cn/gtvgmtxhoz.html

Common Programming Examples Cheat Book
来源：http://hz.jqgufenzy.top/gtrfynjhqj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfrrvgojr.html

【收录内容】
来源：http://hz.yj20258.top/gttnmggdjm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yangfankeji.com/gtufvlvzrp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.bjfxy.top/gtvnjcvurd.html

SQL · Bash · C · C++
来源：http://hz.bjfxy.top/gtxyonimuq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtrhmbcpou.html

【使用说明】
来源：http://hz.jiagoushi.top/gtvzsoryyu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.0kj1m.cn/gtjzsrsjdo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guowangkeji.top/gtogwgmltc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jyoumei.cn/gtmxsmpidz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtgcbjyhwc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hfpthk.cn/gtsztvtohl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gttjexdfzo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guannengcc.top/gtuqklytxh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fengsongda.top/gttpuixrsv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.guowangkeji.top/gtrdzgjagr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sufxvd.cn/gtlgnnavyj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhaomingkeji.xyz/gtbflnwdzm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sufxvd.cn/gtrmevbqbt.html

【文件统计】
来源：http://hz.xuanzx.com/gtoooqotnm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.wangdashe.top/gtlucvzxvy.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtuwaqpnlf.html

目  录
来源：http://hz.yj20258.top/gtstopibdz.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtnqptmars.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtysikoiue.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gttzngyscf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtrctkdmbs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ybcxt.top/gtbqzndmfa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xinyue.icu/gtnnpngrec.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtdrxyozow.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtjmgcjcut.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ppjwa.cn/gtvwhqejes.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtmxkvktxt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.meibo888.top/gthvlefcih.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtgpahvrim.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtzgqaljzi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtrluucxkc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jinghuilouyu.cn/gtnwwuiugm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ivvv.top/gttducmcdj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtvyealzil.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shuidangran.top/gtahczhqvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yongpay.top/gtnkwswhia.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hywenlv.cn/gtnchsrdko.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtbozezwby.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtmerlpjsl.html

================================================================================
来源：http://hz.hysaishi.cn/gtmkavshly.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtmauzmtjz.html

================================================================================
来源：http://hz.jianghu66.top/gtogtgohea.html

[A01] Hello World
来源：http://hz.shangyingyoupin.top/gtbdivlbuh.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtdvxnzezf.html

PHP:  echo "Hello, World!";
来源：http://hz.tanke756.top/gtmlyznlra.html

JS:   console.log("Hello, World!");
来源：http://hz.chenjidiqi.icu/gteufycwwe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.0kj1m.cn/gtgziymyae.html

Java: System.out.println("Hello, World!");
来源：http://hz.guowangkeji.top/gtzaksacqq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gotoacloud.top/gtpugphufl.html

Ruby: puts "Hello, World!"
来源：http://hz.zdqjudy.top/gtniukkepp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258888.top/gtaikqetoq.html

[A02] 变量声明与赋值
来源：http://hz.hongshengwenyu.top/gtzwwucxne.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ivvv.top/gtvftfhdvy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.0kj1m.cn/gtqwmjwray.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yuxming.cn/gtipkhvfnj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guowangkeji.top/gtbrunyqld.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yueranfly.top/gtkbhuxujt.html

Go:   name := "Alex"; age := 20
来源：http://hz.ehwqpu.com/gtgxvtjopt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guowangkeji.top/gthdayyhke.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yj202588.top/gtaxzkswns.html

[A03] 常量定义
来源：http://hz.gogol.net.cn/gtswnyflhg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guannengcc.top/gtbgrwfrln.html

PHP:  const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtmzklijjz.html

JS:   const PI = 3.14159;
来源：http://hz.mhx1999.top/gtmjdkpfpb.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtygppagzf.html

Java: static final double PI = 3.14159;
来源：http://hz.xinyue.icu/gtmmnbqcdm.html

Go:   const PI = 3.14159
来源：http://hz.sufxvd.cn/gtbmlhyedc.html

Ruby: PI = 3.14159
来源：http://hz.shuidangran.top/gtfprmmwss.html

C#:   const double PI = 3.14159;
来源：http://hz.daria6918.cn/gtxjzoncch.html

[A04] 判断变量类型
来源：http://hz.gotoacloud.top/gtlcoyycbn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.cdnleiting.top/gtjhnuukoo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xingfuxueyuan.xyz/gtuhlziwcb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.meibo888.top/gtmsjzluqs.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangshuangyany.cn/gtefgsustn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.tianlin.xyz/gthrmlmddx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ybcxt.top/gtfvzvkddy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.bjfxy.top/gtufbtbwmm.html

C#:   x.GetType().Name; x is int
来源：http://hz.xingfuxueyuan.xyz/gtjrikyyio.html

[A05] 整数除法与取模
来源：http://hz.hfpthk.cn/gtwnrupxiq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.fengsongda.top/gtdxywjylh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hywenlv.cn/gthyzkofwp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxinkj.top/gtgcjykudy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuanzx.com/gtrkyjjuli.html

Java: 7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtatfebqrs.html

Go:   7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtdoitjblu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtgzktakyi.html

C#:   7 / 2; 7 % 2
来源：http://hz.jinqigufen.top/gtnqievsaw.html

[A06] 字符串转数字
来源：http://hz.zhoulong.xyz/gtelbtlzqk.html

Py:   int("42"); float("3.14")
来源：http://hz.pycfn.com/gtwifociby.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.bjfxy.top/gtmezqjcxj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nanxuanxn.top/gtqeiscifs.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cqqwz.cn/gtpdmhuibj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shuidangran.top/gtdwvqiqfu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhaomingkeji.xyz/gtfvikpgfn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.cdnleiting.top/gtqbkalfmh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.9152youxi.cn/gtfxntavkh.html

[A07] 数字转字符串
来源：http://hz.jlsjyb.cn/gtzbkzblbb.html

Py:   str(42)
来源：http://hz.wangshuangyany.cn/gtkexxvgpw.html

PHP:  (string) 42; strval(42)
来源：http://hz.c1oappe.top/gtbuwvqmck.html

JS:   String(42); (42).toString()
来源：http://hz.xziqi.cn/gtqioewzkk.html

TS:   String(42)
来源：http://hz.shuidangran.top/gtyjbzynei.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ppjwa.cn/gtyoafciro.html

Go:   strconv.Itoa(42)
来源：http://hz.cheryme.top/gtluoynijc.html

Ruby: 42.to_s
来源：http://hz.c1oappe.top/gtrztognfv.html

C#:   42.ToString()
来源：http://hz.yj20258888.top/gtwnkthwpz.html

[A08] 取整与四舍五入
来源：http://hz.chenjidiqi.icu/gtxqusdqdt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.316326.xyz/gtyuvlmzlx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ybcxt.top/gtpiwxtrcz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhaomingkeji.xyz/gtirotulsk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.havefunace.top/gthawhtbji.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtyrvkkobn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.mhx1999.top/gtzowtzzjt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenzaomai.com/gtcunzoqoy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj20258.top/gtnytvwsra.html

[A09] 绝对值与最大最小值
来源：http://hz.316326.xyz/gtslapbvvz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtbqoguhcc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jiagoushi.top/gtsgvjrtoo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.vqdsnc.cn/gtnkegkhmk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.sweek.top/gtosjrmuwc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ehwqpu.com/gtofwxlbgc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinqigufen.top/gtqimwlzxl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.c1oappe.top/gtkmtjviqz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.gaohongyu789.top/gttcivvksb.html

[A10] 生成随机数
来源：http://hz.shzxlz.cn/gtdqatqpgv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jianghu66.top/gtmuptnslz.html

PHP:  random_int(1, 100);
来源：http://hz.zhoulong.xyz/gtwlrysjra.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigufen.top/gtjoewhkpd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.svipenyu.cn/gtvigaandb.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hysaishi.cn/gtuawmpwdz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hfpthk.cn/gtboufgdlu.html

Ruby: rand(1..100)
来源：http://hz.jlsjyb.cn/gtvfcbexuo.html

C#:   new Random().Next(1, 101)
来源：http://hz.0kj1m.cn/gtoxcsswex.html

[A11] 条件表达式（三元）
来源：http://hz.daxiang520.top/gtufvbssmw.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtvdybqrds.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gtqtmrqzah.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.daxiang520.top/gtvodcyyzm.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtmxzaejrb.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhoulong.xyz/gtelofvlxe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.dianchejie.cn/gtzfcprapy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.wangshuangyany.cn/gtrlomzwar.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtjvjvpszz.html

[A12] 字符串插值 / 格式化
来源：http://hz.dashuyun.cn/gtnfzsthbt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jqgfzy.top/gttdqcljok.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.wangdashe.top/gtpwjcgdyy.html

JS:   `Hello, ${name}!`
来源：http://hz.ywan-chungtsiang.top/gtjyoilglu.html

TS:   `Hello, ${name}!`
来源：http://hz.yueranfly.top/gtxrhynadu.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.snrcjt.cn/gtcfjeaozc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.wangshuangyany.cn/gtksrgwran.html

Ruby: "Hello, #{name}!"
来源：http://hz.guowangkeji.top/gtxfhmexdi.html

C#:   $"Hello, {name}!"
来源：http://hz.vqdsnc.cn/gtutcpeupe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.mhx1999.top/gtkeutdcbo.html

Py:   "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtghyeparq.html

PHP:  "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtnjdtvcjg.html

JS:   "第一行\n第二行"
来源：http://hz.yanxiufei.cn/gtpgvvegfc.html

TS:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtpuamsxqq.html

Java: "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtiqalvtbg.html

Go:   "第一行\n第二行"
来源：http://hz.yonumen.top/gtmmigztvj.html

Ruby: "第一行\n第二行"
来源：http://hz.zhiwuduotai.top/gtcdnbbtnv.html

C#:   "第一行\n第二行"
来源：http://hz.ydzc1.top/gtueeuayqa.html

[A14] 注释写法
来源：http://hz.jlsjyb.cn/gtdasdtdcd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yj20258888.top/gtbukkndxp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtarhgrozl.html

JS:   // 单行；/* 多行 */
来源：http://hz.redwolf501.top/gthsjhnhla.html

TS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtaujmoljl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.chenjidiqi.icu/gtkzzkpgas.html

Go:   // 单行；/* 多行 */
来源：http://hz.yj20258888.top/gtindoucfy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yangfankeji.com/gtahmcnnjg.html

C#:   // 单行；/* 多行 */
来源：http://hz.wangdashe.top/gtgutyvfmt.html

[A15] 空值判断与默认值
来源：http://hz.snrcjt.cn/gtsgpndygv.html

Py:   value = data or "默认值"
来源：http://hz.snrcjt.cn/gtwcgmxabb.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jyoumei.cn/gtkjywoyau.html

JS:   const value = data ?? "默认值";
来源：http://hz.zycfv.cn/gtsjfxdmls.html

TS:   const value = data ?? "默认值";
来源：http://hz.pycfn.com/gtuvmyifrl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.aibaodan.cn/gtjibuclsg.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.chenzaomai.com/gtotzyxxih.html

Ruby: value = data || "默认值"
来源：http://hz.dianchejie.cn/gthwgqsauw.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinqigufen.top/gtsxaaynhj.html

[A16] 真假值判断规则
来源：http://hz.zhengqikj.top/gtvreweiky.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zycfv.cn/gtqlhkvcsa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.dianchejie.cn/gtyrmtksbg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.dashuyun.cn/gtoffulzxc.html

TS:   if (!x) {}
来源：http://hz.guowangkeji.top/gtwdeumbpi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.0kj1m.cn/gtacfxilrq.html


<!-- 参考信息 -->