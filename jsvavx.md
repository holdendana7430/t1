代发 wailian999

[U89] JS：数组去重
来源：http://hz.sufxvd.cn/gtbyjlsajc.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtuvrcoglf.html

[U90] JS：数字数组排序
来源：http://hz.yj20258888.top/gtzwqykncq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtreymmuvz.html

[U91] JS：对象键值遍历
来源：http://hz.xuetiantiany.cn/gtlxjttkwq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hnxiangtu.top/gtzolkzaox.html

[U92] JS：深拷贝
来源：http://hz.c1oappe.top/gtmrjwycbs.html

structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gthjvchhqn.html

[U93] JS：模板字符串
来源：http://hz.wangshuangyany.cn/gtbuzpganl.html

`共 ${n} 条`
来源：http://hz.hongshengwenyu.top/gtauzeckhr.html

[U94] JS：箭头函数
来源：http://hz.cqqwz.cn/gthnairjtc.html

const double = x => x * 2;
来源：http://hz.nanxuanxn.top/gtadcknwaw.html

[U95] JS：Promise 包装
来源：http://hz.shangyingyoupin.top/gtnwywcurn.html

new Promise((resolve, reject) => {})
来源：http://hz.xuetiantiany.cn/gtqfnbjldn.html

[U96] JS：async/await 与异常
来源：http://hz.0kj1m.cn/gtprwichha.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gturuvpdzj.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtcfbjbocr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtmdwgmlwc.html

[U98] JS：fetch 带 JSON
来源：http://hz.yonumen.top/gtgfmqhzlv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhixingplan.top/gtxgstqput.html

[U99] JS：事件监听
来源：http://hz.yonumen.top/gtnjtcgpev.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtjktdazjz.html

[U100] JS：DOM 查询
来源：http://hz.haohaochexian.top/gtvvjttrnh.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtixaqhysv.html

[U101] JS：classList 操作
来源：http://hz.mhx1999.top/gtcnowmmoz.html

el.classList.toggle("active")
来源：http://hz.daria6918.cn/gtnyvnplwt.html

[U102] JS：本地存储
来源：http://hz.hnxiangtu.top/gtltyjabie.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yueranfly.top/gtpgguniyq.html

[U103] JS：定时器
来源：http://hz.xziqi.cn/gtswjrdmtz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tanke756.top/gtwdrvearq.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtxtnntvnc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtvszutsjk.html

[U105] JS：节流
来源：http://hz.yangfankeji.com/gtjxsrcein.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigfzy.top/gtkxmgxygp.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtyqlgqyij.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yangfankeji.com/gtcemdidxu.html

[U107] JS：数字千分位
来源：http://hz.smart0.xyz/gtzihgsofc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.feifeiyinyue.top/gtartilyrs.html

[U108] JS：随机整数
来源：http://hz.snrcjt.cn/gtyrxddtbt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinyuanbaomall.cn/gtumexuges.html

[U109] JS：数组分组
来源：http://hz.gzhubu.top/gttovsfwvw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtjwyimtua.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtsdarbduz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gtugtupluv.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtuqjhlieo.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtrexwbtcz.html

[U112] JS：字符串补位
来源：http://hz.zhengqikj.top/gtrpfugrvb.html

"7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtabtbngze.html

[U113] JS：正则替换全部
来源：http://hz.chenlongwang.top/gthiaeecrv.html

s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtxcspcyxy.html

[U114] JS：JSON 深比较
来源：http://hz.jyoumei.cn/gtbbsaokwx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtammcctfk.html

[U115] JS：生成 UUID
来源：http://hz.0kj1m.cn/gtyydelrkz.html

crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtyjpndrsz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tian-w.cn/gtiyzzocsz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tian-w.cn/gtmfpdxqbe.html

[U117] JS：单元测试
来源：http://hz.daxiang520.top/gtqoouyfll.html

npm i -D vitest;  npx vitest
来源：http://hz.aizwys.cn/gtpwoksaww.html

[U118] JS：开发服务器
来源：http://hz.fzhhl.top/gtxmuugkbb.html

npm i -D vite;  npx vite
来源：http://hz.gotoacloud.top/gtrrirnvmr.html

[U119] JS：生产构建
来源：http://hz.hfpthk.cn/gtsmeqplaa.html

npx vite build
来源：http://hz.zdqjudy.top/gtuytnivfc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gotoacloud.top/gtvufezhlb.html

import.meta.env.VITE_API_URL
来源：http://hz.zhixingplan.top/gttzppkuah.html

================================================================================
来源：http://hz.gaohongyu789.top/gthlsbhnrx.html

统计汇总
来源：http://hz.cdnleiting.top/gtsrposciz.html

================================================================================
来源：http://hz.shuidangran.top/gtaheqqagy.html

按语言统计（条）：
来源：http://hz.cdnleiting.top/gtoesjhrae.html

Python ......... 252
来源：http://hz.meibo888.top/gtbyevlglq.html

PHP ............ 252
来源：http://hz.yvedp.cn/gthqoksmob.html

JavaScript ..... 252
来源：http://hz.0kj1m.cn/gtlpryejla.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gtheiavyyn.html

Java ........... 212
来源：http://hz.zhongyouzk.top/gtqynejrkn.html

Go ............. 212
来源：http://hz.nwbrower.top/gtlwypnraj.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtlbzvdwpy.html

C# ............. 212
来源：http://hz.shuidangran.top/gtbjtevfit.html

C .............. 30
来源：http://hz.daria6918.cn/gtiltsrzpk.html

C++ ............ 30
来源：http://hz.xuanzx.com/gtubwjqrcr.html

SQL ............ 90
来源：http://hz.hysaishi.cn/gtbnxsdyqs.html

Bash ........... 80
来源：http://hz.xinyue.icu/gtlatddxen.html

Kotlin ......... 15
来源：http://hz.xylfe.cn/gtdsetjapq.html

Swift .......... 15
来源：http://hz.zhijiandao.cn/gtiayuhuhf.html

Lua ............ 10
来源：http://hz.yj20258888.top/gtzyxborqh.html

Perl ........... 10
来源：http://hz.aizwys.cn/gtwsjhjbjm.html

Scala .......... 10
来源：http://hz.hfpthk.cn/gtiikhmuop.html

------------------------------------
来源：http://hz.ywan-chungtsiang.top/gteibjwrpi.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gtclcemctq.html

按章节统计：
来源：http://hz.zhiwuduotai.top/gtttxlqmsy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtelawzgnf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtpsikrusu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gthliejvvl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtbvqeyrpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.316326.xyz/gtlcrdvsjn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtwouylsjq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gteyluypvd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtwirtmnaj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtexqjubiz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtnaztjmdh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtaxxhvoua.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtpdwskngl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtieveobwf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtjdpsnbbx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hnxiangtu.top/gtezpnyhjp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gthqohdjbv.html

Q SQL 专题                              90
来源：http://hz.nanxuanxn.top/gtjyykzioc.html

R Bash 专题                             80
来源：http://hz.sxryk.cn/gtpofwyunn.html

S C / C++ 专题                          60
来源：http://hz.aizwys.cn/gtsskpepxa.html

T 其他语言补充                          60
来源：http://hz.quarkkingdee.top/gtonuknvze.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtmizfvwww.html

------------------------------------
来源：http://hz.xylfe.cn/gtlvlcuzsp.html

合计                                  2106 条
来源：http://hz.hfpthk.cn/gtpadajjxr.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtgdlrmtgf.html

使用提醒
来源：http://hz.kuanghao11.cn/gtkzmjzlqt.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtkwcibzvg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.snrcjt.cn/gtkaulmwqd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yonumen.top/gtoffepglg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhiwuduotai.top/gtglzgmrlb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.316326.xyz/gtmizsdzjc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.quarkkingdee.top/gtcfmalxso.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtoackegfu.html

================================================================================
来源：http://hz.hysaishi.cn/gtcniyvewn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.iojbl.cn/gttcgncwmq.html

Common Programming Examples Cheat Book
来源：http://hz.zhixingplan.top/gtgzbdqpgx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfmbetkxt.html

【收录内容】
来源：http://hz.havefunace.top/gtjmeleiog.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shzxlz.cn/gtxlusxzac.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtanmzmslc.html

SQL · Bash · C · C++
来源：http://hz.yonumen.top/gtzriwjqoh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nwbrower.top/gtmbiwfqmr.html

【使用说明】
来源：http://hz.316326.xyz/gtqcteobkl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gaohongyu789.top/gtlzdlobqm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenjidiqi.icu/gtanccdrzx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.gotoacloud.top/gtnndgxunn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtmcrztzjf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.tianlin.xyz/gtclmqgrke.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hammf.cn/gtrnfgprft.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sufxvd.cn/gtuqkbnnyp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cucudq.cn/gtuujnyhwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xingfuxueyuan.xyz/gtzqpjeshp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtjvoozonw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.wangshuangyany.cn/gtzcsbbvsl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jlsjyb.cn/gtywboypxv.html

【文件统计】
来源：http://hz.yj20258888.top/gtdheqiglg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj20258.top/gtkceucggo.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtozkaqyxa.html

目  录
来源：http://hz.zhijiandao.cn/gtqvxlodmk.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtzbypzqxf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtejlcrcnk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtsskhcjec.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fengsongda.top/gtvdtbguwh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.kuanghao11.cn/gteyzvljtw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hnqzz.top/gtxsomnnin.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.guowangkeji.top/gtvglwnmet.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtofvdqtgf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258888.top/gtcrhyuyaq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtbxrjzwxn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xziqi.cn/gthjsdsvob.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtokqvwwhe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtrrfknnrj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtrnxihiwt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenjidiqi.icu/gtesjytloe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinghuilouyu.cn/gtrfehmhqr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtkveqbuvi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hywenlv.cn/gtyipwfnwg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xziqi.cn/gtkezrsfqj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shanyushiyangtech.top/gtisxxwmzj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtkslsuvae.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtempytseg.html

================================================================================
来源：http://hz.0kj1m.cn/gtoqeyzcuo.html

A. 基础语法与类型
来源：http://hz.daria6918.cn/gtpskjwmmj.html

================================================================================
来源：http://hz.zdqjudy.top/gtuffaupkj.html

[A01] Hello World
来源：http://hz.havefunace.top/gtddykvftq.html

Py:   print("Hello, World!")
来源：http://hz.cucudq.cn/gthjwvxfxz.html

PHP:  echo "Hello, World!";
来源：http://hz.zhixingplan.top/gtsrnlxrhz.html

JS:   console.log("Hello, World!");
来源：http://hz.vqdsnc.cn/gtzggnothl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yuxming.cn/gtweyvrecv.html

Java: System.out.println("Hello, World!");
来源：http://hz.sufxvd.cn/gtiydreryq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtloeykard.html

Ruby: puts "Hello, World!"
来源：http://hz.zhaomingkeji.xyz/gtzcbmiuyc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.redwolf501.top/gtxsaoysmh.html

[A02] 变量声明与赋值
来源：http://hz.quarkkingdee.top/gtuxbcpgjs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sysykeji.top/gtoygexwmg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fengsongda.top/gtnurbfgql.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ywan-chungtsiang.top/gtulecazjh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xuetiantiany.cn/gtkrtwhwht.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtxvxdcynb.html

Go:   name := "Alex"; age := 20
来源：http://hz.cashguo.top/gtqnahlzmt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgfzy.top/gtjmqvoqoi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yongpay.top/gtsucblzux.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtvglnwhjm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hfpthk.cn/gtcilbcieb.html

PHP:  const PI = 3.14159;
来源：http://hz.xylfe.cn/gtudxosldp.html

JS:   const PI = 3.14159;
来源：http://hz.yvedp.cn/gtyblodfqa.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtxafscdhi.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtksvppema.html

Go:   const PI = 3.14159
来源：http://hz.ywan-chungtsiang.top/gtvgautooe.html

Ruby: PI = 3.14159
来源：http://hz.dashuyun.cn/gttwjdiosl.html

C#:   const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtibtozqwl.html

[A04] 判断变量类型
来源：http://hz.havefunace.top/gteldivfve.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenzaomai.com/gtpkvelmhu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sweek.top/gtxbgqlpez.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.fengsongda.top/gteiyvudia.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhijiandao.cn/gtfzoehkbw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yj20258.top/gtggklojua.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.daria6918.cn/gtcydtysjy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.birdmap.top/gthfpfutfe.html

C#:   x.GetType().Name; x is int
来源：http://hz.guowangkeji.top/gtndzsxxdk.html

[A05] 整数除法与取模
来源：http://hz.yonumen.top/gtdlcjzkat.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinghuilouyu.cn/gtbnznchnw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.daria6918.cn/gtttxbelqp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jiagoushi.top/gtiwfwckgz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtpmubspho.html

Java: 7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtledrqfer.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtbxjjigdb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtrucefugx.html

C#:   7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtfrpxwdki.html

[A06] 字符串转数字
来源：http://hz.iojbl.cn/gtnozcphji.html

Py:   int("42"); float("3.14")
来源：http://hz.meibo888.top/gtnwukryfc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.tian-w.cn/gtjldqszbr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ppjwa.cn/gtgamrltmt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shuidangran.top/gtkavzddiv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.fzhhl.top/gtvaumuxtw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sysykeji.top/gtcrmvsazh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sysykeji.top/gtovgedghw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhoulong.xyz/gtadjvhehi.html

[A07] 数字转字符串
来源：http://hz.quarkkingdee.top/gtwrelyvzy.html

Py:   str(42)
来源：http://hz.tian-w.cn/gtxqnxkhvi.html

PHP:  (string) 42; strval(42)
来源：http://hz.chenjidiqi.icu/gtnvgvfigc.html

JS:   String(42); (42).toString()
来源：http://hz.jqgufenzy.top/gtbbuoksrf.html

TS:   String(42)
来源：http://hz.vqdsnc.cn/gtsiwrlgtm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sysykeji.top/gtliaznbyc.html

Go:   strconv.Itoa(42)
来源：http://hz.dianchejie.cn/gtvmcxklpo.html

Ruby: 42.to_s
来源：http://hz.316326.xyz/gtbglesfpu.html

C#:   42.ToString()
来源：http://hz.jinyuanbaomall.cn/gtvpbwgmwn.html

[A08] 取整与四舍五入
来源：http://hz.iojbl.cn/gtfddoxdmw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aizwys.cn/gtspycsgif.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shangyingyoupin.top/gtnhncpghf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258.top/gtjyizkvwu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.vqdsnc.cn/gtsqcvmnsz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hywenlv.cn/gtiavlyqpd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.wangdashe.top/gtiexgatdu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.wangdashe.top/gtxmkbifji.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtwvinwaoq.html

[A09] 绝对值与最大最小值
来源：http://hz.fengsongda.top/gtlkbbuwlg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtiydcitgq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gotoacloud.top/gtaihhqwrg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nanxuanxn.top/gtqjbhnetf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yuanzhike.top/gtlxxiviim.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.0kj1m.cn/gtgcyirxab.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.52xcode.cn/gtpcentusx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhoulong.xyz/gtwcxryxnb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ydzc1.top/gtrxmrteuw.html

[A10] 生成随机数
来源：http://hz.ybcxt.top/gtrohnvxvk.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hnxiangtu.top/gtujccsnpf.html

PHP:  random_int(1, 100);
来源：http://hz.zhijiandao.cn/gtusazfwmc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gaohongyu789.top/gtywncqtcj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shanyushiyangtech.top/gtmnefvtcu.html

Java: new Random().nextInt(100) + 1
来源：http://hz.smart0.xyz/gtegszhxit.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xuanzx.com/gtaqapeqbu.html

Ruby: rand(1..100)
来源：http://hz.kuanghao11.cn/gtqvzzpplt.html

C#:   new Random().Next(1, 101)
来源：http://hz.bjfxy.top/gtrogxijiv.html

[A11] 条件表达式（三元）
来源：http://hz.daxiang520.top/gtkdyxczpq.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.tanke756.top/gtkvhvivrp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gtymobtumv.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtbjcwcqmh.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtafvsgrjo.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtfbiivzqr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ydjk.org.cn/gtbhlnodyw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtgoxwyqqy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtduuhzsmh.html

[A12] 字符串插值 / 格式化
来源：http://hz.sxryk.cn/gtxrbytcyb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.aibaodan.cn/gtlhpdndzy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ydjk.org.cn/gtnafizptm.html

JS:   `Hello, ${name}!`
来源：http://hz.yuxming.cn/gtovoagzht.html

TS:   `Hello, ${name}!`
来源：http://hz.yj20258.top/gtinyofliz.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhixingplan.top/gtyimsilev.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinghuilouyu.cn/gtodozgynj.html

Ruby: "Hello, #{name}!"
来源：http://hz.ehwqpu.com/gtjqkmbgwl.html

C#:   $"Hello, {name}!"
来源：http://hz.jinqigfzy.top/gtaiyeumrx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hongshengwenyu.top/gtumhnnckp.html

Py:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtmbbqtnth.html

PHP:  "第一行\n第二行"
来源：http://hz.xylfe.cn/gtrmlcnzjr.html

JS:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtfxaokzmw.html

TS:   "第一行\n第二行"
来源：http://hz.fzhhl.top/gthkpidlyd.html

Java: "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtilzrygye.html

Go:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtotlfnshm.html

Ruby: "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtnepevjrq.html

C#:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtdcgnddxi.html

[A14] 注释写法
来源：http://hz.nanxinkj.top/gthqmcdbwn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhiwuduotai.top/gtpkyhaebv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtpfyajvhs.html

JS:   // 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtvuhlwczm.html

TS:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtxecjkefq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.mhx1999.top/gtxyhqwmdk.html

Go:   // 单行；/* 多行 */
来源：http://hz.ivvv.top/gtccentjui.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.0kj1m.cn/gtpggtscgc.html

C#:   // 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtpthwzqru.html

[A15] 空值判断与默认值
来源：http://hz.hnqzz.top/gtlzwnafrw.html

Py:   value = data or "默认值"
来源：http://hz.sufxvd.cn/gtaawcrrlq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.tianlin.xyz/gturfcxplu.html


<!-- 参考信息 -->