代发 wailian999

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtpkxygzfm.html

`共 ${n} 条`
来源：http://hz.ybcxt.top/gtjpvtoybw.html

[U94] JS：箭头函数
来源：http://hz.316326.xyz/gtfgbqccsf.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtggffondp.html

[U95] JS：Promise 包装
来源：http://hz.yanxiufei.cn/gtezflnasq.html

new Promise((resolve, reject) => {})
来源：http://hz.xuanzx.com/gtoizhxdsv.html

[U96] JS：async/await 与异常
来源：http://hz.gotoacloud.top/gtbcpeorkg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gthdjxtrvy.html

[U97] JS：并发请求
来源：http://hz.zhixingplan.top/gtjciuoncg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtrvixcffr.html

[U98] JS：fetch 带 JSON
来源：http://hz.yueranfly.top/gtmiuuzeio.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guannengcc.top/gtjaeftvcn.html

[U99] JS：事件监听
来源：http://hz.feifeiyinyue.top/gteitfdyye.html

el.addEventListener("click", e => {})
来源：http://hz.316326.xyz/gtbgbzkyyu.html

[U100] JS：DOM 查询
来源：http://hz.yonumen.top/gtvlkmpgpg.html

document.querySelector(".item")
来源：http://hz.iojbl.cn/gtqcsxingl.html

[U101] JS：classList 操作
来源：http://hz.aibaodan.cn/gtevkoofpz.html

el.classList.toggle("active")
来源：http://hz.0kj1m.cn/gtfhqxuwox.html

[U102] JS：本地存储
来源：http://hz.shangyingyoupin.top/gtesxgdwpz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydjk.org.cn/gtaakiyxxg.html

[U103] JS：定时器
来源：http://hz.zhiwuduotai.top/gtwxyfviry.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yonumen.top/gtferbisft.html

[U104] JS：防抖
来源：http://hz.zhoulong.xyz/gtgbigvhxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtxnnwlcjh.html

[U105] JS：节流
来源：http://hz.daria6918.cn/gtugbriftk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gtrymokupi.html

[U106] JS：日期格式化
来源：http://hz.fzhhl.top/gtqarjnbob.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ppjwa.cn/gtanuahaqk.html

[U107] JS：数字千分位
来源：http://hz.sweek.top/gtcyejxkat.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guowangkeji.top/gtvavjxvmv.html

[U108] JS：随机整数
来源：http://hz.dashuyun.cn/gtzwtmdxbl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.bjfxy.top/gtmkhpbnad.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtlxwstoie.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtamdctcov.html

[U110] JS：数组分块
来源：http://hz.sweek.top/gtoxsrvsfs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.feifeiyinyue.top/gtdsqedgjg.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangtech.top/gtjmkehjdw.html

new Map(Object.entries(obj))
来源：http://hz.jiagoushi.top/gtvvsngtsu.html

[U112] JS：字符串补位
来源：http://hz.316326.xyz/gtqewnznco.html

"7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gttzvyzzaw.html

[U113] JS：正则替换全部
来源：http://hz.zdqjudy.top/gtazhwludf.html

s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtblswsknt.html

[U114] JS：JSON 深比较
来源：http://hz.svipenyu.cn/gteydwrnoe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtzswwukbn.html

[U115] JS：生成 UUID
来源：http://hz.gzhubu.top/gtereqrjed.html

crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtrzjycaey.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zycfv.cn/gtscegjbvq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnqzz.top/gthvmvlmon.html

[U117] JS：单元测试
来源：http://hz.chenlongwang.top/gtihokzeqt.html

npm i -D vitest;  npx vitest
来源：http://hz.dianchejie.cn/gtjqflwlau.html

[U118] JS：开发服务器
来源：http://hz.bjfxy.top/gtvpcflyai.html

npm i -D vite;  npx vite
来源：http://hz.xuanzx.com/gtgwxqeojx.html

[U119] JS：生产构建
来源：http://hz.guannengcc.top/gtgnruygbh.html

npx vite build
来源：http://hz.9152youxi.cn/gtukbqeaov.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhixingplan.top/gtuijpsral.html

import.meta.env.VITE_API_URL
来源：http://hz.52xcode.cn/gtbpepmeam.html

================================================================================
来源：http://hz.sxryk.cn/gtirwmbsib.html

统计汇总
来源：http://hz.hammf.cn/gtqerywpxd.html

================================================================================
来源：http://hz.zhengqikj.top/gtruxrojmg.html

按语言统计（条）：
来源：http://hz.tanke756.top/gttnoeinbb.html

Python ......... 252
来源：http://hz.wangshuangyany.cn/gtjgzknksy.html

PHP ............ 252
来源：http://hz.xylfe.cn/gtiuplgzqt.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gtiotzxfsw.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtoiabfiur.html

Java ........... 212
来源：http://hz.shangyingyoupin.top/gtkukqbdqx.html

Go ............. 212
来源：http://hz.xuanzx.com/gtrnhhdubi.html

Ruby ........... 212
来源：http://hz.fzhhl.top/gttdlvxsbx.html

C# ............. 212
来源：http://hz.shanyushiyangkeji.top/gtqekbznva.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtizpaymuj.html

C++ ............ 30
来源：http://hz.xziqi.cn/gtapxyriqj.html

SQL ............ 90
来源：http://hz.yvedp.cn/gtzrfstpwd.html

Bash ........... 80
来源：http://hz.guannengcc.top/gtrnuezvvv.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtvohbpcme.html

Swift .......... 15
来源：http://hz.cucudq.cn/gteivunsyb.html

Lua ............ 10
来源：http://hz.redwolf501.top/gtuemjygyq.html

Perl ........... 10
来源：http://hz.yj20258888.top/gtzxdwgyqi.html

Scala .......... 10
来源：http://hz.yj20258.top/gtytjbptxf.html

------------------------------------
来源：http://hz.andypj.xyz/gtxscqomum.html

合计 ........... 2106 条
来源：http://hz.zhoulong.xyz/gtvwvpobil.html

按章节统计：
来源：http://hz.yj20258.top/gtrgmvaxul.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtblpcwyig.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.kuanghao11.cn/gtsgbunnsa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtvgyofekr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gttcvaavnd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinghuilouyu.cn/gtqljysgrq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtgmwbglnn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gtepcvqjpn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtjeeoiedj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtpzfpefch.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtdsentlra.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtqninkmdb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtflevjued.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtsccfxuqg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtptzwurdv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gotoacloud.top/gttlrbdfoi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtoamhndup.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtplpiebyg.html

R Bash 专题                             80
来源：http://hz.redwolf501.top/gtjvhsqsfo.html

S C / C++ 专题                          60
来源：http://hz.0kj1m.cn/gtuwhscvss.html

T 其他语言补充                          60
来源：http://hz.chenjidiqi.icu/gttuiqkpaz.html

U 高频实用片段                         120
来源：http://hz.hongshengwenyu.top/gtgasxgowf.html

------------------------------------
来源：http://hz.nwbrower.top/gtghtxtfhy.html

合计                                  2106 条
来源：http://hz.yuxming.cn/gteyctrpyv.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gtyluguwsu.html

使用提醒
来源：http://hz.gotoacloud.top/gtmxfqhmzf.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtjcsmcuvb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hysaishi.cn/gtkeigtemv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hongshengwenyu.top/gtympuijvd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fzhhl.top/gttxuovhii.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jqgfzy.top/gtdnjpwaux.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangdashe.top/gtxtyqaudu.html

—— 文件结束 ——
来源：http://hz.jyoumei.cn/gtqgcsuuqb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfpweumno.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aizwys.cn/gtxrspljlr.html

Common Programming Examples Cheat Book
来源：http://hz.zhongyouzk.top/gtkzumkutm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrokdntmm.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtlokwfvwq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.snrcjt.cn/gtrfbdajxl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtkmgulemn.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gtnjskxctz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhaomingkeji.xyz/gtjdjhfbuy.html

【使用说明】
来源：http://hz.zhaomingkeji.xyz/gtjwjrgwqi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenlongwang.top/gtnejrgtlo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tanke756.top/gthduecnno.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuxming.cn/gtnjezkogl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.smart0.xyz/gtyynmgbpt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sufxvd.cn/gtkcjqyegn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tanke756.top/gthubnmsoc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haohaochexian.top/gtjvvrexdz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.pengpengdd.cyou/gtbhcpzzsv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.wangshuangyany.cn/gtodaqrvcr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sufxvd.cn/gtgkdbekyo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenjidiqi.icu/gtcvwszgxf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nanxuanxn.top/gtycmogrkc.html

【文件统计】
来源：http://hz.yueranfly.top/gtfzatrlev.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ywan-chungtsiang.top/gtnydmizgu.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtvrhprdfe.html

目  录
来源：http://hz.quarkkingdee.top/gtuertdzww.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gttplnwyno.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtgjuknyse.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtyvtoeipe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fengsongda.top/gtjniurfhq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtnxytqcgg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jianghu66.top/gtlruochxi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gttwecyeaj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtzmvtknwo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gttadcatre.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtdlefgzba.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtwxqkempc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtijstkeiu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtumjmkhnc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtkutvfouh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtikqobldj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fzhhl.top/gtobtwolrv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtqzdwgozb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shanyushiyangtech.top/gtmautuddy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinghuilouyu.cn/gtdrlmqrto.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gtyyecwtyr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtbyqassce.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yueranfly.top/gthtrpgrjo.html

================================================================================
来源：http://hz.hammf.cn/gtqljjukeg.html

A. 基础语法与类型
来源：http://hz.yongpay.top/gtemjmrmem.html

================================================================================
来源：http://hz.yonumen.top/gtgatqskky.html

[A01] Hello World
来源：http://hz.ydzc1.top/gteajquhhd.html

Py:   print("Hello, World!")
来源：http://hz.hywenlv.cn/gtbjjkmzym.html

PHP:  echo "Hello, World!";
来源：http://hz.ywan-chungtsiang.top/gtixsxwfig.html

JS:   console.log("Hello, World!");
来源：http://hz.sxryk.cn/gtxwbzyawk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ywan-chungtsiang.top/gtfmscsqwg.html

Java: System.out.println("Hello, World!");
来源：http://hz.jianghu66.top/gtsjackhei.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.vqdsnc.cn/gtcmbpxmyk.html

Ruby: puts "Hello, World!"
来源：http://hz.smart0.xyz/gtqbbclyzv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258.top/gtxvedrrjb.html

[A02] 变量声明与赋值
来源：http://hz.guowangkeji.top/gtdcsxyrgf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nanxuanxn.top/gtchgusncc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ivvv.top/gtqgnfwpmg.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.feifeiyinyue.top/gtvosxbsxm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xinyue.icu/gtqzdfuhup.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydjk.org.cn/gtlimmlfiv.html

Go:   name := "Alex"; age := 20
来源：http://hz.xuanzx.com/gtiglntoee.html

Ruby: name = "Alex"; age = 20
来源：http://hz.havefunace.top/gtwigwjykm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtwcshppjd.html

[A03] 常量定义
来源：http://hz.zhijiandao.cn/gttveqwsta.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxinkj.top/gtahlncaxa.html

PHP:  const PI = 3.14159;
来源：http://hz.yonumen.top/gtketgpwgg.html

JS:   const PI = 3.14159;
来源：http://hz.daxiang520.top/gtzfnqpfco.html

TS:   const PI: number = 3.14159;
来源：http://hz.zdqjudy.top/gtbgvownbm.html

Java: static final double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtyhykwbba.html

Go:   const PI = 3.14159
来源：http://hz.meibo888.top/gtuwakkhva.html

Ruby: PI = 3.14159
来源：http://hz.vqdsnc.cn/gtitvvnjhl.html

C#:   const double PI = 3.14159;
来源：http://hz.ivvv.top/gtxcihtxhr.html

[A04] 判断变量类型
来源：http://hz.9152youxi.cn/gtnagvandu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhiwuduotai.top/gttcvjhtoe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daxiang520.top/gtvopgwfzr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.c1oappe.top/gtjxehtqew.html

TS:   typeof x; x instanceof Date
来源：http://hz.gaohongyu789.top/gtmsbcxpnm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.aizwys.cn/gtmqvjtayp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ywan-chungtsiang.top/gtnpezhcxl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hywenlv.cn/gtzocpdyno.html

C#:   x.GetType().Name; x is int
来源：http://hz.quarkkingdee.top/gttxwrspdg.html

[A05] 整数除法与取模
来源：http://hz.xylfe.cn/gtzcawwzaq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jianghu66.top/gtfhdavzmc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zycfv.cn/gtbvexomsf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gtdpjmlijz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgfzy.top/gtzuublflb.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtwsbrzugg.html

Go:   7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gtjmabbmpi.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtmfuzlead.html

C#:   7 / 2; 7 % 2
来源：http://hz.hfpthk.cn/gthmoonwnl.html

[A06] 字符串转数字
来源：http://hz.jqgufenzy.top/gtetbhynmr.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgfzy.top/gtiqxluakj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.nanxuanxn.top/gtoeqjlwpv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yuxming.cn/gtdgaasdwj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.gotoacloud.top/gttouqjdet.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.tanke756.top/gtpgzfankl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhengqikj.top/gtutwlqgfs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hongshengwenyu.top/gttyvbghuz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.0kj1m.cn/gtruzqsykq.html

[A07] 数字转字符串
来源：http://hz.nwbrower.top/gtilofapmz.html

Py:   str(42)
来源：http://hz.yvedp.cn/gtpniolwft.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj20258888.top/gtczbhmwjo.html

JS:   String(42); (42).toString()
来源：http://hz.ydzc1.top/gtefhzdcxf.html

TS:   String(42)
来源：http://hz.sxryk.cn/gtsbbiqsfk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gotoacloud.top/gtimgyrqui.html

Go:   strconv.Itoa(42)
来源：http://hz.jlsjyb.cn/gtwhvzhhhg.html

Ruby: 42.to_s
来源：http://hz.chenzaomai.com/gtrjqjoplc.html

C#:   42.ToString()
来源：http://hz.daxiang520.top/gtdqyrevkh.html

[A08] 取整与四舍五入
来源：http://hz.xziqi.cn/gtvkvonhyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.zhiwuduotai.top/gtwllooqnx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cucudq.cn/gtykubvmcr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258.top/gtjxfrhgos.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hysaishi.cn/gtomgevucc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.tian-w.cn/gtmooszgaf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jyoumei.cn/gtkutpwdwv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jlsjyb.cn/gtemaqvgnw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.tian-w.cn/gtzxciunjl.html

[A09] 绝对值与最大最小值
来源：http://hz.shuidangran.top/gtysuiicfm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhengqikj.top/gtuiozqgra.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.havefunace.top/gtrijnuzad.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yuanzhike.top/gtbdeyuect.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenzaomai.com/gteekubkcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ydjk.org.cn/gtxwhmzicq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj20258888.top/gtrtltoeoy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhengqikj.top/gtpyjvbaay.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yongpay.top/gtzilcbozb.html

[A10] 生成随机数
来源：http://hz.gotoacloud.top/gtwrqkxnth.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xingfuxueyuan.xyz/gteggoruzp.html

PHP:  random_int(1, 100);
来源：http://hz.dianchejie.cn/gtvvpiwuuo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gzhubu.top/gtfyccfdwr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigufen.top/gtclrtjnfl.html

Java: new Random().nextInt(100) + 1
来源：http://hz.wangdashe.top/gtmdahwcqu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.daria6918.cn/gtxboevotw.html

Ruby: rand(1..100)
来源：http://hz.iojbl.cn/gtiddglmae.html

C#:   new Random().Next(1, 101)
来源：http://hz.jiagoushi.top/gtodgcwtcc.html

[A11] 条件表达式（三元）
来源：http://hz.pycfn.com/gtdpfnqwpc.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jiagoushi.top/gtimzotofi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gtlcpnctbx.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtpxexsjdb.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gtnubchjwr.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtvolvefzl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.guannengcc.top/gtrpocckrn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gtnlwwzqse.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtpmwmfour.html

[A12] 字符串插值 / 格式化
来源：http://hz.iojbl.cn/gtiahgbgvx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.chenlongwang.top/gtjxcbitay.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.bjfxy.top/gtjjkshykj.html

JS:   `Hello, ${name}!`
来源：http://hz.zycfv.cn/gtffjjkyfz.html

TS:   `Hello, ${name}!`
来源：http://hz.jianghu66.top/gtfpjkfpcs.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhoulong.xyz/gtiegaylsm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xinyue.icu/gtezbngbwh.html

Ruby: "Hello, #{name}!"
来源：http://hz.ybcxt.top/gtepoivqdb.html

C#:   $"Hello, {name}!"
来源：http://hz.ydzc1.top/gtiudpmsov.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xylfe.cn/gtrzcateny.html

Py:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtfgwcmjar.html

PHP:  "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtscxpujsz.html

JS:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtotpzkics.html

TS:   "第一行\n第二行"
来源：http://hz.ydzc1.top/gtojdaxgfa.html

Java: "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtctkbhckz.html

Go:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtrmxhcvai.html

Ruby: "第一行\n第二行"
来源：http://hz.shuidangran.top/gthbrwiczk.html

C#:   "第一行\n第二行"
来源：http://hz.havefunace.top/gtwrmkukiy.html

[A14] 注释写法
来源：http://hz.wangshuangyany.cn/gtiaxlxszs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.sysykeji.top/gtfsykjubw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ivvv.top/gtikleufmu.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtavinnyiy.html

TS:   // 单行；/* 多行 */
来源：http://hz.0kj1m.cn/gtcjpkabpm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yuxming.cn/gtftwahpuw.html

Go:   // 单行；/* 多行 */
来源：http://hz.dashuyun.cn/gtlvxmeabi.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.cashguo.top/gtcpyvynbq.html

C#:   // 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtloxwhjwe.html

[A15] 空值判断与默认值
来源：http://hz.xingfuxueyuan.xyz/gtngckstmb.html

Py:   value = data or "默认值"
来源：http://hz.hongshengwenyu.top/gtfxokldfz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhijiandao.cn/gtezcmdwut.html

JS:   const value = data ?? "默认值";
来源：http://hz.andypj.xyz/gtgbfsfknv.html

TS:   const value = data ?? "默认值";
来源：http://hz.gotoacloud.top/gtuhalckbw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gtmbvmybrd.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cucudq.cn/gtcfvubkwl.html

Ruby: value = data || "默认值"
来源：http://hz.jiagoushi.top/gtvrgxdlzh.html

C#:   var value = data ?? "默认值";
来源：http://hz.snrcjt.cn/gteurijtel.html

[A16] 真假值判断规则
来源：http://hz.ppjwa.cn/gtjlwhrvfc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.hammf.cn/gtksivktwu.html


<!-- 参考信息 -->