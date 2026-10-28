代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.haohaochexian.top/gtfduvtynr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hammf.cn/gtwmoplbsx.html

[U92] JS：深拷贝
来源：http://hz.wangshuangyany.cn/gthqpcaxdb.html

structuredClone(obj)
来源：http://hz.cqqwz.cn/gtgcgsaymn.html

[U93] JS：模板字符串
来源：http://hz.zycfv.cn/gtavowcgey.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtziseevri.html

[U94] JS：箭头函数
来源：http://hz.guannengcc.top/gtlowkqdvg.html

const double = x => x * 2;
来源：http://hz.gzhubu.top/gtgvhlhcer.html

[U95] JS：Promise 包装
来源：http://hz.yj202588.top/gthcrckzua.html

new Promise((resolve, reject) => {})
来源：http://hz.fzhhl.top/gtfwopperq.html

[U96] JS：async/await 与异常
来源：http://hz.0kj1m.cn/gtktbsbnzq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtxhdjwncr.html

[U97] JS：并发请求
来源：http://hz.jiagoushi.top/gtlhkqpfwq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtzwjhhwhh.html

[U98] JS：fetch 带 JSON
来源：http://hz.shanyushiyangkeji.top/gthlzvcldu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.quarkkingdee.top/gtysnydswj.html

[U99] JS：事件监听
来源：http://hz.wangdashe.top/gtipcrlcyn.html

el.addEventListener("click", e => {})
来源：http://hz.ehwqpu.com/gtxnflvrjm.html

[U100] JS：DOM 查询
来源：http://hz.yanxiufei.cn/gtvdcoczkl.html

document.querySelector(".item")
来源：http://hz.havefunace.top/gtcczantan.html

[U101] JS：classList 操作
来源：http://hz.pycfn.com/gtywtlvxqk.html

el.classList.toggle("active")
来源：http://hz.tian-w.cn/gtfjlivlof.html

[U102] JS：本地存储
来源：http://hz.zhiwuduotai.top/gtgpcsjueg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gteyqdizqb.html

[U103] JS：定时器
来源：http://hz.wangshuangyany.cn/gtheititdp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ywan-chungtsiang.top/gtzvhccadr.html

[U104] JS：防抖
来源：http://hz.gzhubu.top/gtpavtitgj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtgsxysqbj.html

[U105] JS：节流
来源：http://hz.guannengcc.top/gtnezwlryk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ybcxt.top/gtnnygfsep.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gteocedmix.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cheryme.top/gtqgwmncre.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtfxaxazir.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigufen.top/gtqrlvcucl.html

[U108] JS：随机整数
来源：http://hz.yanxiufei.cn/gtvoocxgmh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yongpay.top/gtnkaehhed.html

[U109] JS：数组分组
来源：http://hz.daxiang520.top/gtyepwoqwz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtoqgjonqe.html

[U110] JS：数组分块
来源：http://hz.jqgufenzy.top/gtdjlqmkqy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gtufzzlcbe.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gtbarseyyj.html

new Map(Object.entries(obj))
来源：http://hz.shzxlz.cn/gtesdetazi.html

[U112] JS：字符串补位
来源：http://hz.sweek.top/gtvytjmocs.html

"7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtwdmceont.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangkeji.top/gtsnnhpcuw.html

s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtwbyqcirc.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtsrmmieef.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtteqqusfd.html

[U115] JS：生成 UUID
来源：http://hz.jinqigfzy.top/gtlmtxrphb.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtueaoqlda.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.0kj1m.cn/gtbfvoiaye.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtcyhtlfev.html

[U117] JS：单元测试
来源：http://hz.ppjwa.cn/gtwfhgxbwy.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gtxujrywns.html

[U118] JS：开发服务器
来源：http://hz.gzhubu.top/gtwpzkbfzb.html

npm i -D vite;  npx vite
来源：http://hz.chenlongwang.top/gtrxqbqgkj.html

[U119] JS：生产构建
来源：http://hz.jqgfzy.top/gtugzhweio.html

npx vite build
来源：http://hz.hysaishi.cn/gtdjfngxal.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenlongwang.top/gtihawyeda.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtrehrgidk.html

================================================================================
来源：http://hz.316326.xyz/gtnplhpesv.html

统计汇总
来源：http://hz.chenzaomai.com/gtyvjxdssl.html

================================================================================
来源：http://hz.yonumen.top/gtsmewffez.html

按语言统计（条）：
来源：http://hz.zhengqikj.top/gtftovheal.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtitcprfpd.html

PHP ............ 252
来源：http://hz.cucudq.cn/gtykaqsmgb.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtbnvrdhkd.html

TypeScript ..... 212
来源：http://hz.nwbrower.top/gtxfjhtpfl.html

Java ........... 212
来源：http://hz.smart0.xyz/gtbgzyiuae.html

Go ............. 212
来源：http://hz.snrcjt.cn/gtlhhoajzr.html

Ruby ........... 212
来源：http://hz.birdmap.top/gtygyqmwwk.html

C# ............. 212
来源：http://hz.nanxuanxn.top/gtkmvujpyt.html

C .............. 30
来源：http://hz.dashuyun.cn/gtsxnmjkkv.html

C++ ............ 30
来源：http://hz.gzhubu.top/gtsmcrkekn.html

SQL ............ 90
来源：http://hz.9152youxi.cn/gtnygwpvel.html

Bash ........... 80
来源：http://hz.wangdashe.top/gtnuvznjyf.html

Kotlin ......... 15
来源：http://hz.zhiwuduotai.top/gtwinjymrh.html

Swift .......... 15
来源：http://hz.yuxming.cn/gtfppcssut.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtwrqrtudf.html

Perl ........... 10
来源：http://hz.nwbrower.top/gtntvtsisz.html

Scala .......... 10
来源：http://hz.chenlongwang.top/gtsiwxfkhv.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtuenvjbgf.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtslpwlygh.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtbrqtfhgw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtvflvsfyj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtirtvpomu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtlrgtxfia.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtovtszkoz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.meibo888.top/gtbrqhtbfj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.meibo888.top/gtwrhaocwp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtpfovscbk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenjidiqi.icu/gtvnbewaca.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gthqfykqzp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtnvnfaarc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtmlcxfjul.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtptmworkk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtrhijflhg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtvrpuagmp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cheryme.top/gthzgeadla.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtxpyjjjmp.html

Q SQL 专题                              90
来源：http://hz.hammf.cn/gtmtjigabz.html

R Bash 专题                             80
来源：http://hz.jianghu66.top/gtdwvcyqdd.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangtech.top/gtbouxvwiw.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtbnrnoybh.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gtvxrtmcgm.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gteigdxlmp.html

合计                                  2106 条
来源：http://hz.ydjk.org.cn/gtyvdbbzit.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtshgvijkz.html

使用提醒
来源：http://hz.zhaomingkeji.xyz/gtobnfttmy.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtwwcehxzo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuxming.cn/gtkjhrvjoh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtazeskxns.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.316326.xyz/gtljdlcxyf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.52xcode.cn/gtkrynrqbn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tian-w.cn/gtasuyccqd.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtysegjjmw.html

================================================================================
来源：http://hz.zycfv.cn/gtycdaclba.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hongshengwenyu.top/gtgroikyek.html

Common Programming Examples Cheat Book
来源：http://hz.xingfuxueyuan.xyz/gtnqwrzdxu.html

================================================================================
来源：http://hz.hnxiangtu.top/gttdmnmich.html

【收录内容】
来源：http://hz.cashguo.top/gtdbejpanw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gttcezjqgy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jlsjyb.cn/gtddphtuko.html

SQL · Bash · C · C++
来源：http://hz.jinyuanbaomall.cn/gtuucfcone.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj20258.top/gtpmurkloj.html

【使用说明】
来源：http://hz.dianchejie.cn/gttepczgjv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.bjfxy.top/gtxygldrne.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.iojbl.cn/gtbiudjeng.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.c1oappe.top/gtuhbkdbrf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sufxvd.cn/gtzcgssnji.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinyuanbaomall.cn/gtgfkyoieg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtcmzzkrfx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.mhx1999.top/gtoanhehbt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.guowangkeji.top/gtzwivrbaq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.tianlin.xyz/gtjcmqsqpq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nwbrower.top/gtlnqlwqbm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hfpthk.cn/gtjstzzshd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yonumen.top/gtxwxyydmm.html

【文件统计】
来源：http://hz.jinqigfzy.top/gtxhqawyrt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.c1oappe.top/gttzvdcefp.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtekywpswn.html

目  录
来源：http://hz.cucudq.cn/gtfazxekha.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtawpsrgrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtxphqnbmt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtymisuslf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtdnyigjqc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gthlsauymk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtucsckobz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtlwfxaprv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtfgmeojjm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtjiocfdgg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtjwmqrszo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xuanzx.com/gtsxoxwjmu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtzfzunzyd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtnpiwljyu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtqvodzcwl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zycfv.cn/gteohxspmy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cheryme.top/gtcpwomwol.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gthpcacyod.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gttrcvqodf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jyoumei.cn/gtbtndcbni.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dianchejie.cn/gtekedztyn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtpajcnjse.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtfezvinaa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtplmksbby.html

A. 基础语法与类型
来源：http://hz.52xcode.cn/gtealdormc.html

================================================================================
来源：http://hz.daria6918.cn/gtrdvbwhwx.html

[A01] Hello World
来源：http://hz.birdmap.top/gtlnusyvne.html

Py:   print("Hello, World!")
来源：http://hz.xingfuxueyuan.xyz/gtnzskpzzb.html

PHP:  echo "Hello, World!";
来源：http://hz.hongshengwenyu.top/gtjdesphrq.html

JS:   console.log("Hello, World!");
来源：http://hz.dashuyun.cn/gtdmdicsis.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xingfuxueyuan.xyz/gtkvvbsxin.html

Java: System.out.println("Hello, World!");
来源：http://hz.gaohongyu789.top/gtcupaghrr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.havefunace.top/gtyniynyyk.html

Ruby: puts "Hello, World!"
来源：http://hz.yvedp.cn/gtrajkipnc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.daxiang520.top/gtamtbjvgg.html

[A02] 变量声明与赋值
来源：http://hz.wangdashe.top/gtwlrluivn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nwbrower.top/gtdrmhcjyo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gthsuxyrql.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shangyingyoupin.top/gtnvpysxcw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sxryk.cn/gtnfrrrdrd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtccojsofq.html

Go:   name := "Alex"; age := 20
来源：http://hz.quarkkingdee.top/gtcpptolje.html

Ruby: name = "Alex"; age = 20
来源：http://hz.mhx1999.top/gtzmtulxjf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtppkfsgeg.html

[A03] 常量定义
来源：http://hz.hammf.cn/gtzuhgtrck.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.fzhhl.top/gtyvrctxrc.html

PHP:  const PI = 3.14159;
来源：http://hz.snrcjt.cn/gtizmotupg.html

JS:   const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtwhwzkssl.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigfzy.top/gtjnmezcph.html

Java: static final double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtvrfnhpui.html

Go:   const PI = 3.14159
来源：http://hz.vqdsnc.cn/gtexkdckdo.html

Ruby: PI = 3.14159
来源：http://hz.xingfuxueyuan.xyz/gtbsoeeotl.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtyfbcgvck.html

[A04] 判断变量类型
来源：http://hz.xingfuxueyuan.xyz/gtyzlxiphf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxuanxn.top/gtviggnhzx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shzxlz.cn/gtpqmdbtlm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ywan-chungtsiang.top/gtvbwrbhbs.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydzc1.top/gtsyjmcpth.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jqgufenzy.top/gtwgcoqdfo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.sxryk.cn/gtomxhlmqo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ppjwa.cn/gtkxgxzgfn.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtmvkecgig.html

[A05] 整数除法与取模
来源：http://hz.jinghuilouyu.cn/gtgidvlzwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhixingplan.top/gtqoonankw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.guowangkeji.top/gthktwgucy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yueranfly.top/gtjmzenuqp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tianlin.xyz/gtutqwezxj.html

Java: 7 / 2; 7 % 2
来源：http://hz.gzhubu.top/gtfdlxgclm.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhijiandao.cn/gtvknthqsm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gthfcbxldf.html

C#:   7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtaeatcnev.html

[A06] 字符串转数字
来源：http://hz.jiagoushi.top/gttzmwexys.html

Py:   int("42"); float("3.14")
来源：http://hz.chenlongwang.top/gtqlnfxkhz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shanyushiyangtech.top/gtldkehzbo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yj202588.top/gtvxnrhtjv.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinqigfzy.top/gtmsaanibx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.316326.xyz/gtmsclngys.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinghuilouyu.cn/gthxldicen.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.chenjidiqi.icu/gtwjnvvwzj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj20258.top/gteutugmof.html

[A07] 数字转字符串
来源：http://hz.aibaodan.cn/gtvlxleepx.html

Py:   str(42)
来源：http://hz.cheryme.top/gtsxkrpkrn.html

PHP:  (string) 42; strval(42)
来源：http://hz.jinyuanbaomall.cn/gtsxrkbgkn.html

JS:   String(42); (42).toString()
来源：http://hz.iojbl.cn/gtdixtsggm.html

TS:   String(42)
来源：http://hz.shangyingyoupin.top/gthjkppwkk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jinqigufen.top/gtagpyflqh.html

Go:   strconv.Itoa(42)
来源：http://hz.hywenlv.cn/gtqvdsvicd.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gtunbqelhc.html

C#:   42.ToString()
来源：http://hz.ydzc1.top/gtgmyekahl.html

[A08] 取整与四舍五入
来源：http://hz.xinyue.icu/gtoksmkpfy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shuidangran.top/gtjwswgiwu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shzxlz.cn/gtbvzvpywq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.pycfn.com/gtvtlqmdop.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shuidangran.top/gtegmonlhj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.tanke756.top/gtdatftwvx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zycfv.cn/gtdzyzpulz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.aibaodan.cn/gteyefkcar.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtsmafrmtz.html

[A09] 绝对值与最大最小值
来源：http://hz.ydzc1.top/gtuneyjsfz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtivaitlji.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenzaomai.com/gteweyrbqc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.fengsongda.top/gtojuvxlcv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gtawkctzjg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.kuanghao11.cn/gttzqncrgr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.guannengcc.top/gtyzfctlkc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hnxiangtu.top/gtrwzujllr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sysykeji.top/gtcupxfvme.html

[A10] 生成随机数
来源：http://hz.pengpengdd.cyou/gtgerjykbq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.c1oappe.top/gtldgkyuny.html

PHP:  random_int(1, 100);
来源：http://hz.cashguo.top/gtkcphaenn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zycfv.cn/gtwarjztac.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hnxiangtu.top/gtxlczkoqp.html

Java: new Random().nextInt(100) + 1
来源：http://hz.aizwys.cn/gtubqyeclo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xziqi.cn/gtrryeffwu.html

Ruby: rand(1..100)
来源：http://hz.zhiwuduotai.top/gtlqwmpbdv.html

C#:   new Random().Next(1, 101)
来源：http://hz.yanxiufei.cn/gtyjkvbhtl.html

[A11] 条件表达式（三元）
来源：http://hz.redwolf501.top/gtqlwunoiq.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.mhx1999.top/gtfzxspmxl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.guowangkeji.top/gtvhimeays.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hnxiangtu.top/gtxrgopmkw.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtpshpbndl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtbigdtunz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gotoacloud.top/gtyszvyjqx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtsllabjgm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yuanzhike.top/gtykldbbao.html

[A12] 字符串插值 / 格式化
来源：http://hz.vqdsnc.cn/gtosxqxmyz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.quarkkingdee.top/gthijdtjlx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yonumen.top/gtqdrizyuc.html

JS:   `Hello, ${name}!`
来源：http://hz.vqdsnc.cn/gtqeijdjbn.html

TS:   `Hello, ${name}!`
来源：http://hz.xingfuxueyuan.xyz/gtpbolkomj.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.havefunace.top/gtheryofsl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yonumen.top/gtwtuvbmag.html

Ruby: "Hello, #{name}!"
来源：http://hz.vqdsnc.cn/gttgjgpwff.html

C#:   $"Hello, {name}!"
来源：http://hz.yanxiufei.cn/gtpradadld.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.shzxlz.cn/gtooqlnkib.html

Py:   "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtlwenutxz.html

PHP:  "第一行\n第二行"
来源：http://hz.havefunace.top/gtorxsmjje.html

JS:   "第一行\n第二行"
来源：http://hz.c1oappe.top/gtwpbuszwp.html

TS:   "第一行\n第二行"
来源：http://hz.yongpay.top/gtllcwjlpf.html

Java: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtaxypcjvd.html

Go:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtaffhbbxi.html

Ruby: "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtydoigcah.html

C#:   "第一行\n第二行"
来源：http://hz.iojbl.cn/gtgkhiigkv.html

[A14] 注释写法
来源：http://hz.jqgfzy.top/gtowayovkr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jianghu66.top/gtmdyuqtqu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.birdmap.top/gtkeurqzbx.html

JS:   // 单行；/* 多行 */
来源：http://hz.zdqjudy.top/gtxckvvzko.html

TS:   // 单行；/* 多行 */
来源：http://hz.yuxming.cn/gtigtzgpve.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sufxvd.cn/gtdcycamvo.html

Go:   // 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtvztetfpb.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jinghuilouyu.cn/gtxpemajxt.html

C#:   // 单行；/* 多行 */
来源：http://hz.chenzaomai.com/gtqgddlwsx.html

[A15] 空值判断与默认值
来源：http://hz.ivvv.top/gtlxpvtbfk.html

Py:   value = data or "默认值"
来源：http://hz.jyoumei.cn/gtmzomswru.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhijiandao.cn/gtrtgqjibg.html

JS:   const value = data ?? "默认值";
来源：http://hz.ivvv.top/gthkjbsfsz.html

TS:   const value = data ?? "默认值";
来源：http://hz.chenjidiqi.icu/gtchugobuc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.316326.xyz/gtahudaqnm.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.9152youxi.cn/gtukguumli.html


<!-- 参考信息 -->